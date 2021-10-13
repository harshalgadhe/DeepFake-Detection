<h1>DeepFake-Detection</h1>

<b>DeepFake</b> is a technique that aims to replace the face of a targeted person with the face of someone else in a video. It first appeared in autumn 2017 as a script used to generate face-swapped adult content. We have proposed a model which can be used to detect the forged video and hence can become a great public concern recently. 

<h1> Comparision between the proposed model with model used in the Research Paper</h1>
<ul>
  <li>We used different preprocessing model than the one used in the research paper</li>
  <li>Our dataset is lesser than the one originally used </li>
  <li>To solve the problem of dataset we use data augmentation techniques</li>
  <li>We biild our own prediction model so that one can do prediction for the video without having to understand the code, you just need to add the path</li>
  <li>Well balanced dataset with each category having around 800 images</li>
</ul>

<h1>Setting up the model locally or on Colab</h1>
You can run our model locally as well on colab by uploading the .ipynb file on your colab. For running the model on your computer you will have to download dependencies. For downloading click on <a href='https://github.com/harshalgadhe/DeepFake-Detection/blob/main/requirements.txt'>Requirements File</a>. After downloading you need to run the code by opening the command propmt and pasting the following code:
pip install -r /path to requirements.txt file.

<h1> Datasets and Weights file </h1>
<br>
<a href='https://www.kaggle.com/c/deepfake-detection-challenge/data'>Dataset</a>  -> This link contains dataset having videos which were later pre processed. For that you need to first login to kaggle <br>
<a href='https://drive.google.com/drive/folders/1ZEWRR9M7M2RW2h28lPRZHCYGAGl5U0q9?usp=sharing'>Preprocessed Dataset</a><br>
<a href='https://drive.google.com/drive/folders/1CAzFPJyb3vOelGo9N45UkIek1psDKSon?usp=sharing'>Weights File</a><br>

<h1>Model</h1>
The proposed model used Meso-4 Architecure as in the research paper <a href='https://arxiv.org/pdf/1809.00888v1.pdf'>MesoNet: a Compact Facial Video Forgery Detection Network
</a> and was used for prediction of Fake Videos. We build our own custom model for data preprocessing and prediction which can be found in the .ipynb file. Model trained with accuracy of over 75% on training data and over 60% on testing data. Though the model show overfitting but it can be solved by adding more data. The graphs for accuracy and loss is as follows : <br><br>
<img src='https://github.com/harshalgadhe/DeepFake-Detection/blob/main/images/accuracy.png'>
<img src = 'https://github.com/harshalgadhe/DeepFake-Detection/blob/main/images/loss.png'><br>
<h3>The results of the prediction model when tested on unseen data is as follows. As you can see the model was able to predict correctly.</h3><br>
<img src='https://github.com/harshalgadhe/DeepFake-Detection/blob/main/images/Screenshot%20(24).png'><br> 


