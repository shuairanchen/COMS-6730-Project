# COMS-6730-Project

# Dataset
- Person Detection Model Dataset:
- https://www.kaggle.com/datasets/laundaactive/person-detection-yolov8n-dectection
- 26 Class Model Dataset:
- https://www.kaggle.com/datasets/mohamedgobara/26-class-object-detection-dataset

# Base Model Training
- You could use the Third Cell in the Code which has model.train() function to training the base model by yourself
- If you don't want training the model, you could get the model weights we trained by the following links：
- https://drive.google.com/drive/folders/1LCDbRsVFyJXFq2XfSf1YkDt8tXx_cKdZ?usp=drive_link

# Code Files
- CustomPGDAttack.ipynb (Our PGD Attack on the Base Model for No Person)
- ADVTraining.ipynb (Our PGD Attack on the Advarsarial Model for No Person)
- 26_Class_of_PGDAttack.ipynb (Our PGD Attack on the 26 Class Model for No Person)
- All_Person_26_Class_of_PGDAttack.ipynb (Our PGD Attack on the 26 Class Model for All Person)
- abstraction folder demonstrates the abstraction based attack

# Video Demo
- You could find the "PGD Attack Demo.mp4" file under the link folder which showed our PGD Attack worked, and how to run the code：
- https://drive.google.com/drive/folders/1LCDbRsVFyJXFq2XfSf1YkDt8tXx_cKdZ?usp=drive_link

# PGD Attack Function
- For PGD attack, you could just run the attack_and_show_image() function with the follow parameters:
- model: YoloV8 model with weights loaded
- image_path: path to the input image file (string)
- epsilon: maximum range of adversarial perturbation
- alpha: step size for updating adversarial perturbation in each iteration
- num_iter: number of iterations of adversarial attack
- class_range: list of all class names that the model can detect
- If your model target class is different with our dataset, you need change the parameter "target_class" in the pgd_attack() function to your target class index of the model

# How to run the code
- Dependency : python 3.12
- Install the required libraries using the following command
```first cell of the notebook contain the required dependency make sure to install them before executing the code
- Run the remaining cells of the notebook to execute attack and generate the results


