# Machine-Learning-Driven-Optimization-of-Airfoil-Design-for-Noise-Reduction

# Project Overview


This project aims to build a machine learning pipeline to predict sound levels based on features from the NASA Airfoil Self Noise dataset. An airfoil is a streamlined shape designed to generate lift when air flows over it, commonly used in aircraft wings and the bodies of sports cars to enhance performance. The design of an airfoil significantly impacts its aerodynamic efficiency and noise generation.

![image](https://github.com/user-attachments/assets/b62197f0-831c-4f99-b2e6-764fb7c37eb3)



The angle of attack refers to the angle between the chord line of the airfoil and the oncoming airflow. It plays a critical role in determining the airflow patterns over the airfoil and, consequently, the sound levels produced. By accurately predicting noise levels associated with various angles of attack, this project allows engineers to optimize airfoil designs for reduced noise and improved performance.
![image](https://github.com/user-attachments/assets/6bf44718-0241-4f80-8471-811f538ce6e0)


Accurate noise prediction is essential in the aeronautics industry, enabling engineers to design quieter and more efficient airfoils. By streamlining the data cleaning and model training processes, this project enhances design efficiency, supports data-driven decision-making, and reduces time and costs. The scalable pipeline can be adapted for various predictive tasks, and by persisting the trained model, it ensures ongoing innovation and alignment with sustainability goals.

# Objectives
1) In this project, we will:

2) Perform ETL Activity

3) Load the CSV dataset.

4) Remove duplicates and drop rows with null values.

5) Transform the data and store it in Parquet format.

6) Create a Machine Learning Pipeline:

7) Develop a machine learning pipeline for predicting sound levels.


8) Assess the model's performance using relevant metrics.

9) Persist the Model.

10)Save the trained model for future production use and verify the stored model.


# Dataset
The dataset used in this project is the NASA Airfoil Self Noise dataset. It is licensed under a Creative Commons Attribution 4.0 International (CC BY 4.0) license.

# Conclusion
The machine learning pipeline was used to predict airfoil noise levels, with the following key outcomes:

### Model Performance:

Mean Squared Error (MSE): 22.59

Mean Absolute Error (MAE): 3.73

R-squared (R2): 0.54

These metrics indicate that the model has moderate predictive power, explaining about 54% of the variance in the sound level data.

### Feature Importance:
The linear regression coefficients reveal the impact of each feature on the predicted sound level:

Frequency: -3.9728

AngleOfAttack: -2.4775

ChordLength: -3.3818

FreeStreamVelocity: 1.5789

SuctionSideDisplacement: -1.6465

This suggests that:

Increasing frequency, angle of attack, chord length, and suction side displacement tend to decrease the sound level.
Increasing free stream velocity tends to increase the sound level.

Frequency has the largest impact on sound level, followed by chord length.



### Model Usability:
The pipeline model was successfully saved and loaded, demonstrating its potential for deployment in real-world applications. This allows for easy reuse of the model for predicting airfoil noise levels without needing to retrain.



In conclusion, this project developed a functional machine learning pipeline for predicting airfoil noise, providing insights into the factors affecting noise levels. While the model shows moderate accuracy, it offers a foundation for further refinement and could be valuable in aircraft design processes aimed at noise reduction.
