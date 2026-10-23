# SLM-Based Light Control Command System

## Project Overview

This project focuses on developing and training a custom Small Language Model (SLM) to understand light control commands such as `light_on` and `light_off`. The model is designed to process commands and produce the corresponding light-control labels.

The project is developed using **COBNOX**, a programming language with its own dedicated compiler. The model has undergone multiple training experiments to improve its command recognition and response behavior by adjusting the number of model layers and training steps.

The current version uses **2 layers and 55 training steps**. During development, the model was trained and refined through several configurations, resulting in the current working version.

### Latest Training Results

- **Pre-training Loss:** `0.3532`
- **Supervised Fine-Tuning (SFT) Loss:** `0.0005`

The model's sample outputs include `light_on` and `light_off`, demonstrating its intended output format for light-control commands. These loss values represent the recorded training results; additional testing is needed to establish accuracy on unseen commands.

## Key Features

- Custom-trained Small Language Model (SLM).
- Light ON/OFF command recognition.
- Structured command outputs using `light_on` and `light_off`.
- Command-based light state management.
- Multiple training experiments and model configurations.
- Training loss tracking for pre-training and supervised fine-tuning.
- Implementation using the COBNOX programming language and its dedicated compiler.

## Model Training and Development History

The model was developed through several training experiments. The initial configuration did not produce sufficiently accurate responses, so subsequent experiments adjusted the model architecture and training steps.

| Experiment | Model Layers | Training Steps | Observation |
|---|---:|---:|---|
| Initial Version | 1 | 65 | Responses needed improvement |
| Second Experiment | 2 | 40 | Accuracy still needed improvement |
| Third Experiment | 2 | 50 | A working configuration was achieved |
| Current Version | 2 | 55 | Latest working configuration |

These experiments document the model's development process and the changes made to its training configuration.

## Current Version

The current version uses **2 layers and 55 training steps**.

Its main objective is to recognize light-control commands and produce the corresponding output labels:

- `light_on` — represents a request to turn the light on.
- `light_off` — represents a request to turn the light off.

The model is intended to maintain the corresponding command state based on the requested action.

## Training Results and Model Evaluation

### Training Loss

| Metric | Recorded Value |
|---|---:|
| Pre-training Loss | `0.3532` |
| SFT Loss | `0.0005` |

Pre-training loss reflects the training objective during the initial model training stage, while SFT loss reflects the supervised fine-tuning objective.

The recorded SFT loss is low, indicating a close fit to the fine-tuning objective. However, loss values alone do not establish real-world command accuracy or generalization.

### Sample AI Outputs

The following responses were observed during testing:

| Test | AI Response |
|---|---|
| First Reply | `light_on` |
| Second Reply | `light_off` |
| Third Reply | `light_on` |
| Fourth Reply | `light_off` |

These outputs demonstrate the model's intended command-label format. Further testing with varied and unseen inputs can help evaluate its reliability.

## Technology and Development Environment

- **Programming Language:** COBNOX
- **Execution Environment:** COBNOX Compiler
- **Model Type:** Small Language Model (SLM)
- **Application:** Light-control command recognition

The project code is written in COBNOX and should be executed using its appropriate compiler environment. This project does not use a Python or Jupyter Notebook execution workflow.

## How to Run the Project

To run this project, use the COBNOX compiler.

1. Access the COBNOX compiler through its official development environment.
2. Open or obtain the project code from this repository.
3. Ensure that the required model files, training data, and dependencies are available.
4. Follow the compiler's instructions to configure and execute the project.
5. Test the model using light-control commands and inspect the generated outputs.

**To execute the project, open the code in the COBNOX compiler environment and follow the applicable compilation and execution instructions.**

The exact commands and setup requirements depend on the compiler environment and the files included in the repository.

## Learning Outcomes

This project demonstrates practical experience in:

- Custom Small Language Model training.
- Model architecture experimentation.
- Adjusting training steps and evaluating recorded loss.
- Supervised fine-tuning.
- Command recognition and structured output generation.
- State-based light-control logic.
- Using COBNOX and its dedicated compiler for model development.

## Future Improvements

- Expand the supported command vocabulary.
- Evaluate command accuracy using a dedicated test dataset.
- Improve response consistency on unseen inputs.
- Support additional device-control commands.
- Explore integration with physical light-control hardware.

## Conclusion

This project demonstrates the development of a custom-trained Small Language Model for light-control command recognition using COBNOX.

Through multiple training experiments, changes to model architecture, and adjustments to training steps, the model reached its current working configuration of 2 layers and 55 training steps. The recorded training losses and sample outputs provide a starting point for further evaluation and improvement.

The project serves as a foundation for exploring lightweight AI models and command-based automation systems.
