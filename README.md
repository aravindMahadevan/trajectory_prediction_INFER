# ECE 285 trajectory prediction project


## Instructions 

1. Go to the [Nuscenes github page](https://github.com/nutonomy/nuscenes-devkit#nuscenes) and install the devkit. Once the devkit is installed, download the data set from the [Nuscenes website](https://www.nuscenes.org/download). In our experiments, we were only able to download the first 85 scenes from the TrainVal dataset. 
2. Use the semantic segmentation network [here](https://github.com/mapillary/inplace_abn) to segment the camera images in the TrainVal dataset. Ensure that the destination directory for the semantically segmented camera images is different than the source directory. 
3. When segmentation is finished, rename the source directory where the camera originated to a different name such as CAM_FRONT_OLD and rename the target directory to the previous source destination name. This step is important because it allows us to access the segmented camera images using the functions provided by the nuscenes devkit. 
4. Construct the intermediate representation using generate_data.py. 
5. Train the model using train_safety.py
