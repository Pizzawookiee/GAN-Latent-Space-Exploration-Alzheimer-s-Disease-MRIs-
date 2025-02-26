# GAN-Latent-Space-Exploration-Alzheimer-s-Disease-MRIs-
Contains graphics and other relevant resources.

Try it yourself!
1) Clone the StyleGAN2 repo and follow their instructions to set up the appropriate Python environment: https://github.com/NVlabs/stylegan2-ada-pytorch
2) Download pre-trained weights here: https://drive.google.com/file/d/1e8HHqbKazC_h4Jt_5Guo5HMwiUpMJF7w/view?usp=sharing
3) You will need an MRI scan(s) in your posession. Some resources include ADNI (https://adni.loni.usc.edu/) and OASIS3 (https://sites.wustl.edu/oasisbrains/); you will have to apply for access. I processed my scans in Freesurfer using recon-all and mri_vol2vol functions, then extracted coronal slices that contained the hippocampus.
4) Follow the instructions in the 'Projecting image to latent space' section of StyleGAN2 README using the coronal slices from (3). Use the path to the pre-trained weights for --network argument. 
5) Use image similarity metric of your choice to compare your original and projected image. ssim.py in this repo is the script that I used.

