
# Usage
### Installation:
1. Create the environment from the <kbd>environment.yml</kbd> file:

        conda env create -f environment.yml

2. Activate the new environment:

        conda activate uie

3. Verify that the new environment was installed correctly:

        conda env list

You can also use <kbd>conda info --envs</kbd>.

### Train:
Use this line to train the model

        python train.py --cuda_id 0 --exp CCMSRNet.yml
### Test:
Use this line to predict results

        python test.py --cuda_id 0 --exp CCMSRNet.yml --ckpt ./weights/checkpoint.pth --input path_to_img_folder --output path_to_save_folder

# Results

![](./imgs/C60_half.png)
![](./imgs/RUIE_half.png)
