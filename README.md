## Training Results and Model Evaluation

### Training Loss

- **Pre-training Loss:** `0.3532`
- **Supervised Fine-Tuning (SFT) Loss:** `0.0005`

These values represent the loss recorded during the model's pre-training and supervised fine-tuning stages. The low SFT loss indicates that the model fits its fine-tuning training objective closely; however, performance on unseen commands should be evaluated separately.

### Sample AI Outputs

The following outputs were observed during testing:

| Test | AI Response |
|---|---|
| First Reply | `light_on` |
| Second Reply | `light_off` |
| Third Reply | `light_on` |
| Fourth Reply | `light_off` |

### Results Summary

The current model produces light-control labels such as `light_on` and `light_off`. These outputs demonstrate the intended command-label format for the project.

Further evaluation with different commands and unseen test examples can help assess the model's response consistency and generalization.
