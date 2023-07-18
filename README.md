# fetal_CP_segment_attention


Pretrained weights(*.h5) and deployed model(singularity image) are archived with the following drive.

https://drive.google.com/drive/folders/17QhKw-_kswtbMwBoYidAR4iMPXnQDCm_?usp=sharing


# Usage with deployed singularity image(sif)
singularity run --no-home -B {file_path}:/data --nv {path for sif image} {segmentation target filename} . 1;

# -B: path containing model input (recon_to31_nuc.nii), also designated path for output (recon_to31_nuc_deep_agg.nii.gz)
# . : path for output (linked to -B path by default)
# 1: Number of GPU to use
