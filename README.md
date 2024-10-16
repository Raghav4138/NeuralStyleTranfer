# Image Style Transfer with PyTorch

This project demonstrates an image style transfer pipeline using PyTorch. It allows for image transformation and processing using various libraries like `albumentations` and `PIL`.

## Features

- Dynamic GPU/CPU device selection for efficient computation.
- Image loading and transformation using `torchvision.transforms`.
- Style and content image loading for style transfer tasks.

## Requirements

- Python 3.x
- PyTorch
- Albumentations
- Pillow (PIL)
- TimM
- Matplotlib

To install the required packages, you can use the following:

```bash
pip install torch torchvision albumentations pillow timm matplotlib
```

## Usage

1. Set up the project and ensure all dependencies are installed.
2. Use the img_loader function to load and transform images for style transfer tasks
   ```bash
   img = img_loader("path_to_your_image.jpg")
   ```
3. Modify the image size dynamically based on the availability of GPU resources:
   ```bash
   img_size = 512 if torch.cuda.is_available() else 128
   ```
4. To execute the notebook, ensure you are using a Jupyter environment with CUDA support.

## Collaborations and Suggestions

I welcome any collaborations, suggestions, or improvements to the project. Feel free to open an issue or submit a pull request if you have ideas or feedback!
