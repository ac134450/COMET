# COMET: Contrastive Mean Teacher for Online Source-free Universal Domain Adaptation

This is the official repository to the paper "COMET: Contrastive Mean Teacher for Online Source-free Universal Domain Adaptation". Some parts of this implementation are based on [mariodoebler/test-time-adaptation](https://github.com/mariodoebler/test-time-adaptation) and [HobbitLong/SupContrast](https://github.com/HobbitLong/SupContrast).

## Usage
### Preparation
- Clone this repository
- Install the requirements by running `pip install -r requirements.txt`

### Source training
We uploaded the checkpoints of our pre-trained source models. To still do the source training yourself, edit the corresponding config file [source_training.yaml](configs/source_training.yaml) accordingly and run the following command: `python fit --config configs/source_training.yaml`

### Source-only testing
To test without adaptation, i.e. to get the source-only results, edit the corresponding config file [source_only_testing.yaml](configs/source_only_testing.yaml) to select the desired scenario 

### Target adaptation
We provide all config files we used for the target adaptation in the folder [configs](configs). To perform the target adaptation, select the config file corresponding the your desired scenario and run the following command: `python fit --config configs/.../selected_config_file.yaml`
