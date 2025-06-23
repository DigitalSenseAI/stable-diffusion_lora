# Stable Diffusion - FineTuning with LoRA and Dreambooth
Technical activity - Sensational Week - June 2025

## Getting started

In this example we will work on the servers
- Hefesto
- Afrodita
- Hercules

Each group is assigned to one server

### Log in to the server assigned
Your user-name is <name.surname> and the IPs are:
* Hefesto: `192.168.0.225`
* Afrodita: `192.168.0.227`
* Hercules: `192.168.0.222`

```bash
ssh <user-name>@<server-ip>
```
### Create / Activate conda env

Currently, we have different paths for conda bin. 
* In **hercules** is `/data/miniconda3/bin/conda`
* In **hefesto** and **afrodita**: `/mnt/data/miniconda3/bin/conda`

There an env already created. Activate it with (be careful to change the conda path according to the server you're using):
```bash
<conda-bin-path> activate lora
```

example for Hefesto: `/mnt/data/miniconda3/bin/conda activate lora`

#### In case you need to create it:
```bash
<conda-bin-path> create -n lora python=3.11
<conda-bin-path> activate lora
pip install -r requirements.txt
```

## Train with lora
Follow the steps in [lora_training.ipynb](lora_training.ipynb)
