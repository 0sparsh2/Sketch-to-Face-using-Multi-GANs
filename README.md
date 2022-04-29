# Sketch-to-Face-using-Multi-GANs

The project involves converting a sketch image to a real life face like image using a series of GANs (Generative Adversarial Network) models. 
Contextual GANs, GFPGANs and DeOldify were used to implement our model which was hosted over Anvil server. 

## Steps to implement : 

### Step 1

Train the model for Contextual GANs and save them. 
For the code of training the model, you can refer to this link [Sketch to Face Code](https://github.com/Malikanhar/Face-Sketch-to-Image-Generation-using-GAN/blob/master/Predict%20Image.ipynb). The code doesn't support Python 3.10 so I have made changes and uploaded the updated Python files in the current repository for referral. 

### Step 2

Once the model is trained, save it in an H5 file as per the code. The training takes months over a CPU so it's suggested to use GPUs or TPUs to train. 
Save the H5 file over your google drive which you can refer to your colab notebook.

### Step 3

Fire up the [colab notebook](Sketch_To_Face_Using_Multi_GANs.ipynb). Run all imports and installations including accessing h5 model from google drive.

### Step 4

Alterations in the notebook. gfpgan_inference.py file present in the GFPGANs folder after github pull command needs to be edited. The replacement of the specific code is provided towards the end in the colab notebook. 

### Step 5

Open Anvil. Link to colab notebook . Tutorial link which helped me - [Sample Anvil article](https://anvil.works/learn/tutorials/deepnote-to-web-app). 
You can also refer to the [official documentations](https://anvil.works/docs/overview) . 

<br />
## Layers of Processing: </br>

![f-042-01-sz1](https://user-images.githubusercontent.com/50074241/165392007-a899b570-127c-4158-a1dc-2b3e488998d5.jpg)
![Screenshot 2022-04-27 at 2 19 16 AM](https://user-images.githubusercontent.com/50074241/165392042-93ffca27-dceb-4ca6-ae99-2c04d9942f0b.png)
![Screenshot 2022-04-27 at 2 37 33 AM](https://user-images.githubusercontent.com/50074241/165392609-4aa9aece-9251-4450-a5d8-12e3873bdb6d.png)
![Screenshot 2022-04-27 at 2 43 04 AM](https://user-images.githubusercontent.com/50074241/165393483-cb4b8b28-5b61-4bb9-aa0f-728ecc40f132.png)

Actual Face: <br />
![f-042-01](https://user-images.githubusercontent.com/50074241/165392077-2afc0b5d-d3f4-40ce-98bb-f3a639334e5f.jpg)

## Evaluation

We used two metrics in our method of multigan. </br>
*Structural Similarity Index Measure* and *L2-Normalization score* 

### Structural Similarity Index Measure : 0.7804028372700662
### L2-Normalization Score :  93.7520664666667
