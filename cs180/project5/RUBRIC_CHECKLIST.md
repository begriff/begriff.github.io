# Project 5 Part A - Rubric Checklist

## Part 0: Setup
- [x] Come up with some interesting text prompts and generate their embeddings
- [x] Choose 3 of your prompts to generate images and display the caption and the output
- [x] Reflect on the quality of the outputs and their relationships to the text prompts
- [x] Make sure to try at least 2 different num_inference_steps values (mentioned in reflection)
- [x] Report the random seed (9001)

## Part 1.1: Implementing the Forward Process
- [x] Implement the noisy_im = forward(im, t) function (mentioned)
- [x] Show the Campanile at noise level [250, 500, 750] (all 3 shown)

## Part 1.2: Classical Denoising
- [x] For each of the 3 noisy Campanile images, show your best Gaussian-denoised version side by side (all 3 shown)

## Part 1.3: One-Step Denoising
- [x] For the 3 noisy images (t = [250, 500, 750]):
  - [x] Use forward function to add noise to Campanile
  - [x] Estimate the noise by passing through stage_1.unet
  - [x] Remove the noise to obtain estimate of original image
  - [x] Visualize original, noisy, and denoised images (all 3 timesteps shown)

## Part 1.4: Iterative Denoising
- [x] Using i_start = 10:
  - [x] Create strided_timesteps (mentioned)
  - [x] Complete the iterative_denoise function (mentioned)
  - [x] Show noisy Campanile every 5th loop of denoising (steps 5, 10, 15, 20, 25, 30, 35 shown)
  - [x] Show final predicted clean image using iterative denoising
  - [x] Show predicted clean image using only single denoising step
  - [x] Show predicted clean image using gaussian blurring

## Part 1.5: Diffusion Model Sampling
- [x] Show 5 sampled images (all 5 shown)

## Part 1.6: Classifier-Free Guidance (CFG)
- [x] Implement the iterative_denoise_cfg function (mentioned)
- [x] Show 5 images of "a high quality photo" with CFG scale of 7.5 (all 5 shown)

## Part 1.7: Image-to-image Translation
- [x] Edits of the Campanile image at noise levels [1, 3, 5, 7, 10, 20] with prompt "a high quality photo" (all shown)
- [x] Edits of 2 of your own test images (Big Sur and Zoo shown)

### Part 1.7.1: Editing Hand-Drawn and Web Images
- [x] 1 image from the web edited at noise levels [1, 3, 5, 7, 10, 20] (Big Sur shown)
- [x] 2 hand drawn images edited at noise levels [1, 3, 5, 7, 10, 20] (Horse and Water shown)

### Part 1.7.2: Inpainting
- [x] A properly implemented inpaint function (mentioned)
- [x] The Campanile inpainted (shown with mask and result)
- [x] 2 of your own images edited with masks (Minecraft and Statue shown)

### Part 1.7.3: Text-Conditional Image-to-image Translation
- [x] Edits of the Campanile using given prompt at noise levels [1, 3, 5, 7, 10, 20] (shown with "a rocket ship" prompt)
- [x] Edits of 2 of your own test images (Regshow and Road shown)

## Part 1.8: Visual Anagrams
- [x] Correctly implemented visual_anagrams function (mentioned)
- [x] 2 illusions that change appearance when flipped upside down (Bunny/Seal and Light/Canal shown)

## Part 1.9: Hybrid Images
- [x] Correctly implemented make_hybrids function (mentioned)
- [x] 2 hybrid images (Ear/Mouth and Old Man/Hamster shown)

## Summary
All required deliverables appear to be satisfied. The website includes:
- All required images and visualizations
- Proper organization matching the rubric structure
- Reflections and explanations where required
- All technical implementations mentioned

