# Object Mover (Avataar Assignment)

Please Use Avataar_Assignment_New instead of Avataar_Assignment
and preferably run on kaggle notebooks for seamless connection to dataset
containing given example images and some weights (pth files)

The link to notebook is: https://www.kaggle.com/code/ronitkhurana/avataar-assignment-cont

(Some parts of this readme file might mention about the outdated Avataar_Assignment.ipynb, the new ipynb has been updated to use GroudingSAM)

(Wherever this readme mentions V1, it refers to Avataar_Assignment.ipynb, and wherever it mentions V2, it refers to Avataar_Assignment_new.ipynb)



## Overview

The Object Mover is an innovative tool designed for effortless image manipulation, allowing users to relocate specific objects within a selected image. This project utilizes advanced deep learning techniques, including the YOLOv3 (You Only Look Once) and GroundingDINO algorithms for object detection and the Segment Anything Model (SAM) for accurate image segmentation. By combining these powerful technologies, the Object Mover provides an intuitive and efficient way to manipulate images.
<br><br>
<b>
This readme file is written to explain the features and usage to the recruiters at Avataar. Thanks for checking my assignment out. Hope you like it!
</b>

## Features

- **Object Detection** Utilizes YOLOv3(Avataar_Assignment.ipynb)/GroundingDINO(Avataar_Assignment_New.ipynb) to identify objects in the selected image
- **Smart Mask Generation** Employs SAM to create precise masks for the detected objects
- **Outpainting Capability** Automatically extends images and fills in background areas when objects are near the edges (WIP for GroundingSAM version, will be pushed within few hours)
- **Seamless Inpainting** Effectively removes the original object and inpaints the background for a natural look

## Workflow

1. **Run the Program**

   Execute the main script using Python or run the notebook on colab/kaggle notebooks/jupyter.
   
3. **Select an Image**
  
   Upon running, you'll be prompted to choose an image
   Enter your image path to continue
   The new version will automatically extract the object to be segmented based on image name

   <em>On google colab/local, you can add your own image </em>


4. **Processing**

   The script will

   - Detect the specified object using YOLOv3/GroundingDINO
   - If the object is near the image edge, it will extend the image and perform outpainting
   - Generate a precise mask of the object using SAM
   - Inpaint the background to remove the object seamlessly
   - Relocate the object to a new position within the image

8. **View Results**

    The final image with the relocated object will be saved as `final_image_with_subject.png` in the working directory; additionally, intermediate steps are visualized for better understanding

## Dependencies

- **YOLOv3** For object detection in V1
- **GroundingDINO** For object detection in V2
- **Segment Anything Model (SAM)** For image segmentation
- **OpenCV** For image processing and manipulation
- **NumPy** For efficient numerical operations on matrices
- **Matplotlib** For displaying/plotting images for immediate visualization

## Why you Should Hire me at Avataar

This project has been an incredible journey through the world of machine learning! Working on this tool to move objects allowed me to dive deep into exciting technologies like YOLOv3, GroundingDINO and SAM. I came across many issues during the completion of this project, but was able to breeze past all of them, using help from stackoverflow, github issues, and some guidance from Harsh Maheshwari Sir.

I believe my hands-on experience with these advanced models and my passion for creative problem-solving make me a fantastic fit for Avataar. I’m all about turning complex challenges into seamless solutions, just like this project, along with all the other projects i have worked at (Do check them, now that you are on my github profile)

So, if you’re looking for someone who can bring enthusiasm and innovation to your team, look no further! Let’s create some amazing AI experiences together!

   
