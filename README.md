# Project Instructions

These instructions are for users of the code.

*   Includes 6 classification models, which are efficientnet-b0, inception-V3, resnet50, swintransformer, vit, and visionmamba.
*   The first five models are trained using notebooks. Vision Mamba is stored in the `vim` directory as `.py` files.
*   For the code in the notebooks, first customize/define the dataset class, and then execute sequentially.
*   For the code in the `vim` directory, first install the environment required for Mamba. Then run `dummy_main.py` for testing. If you need to use your own dataset, please use the `main.py` file and modify the `build_dataset` function within `datasets.py`.
*   If you encounter problems during the Mamba environment installation process, you can refer to CSDN: https://blog.csdn.net/leonardotu/article/details/136386581. You can install according to the following commands:

    ```bash
    conda create -n your_env_name python=3.10.13
    conda activate your_env_name
    conda install cudatoolkit==11.8 -c nvidia
    pip install torch==2.1.1 torchvision==0.16.1 torchaudio==2.1.1 --index-url https://download.pytorch.org/whl/cu118
    conda install -c "nvidia/label/cuda-11.8.0" cuda-nvcc
    conda install packaging
    pip install causal-conv1d==1.1.1
    pip install mamba-ssm
    ```

*   If you have questions, please contact: 2210417004@stumail.sztu.edu.cn
