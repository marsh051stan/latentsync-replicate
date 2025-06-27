# LatentSync - Lip Synchronization Model

This is a deployment of the LatentSync model on Replicate. LatentSync is a state-of-the-art lip synchronization model that can generate realistic lip movements synchronized with audio.

## Features

- High-quality lip synchronization
- Supports various video formats
- Configurable guidance scale and inference steps
- Automatic model download from HuggingFace

## Usage

The model takes:
- **video**: Input video file
- **audio**: Input audio file to synchronize with
- **guidance_scale**: Controls generation quality (1.0-3.0, default: 2.0)
- **inference_steps**: Number of denoising steps (20-50, default: 20)
- **seed**: Random seed (0 for random)

## Deployment

To deploy this model on Replicate:

1. Push your code to a GitHub repository
2. Connect the repository to Replicate
3. The model will automatically build using the `cog.yaml` configuration

## Model Details

- Base model: ByteDance/LatentSync-1.6 from HuggingFace
- Framework: PyTorch with Diffusers
- GPU Required: Yes (CUDA 12.1)
