# kaggle_competiton_img2prompt

Create Prompt

```
prompts = []

images_path = "../input/stable-diffusion-image-to-prompts/images/"
for image_name in images:
    img = Image.open(images_path + image_name).convert("RGB")
    
    
    generated = interrogate_classic(img)
    
    
    prompts.append(generated)
