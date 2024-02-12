# Stable Diffusion Custom Dream booth Inpainting Model

# Steps to Reproduce the results

### 1. Install necesssary libraries mentioned in 01_Dream_Booth_Dog_model_training.ipynb and follow the notebook to train dream booth model for the specific dog. Note For the specific dog instance dataset, use the images curated in the dataset Dataset\Specific_Dog_Images_dataset folder for training.

# 2. The image dataset I made for that specific dog are as shown below (just used image outpainting and background change to create a variety) :

<table>
  <tr>
    <td><img src="Dataset\Specific_Dog_Images_dataset\close-up-portrait-of-dog-royalty-free-image-1577697658-Photoroom.jpg" width="400" /></td>
    <td><img src="Dataset\Specific_Dog_Images_dataset\close-up-portrait-of-dog-royalty-free-image-1577697658.jpg" width="400" /></td>
  </tr>
  <tr>
    <td><img src="Dataset\Specific_Dog_Images_dataset\getimg_ai-2024-02-12T09_44_31-Photoroom.jpg" width="400" /></td>
    <td><img src="Dataset\Specific_Dog_Images_dataset\getimg_ai-2024-02-12T09_44_31.317Z.png" width="400" /></td>
  </tr>
</table>
<h2>Images in the dataset.</h2>

# 3. Download these 3 models from the urls given below  : One custom dream booth model + 1 in painting and one stable diffusion model:

In Painting Model : https://huggingface.co/runwayml/stable-diffusion-inpainting/resolve/main/sd-v1-5-inpainting.ckpt?download=true <br>
Stable Diffusion 1.5 model : https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt?download=true <br>
Custom Dream booth Dog model : https://drive.google.com/file/d/1EEAb9r0oVJ_FyQ550F5AdiP8-BZHItmr/view?usp=sharing <br>
 
# 3. Now Start the Comfy UI workflow with final_workflow.json as shown below:

<img src="workflow_image.png" width="750" />

<figcaption ><h2>This ComfyUI workflow combines 3 models mentioned above to create an inpainting dreambooth model of the dog</h2></figcaption>


# 4. Results of Dreambooth in painting of the dog:

<img src="Input_maksed_image_for_inpainting.png" width="400" />
<figcaption ><h2>Input Masked image of a beach</h2></figcaption>
<br>


<table>
  <tr>
    <td><img src="Output_image.png" width="400" /></td>
    <td><img src="ComfyUI_00100_.png" width="400" /></td>
  </tr>
</table>
<figcaption ><h2>Generated outptus</h2></figcaption>