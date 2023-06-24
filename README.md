# TFOD Tensorflow Object Detection Walkthrough

This set of Notebooks provides a complete set of code to be able to train and leverage your own custom object detection model using the Tensorflow Object Detection API.

# STEPS

# Step 1:

  Clone this repository:https://github.com/Vicky-Projects/object-    detection.git

# Step 2: Create a new virtual environment

    python -m venv ROOM

# Step 3: Activate your virtual environment

    source ROOM/bin/activate # Linux

    .\ROOM\Scripts\activate # Windows 

# Step 4: Install dependencies and add virtual environment to the Python Kernel

    python -m pip install --upgrade pip

    pip install ipykernel

    python -m ipykernel install --user --name=ROOM

# Step 5:

Collect images using the Notebook 

1. Image Collection.ipynb - ensure you change the kernel to the virtual
   environment as shown below

   <a href="https://ibb.co/82j8NrF"><img src="https://i.ibb.co/Dk7Kz93/Untitled-presentation.jpg" alt="Untitled-presentation" border="0"></a><br /><a target='_blank' href='https://poetandpoem.com/Robert-Frost/Dust-of-Snow'>dust of snow robert frost</a><br />

# Step 6: 

Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders.

    \TFODCourse\Tensorflow\workspace\images\train

    \TFODCourse\Tensorflow\workspace\images\test

# Step 7: 

Begin training process by opening 

2. Training and Detection.ipynb, 

  this notebook will walk you through installing 

    Tensorflow Object Detection,
  
    making detections, 
  
    saving and 
  
    exporting your model.

# Step 8: 

During this process the Notebook will install Tensorflow Object Detection. 

You should ideally receive a notification indicating that the API has installed successfully 

# At Step 8 with the last line stating OK.

![image](https://github.com/Vicky-Projects/object-detection/assets/136788912/ecc896ed-a73a-4a13-b79c-4b1200a5fe6a)

If not, resolve installation errors by referring to the Error Guide.md in this folder.

# Step 9: 

Once you get to step 6. Train the model, inside of the notebook, you may choose to train the model from within the notebook. I have noticed however that training inside of a separate terminal on a Windows machine you're able to display live loss metrics.

![image](https://github.com/Vicky-Projects/object-detection/assets/136788912/deb7bf8e-2b2b-42ed-9a0f-aeac6cdc76ec)

# Step 10: 

You can optionally evaluate your model inside of Tensorboard. Once the model has been trained and you have run the evaluation command under Step 7. Navigate to the evaluation folder for your trained model 

e.g.cd Tensorlfow/workspace/models/my_ssd_mobnet/eval
and open Tensorboard with the following 

    command=tensorboard --logdir=. 

Tensorboard will be accessible through your browser and you will be able to see metrics including mAP - mean Average Precision, and Recall.

