# Notebooks for running prediction and quantification of on malarial gametocyte stages.
Code written by Michael Mckay from BAC for Katrina Larcher for training of a YoloV8 network to classify stages of malarial parasite infection of red blood cells

## Code
train_yolo.ipynb is for training of yolo network with both standard and custom augmentation
run_counts_predictions.ipynb is for running counting and prediction of new images

## Classes
    -Early
    -stage 2
    -stage 3
    -stage 4
    -stage 5
    -debris 

Most classes will have good results with high confidence values, stage 4 is difficult and ambiguous but results should be around ~60% accurate
    
## Steps for usage
    1. Select environment from list by clicking select kernal in the top right. The environment is located in /vast/projects/BAC_shared/conda_envs/yolo_env
    2. Modify filepaths for model weights and location of images to predict. Images must be in .jpg or .png format
    3. Run cells by selecting run all at the top or selecting individual cells and pressing shift+enter
    4. Csv counts and confidence values csv files will be output in the directory and will be replaced with every run. Make sure to download them each time after running counting

# For deployment
-make sure she can see and select environment
-generate .requirements file
-adjust file paths for her workspace
-download weights files

# Env details
python=3.12
