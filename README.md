# Waste-Image-Classifier-with-Transfer-Learning-VGG16
## Table of Contents
- [Overview](#overview)
- [Aim of the Project](#aim-of-the-project)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation & How to Run](#installation--how-to-run)
- [Screenshots / Demo](#screenshots--demo)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Overview
EcoClean currently lacks an efficient and scalable method to automate the waste sorting process. The manual sorting of waste is not only labor-intensive but also prone to errors, leading to contamination and inefficient recycling. To address these issues, I have developed this project to use transfer learning and image classification to automate waste sorting.

## Aim of the Project
The aim of this project is to develop an automated waste classification model that can accurately differentiate between recyclable and organic waste based on images. By the end of this project, I aim to provide a robust solution to improve the efficiency and accuracy of the waste sorting process.

## Technologies Used
- **Programming Language:** Python
- **Libraries:** TensorFlow, Keras, OpenCV
- **Tools:** Jupyter Notebook, Git, VS Code

## Prerequisites
- Python (version 3.6 or higher)
- Git
- Jupyter Notebook

## Installation & How to Run
To set up and run the project locally:

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/ImaadhRenosh/Waste-Image-Classifier-with-Transfer-Learning.git
    cd Waste-Image-Classifier-with-Transfer-Learning
    ```

2. **Install Dependencies**: Install the required libraries using:
    ```sh
    !pip install tensorflow==2.17.0 | tail -n 1
    !pip install numpy==1.24.3 | tail -n 1
    !pip install scikit-learn==1.5.1  | tail -n 1
    !pip install matplotlib==3.9.2  | tail -n 1
    ```

3. **Run the Jupyter Notebook**: Launch Jupyter Notebook and open `Final Proj-Classify Waste Products Using TL FT.ipynb` to train and evaluate the model.

4. ## Jupyter Notebook
    You can find the Jupyter notebook used for this project [here](https://github.com/ImaadhRenosh/Waste-Image-Classifier-with-Tranfer-Learning-VGG16/blob/main/Waste-Image-Classifier-with-Transfer-Learning%20FT.ipynb)
   

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Importing Required Libraries</h2>
  <hr/>
  <img width="716" alt= <img width="725" alt="Screenshot 2025-04-04 at 03 26 27" src="https://github.com/user-attachments/assets/be4451ef-f2e8-45ab-a3b0-21081111d693" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Importing Data</h2>
  <hr/>
  <img width="1011" alt= <img width="903" alt="Screenshot 2025-04-04 at 03 31 23" src="https://github.com/user-attachments/assets/e3225879-21b3-4e67-8099-1329753cfbdd" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Defining configuration options</h2>
  <hr/>
  <img width="456" alt= <img width="455" alt="Screenshot 2025-04-04 at 03 35 02" src="https://github.com/user-attachments/assets/1b6b6a83-526a-4393-98bc-78e3e57f1219" />
  
</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>ImageDataGenerators</h2>
  <hr/>
    <img width="863" alt="Screenshot 2025-04-04 at 03 38 51" src="https://github.com/user-attachments/assets/1531a185-a033-424e-b46d-d0f81d99dba6" />
    <img width="439" alt="Screenshot 2025-04-04 at 03 40 05" src="https://github.com/user-attachments/assets/e7ffe606-8976-4f64-9ecb-10e028a6ee95" />
  
</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 1: Creating a test_generator using the test_datagen object</h2>
  <hr/>
  <img width="819" alt="Screenshot 2025-04-04 at 03 43 13" src="https://github.com/user-attachments/assets/706e1f62-f117-4e05-a9c4-b4debbf66ca4" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Let's look at a few augmented images</h2>
  <hr/>
  <img width="908" alt="Screenshot 2025-04-04 at 03 44 49" src="https://github.com/user-attachments/assets/5926b1ec-c2b9-4a51-a0bf-026951319ffc" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Pre-Trained Models / VGG-16</h2>
  <hr/>
  <img width="904" alt="Screenshot 2025-04-04 at 03 46 13" src="https://github.com/user-attachments/assets/958dc8cc-edf2-4ccf-ba6a-9649bc659a75" />
  <img width="903" alt="Screenshot 2025-04-04 at 03 47 10" src="https://github.com/user-attachments/assets/304dc80e-4370-41b8-8c7e-e1b02a4508d5" />
    
</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Model Summary</h2>
  <hr/>
  <img width="739" alt="Screenshot 2025-04-04 at 03 48 11" src="https://github.com/user-attachments/assets/f7ccf9bc-1f1c-4e88-8998-e4496ba3b7b4" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 2: Compile the Model</h2>
  <hr/>
  <img width="590" alt="Screenshot 2025-04-04 at 03 49 43" src="https://github.com/user-attachments/assets/cf562756-deb9-471f-9a04-256cf461ea95" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Callback function with Learning Rate Scheduler</h2>
  <hr/>
  <img width="745" alt="Screenshot 2025-04-04 at 03 50 36" src="https://github.com/user-attachments/assets/2d6b41c7-9a7e-4c99-975b-d557d349b788" />
</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 3: Fit and train the model</h2>
  <hr/>
  <img width="681" alt="Screenshot 2025-04-04 at 03 52 50" src="https://github.com/user-attachments/assets/02a925cd-1ab6-4e38-baad-e0554b6be370" />
  <img width="912" alt="Screenshot 2025-04-04 at 03 53 55" src="https://github.com/user-attachments/assets/de296e94-7edf-42cd-a05e-daa7cba19874" />
    
</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 4: Plot loss curves for training and validation sets (extract_feat_model)</h2>
  <hr/>
    <img width="699" alt="Screenshot 2025-04-04 at 03 58 05" src="https://github.com/user-attachments/assets/1e333b05-6684-4849-9cef-48849a1a739b" />
    <img width="476" alt="Screenshot 2025-04-04 at 03 58 34" src="https://github.com/user-attachments/assets/ad728e93-3875-4114-a4a8-31760ec437cd" />
  
</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 5: Plot accuracy curves for training and validation sets (extract_feat_model)</h2>
  <hr/>
    <img width="866" alt="Screenshot 2025-04-04 at 04 00 39" src="https://github.com/user-attachments/assets/4dbfa82b-c38d-49ec-a071-31392a66af24" />
    <img width="497" alt="Screenshot 2025-04-04 at 04 01 13" src="https://github.com/user-attachments/assets/c1850242-af1f-461e-8e99-c83307d15aab" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 6: Fine-Tuning model</h2>
  <hr/>
  <img width="743" alt="Screenshot 2025-04-04 at 06 02 20" src="https://github.com/user-attachments/assets/7ac6497e-1bf0-47ec-9ba3-78303b637267" />
  <img width="578" alt="Screenshot 2025-04-04 at 06 03 05" src="https://github.com/user-attachments/assets/bb60cad8-0fad-43ea-82af-5f696836b3a6" />

</div>


<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Similar to what was done before, I will create a new model on top, and add a Dropout layer for regularization</h2>
  <hr/>
  <img width="747" alt="Screenshot 2025-04-04 at 06 04 09" src="https://github.com/user-attachments/assets/aa011441-2500-4464-ba0a-51c794224aa5" />
  <img width="923" alt="Screenshot 2025-04-04 at 06 04 47" src="https://github.com/user-attachments/assets/156c1c6a-4cb6-4e34-9f02-af5b0e65cf6c" />


</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 7: Plot loss curves for training and validation sets (fine-tune model)</h2>
  <hr/>
  <img width="866" alt="Screenshot 2025-04-04 at 06 06 06" src="https://github.com/user-attachments/assets/5b0b9c7c-d9e0-49c8-bbe0-7c6f126fd364" />
  <img width="482" alt="Screenshot 2025-04-04 at 06 06 49" src="https://github.com/user-attachments/assets/897ad787-cdd0-423a-857b-ca1f1a9c3cbc" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 8: Plot accuracy curves for training and validation sets (fine tune model)</h2>
  <hr/>
  <img width="864" alt="Screenshot 2025-04-04 at 06 07 39" src="https://github.com/user-attachments/assets/2e339d06-f696-4d0b-b788-3da121fa5131" />
  <img width="483" alt="Screenshot 2025-04-04 at 06 08 03" src="https://github.com/user-attachments/assets/7b734ef8-fd54-4a84-95d9-fc0188e26b0b" />


</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 9: Evaluate both models on test data</h2>
  <hr/>
  <img width="899" alt="Screenshot 2025-04-04 at 06 08 51" src="https://github.com/user-attachments/assets/a63f61de-2184-4772-82e0-5b88ad1ba407" />
  <img width="896" alt="Screenshot 2025-04-04 at 06 09 12" src="https://github.com/user-attachments/assets/6c13e8e2-b16b-47d0-8e27-1b59b1d2ccd2" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 10: Plot a test image using Extract Features Model (index_to_plot = 1)</h2>
  <hr/>
    
  <img width="451" alt="Screenshot 2025-04-04 at 06 09 46" src="https://github.com/user-attachments/assets/c6cdec18-9981-4a20-b42c-de73b51a981d" />
  <img width="897" alt="Screenshot 2025-04-04 at 06 10 32" src="https://github.com/user-attachments/assets/352a58af-1efe-4799-8c69-fefab40997a6" />

  <img width="1005" alt="Screenshot 2025-03-15 at 07 55 58" src="https://github.com/user-attachments/assets/bca84ab8-264b-4b34-82fc-20c6b84411b8" />
  <img width="580" alt="Screenshot 2025-03-15 at 07 56 19" src="https://github.com/user-attachments/assets/65d43694-01d6-4680-b044-28e862d7b219" />
  <img width="397" alt="Screenshot 2025-03-15 at 07 56 41" src="https://github.com/user-attachments/assets/dc771448-ac2c-4248-b634-da3b82b69cb8" />

</div>

<div style="margin-top: 30px; margin-bottom: 30px;">
  <h2>Step 11: Plot a test image using Fine-Tuned Model (index_to_plot = 1)</h2>
  <hr/>
<img width="897" alt="Screenshot 2025-04-04 at 06 12 49" src="https://github.com/user-attachments/assets/17c945a6-c9ae-41ba-9020-5bddae1c1012" />

  
  
</div>


## Usage
After launching the Jupyter Notebook, you can:
- Upload images of waste.
- The model will classify the waste as either recyclable or organic.

## Contributing
Contributions are welcome! If you’d like to improve this project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push the branch.
4. Open a pull request detailing your changes.

## License
This project is licensed under © IBM Corporation. All rights reserved.

## Acknowledgements
- Thanks to the contributors of TensorFlow, Keras, and OpenCV.
- Special thanks to the EcoClean team for their support and collaboration.

## Contact
For any questions or suggestions, feel free to reach out:
- **Email:** imaadhrenosh@gmail.com
- **LinkedIn profile**: [LinkedIn profile](https://www.linkedin.com/in/imaadh-renosh-007aba348)


