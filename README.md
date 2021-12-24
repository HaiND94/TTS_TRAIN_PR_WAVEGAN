# This version use for training TTS

Here there are vocoder model implementations which can be combined with the other TTS models.

Currently, following models are implemented:

- Melgan
- MultiBand-Melgan
- ParallelWaveGAN

It is also very easy to adapt different vocoder models as we provide a flexible and modular (but not too modular) framework.

## Training a model

For training, you must be run step by step:


### Step 1: Must be set model_config.json file and vocoder_config.json file follow your data
### Step 2: run in terminal follow
    - pip install -r requirements.txt
    - python compute_statistics.py --config_path model_config.json --out_path ./
    - CUDA_VISIBLE_DEVICES="0" python train_tts.py --config_path model_config.json
    - CUDA_VISIBLE_DEVICES="0" python train_vocoder.py --config_path vocoder_config.json
    
    

