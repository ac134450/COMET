# COMET: Contrastive Mean Teacher for Online Source-free Universal Domain Adaptation

This is the official repository to the paper "COMET: Contrastive Mean Teacher for Online Source-free Universal Domain Adaptation". Some parts of this implementation are based on [mariodoebler/test-time-adaptation](https://github.com/mariodoebler/test-time-adaptation) and [HobbitLong/SupContrast](https://github.com/HobbitLong/SupContrast).

## Usage
### Preparation
- Clone this repository
- Install the requirements by running `pip install -r requirements.txt`

### Source training
We uploaded the checkpoints of our pre-trained source models. To still do the source training yourself by running the following command:
`python fit --config configs/source_training.yaml`

### Target adaptation
