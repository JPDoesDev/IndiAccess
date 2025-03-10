# IndiAccess - A Computer Vision Model for Text-to-Speech Functionality for Visually Impaired Accessibility

## Overview:
**IndiAccess** is a computer vision model that uses a YOLOv8 model trained on images captured from the video game "Indiana Jones and the Great Circle". The game currently lacks built-in screen reader functionality and does not work well with Windows' built-in screen magnifier software, making it difficult for visually impaired players to enjoy the game.

## Installation/Setup Instructions:
This script requires Python and was created using version 3.9. Newer versions may cause dependency module errors, resulting in the program not functioning. NVIDIA CUDA technology is used by default and is required for proper performance. While CPU operation is possible, it results in poor performance.

### Prerequisite Installation:
1. Install Python 3.9 from the [python.org website](https://www.python.org/downloads/release/python-390/)
2. Install NVIDIA CUDA 12.4 runtime via: [CUDA 12.4 Download](https://developer.nvidia.com/cuda-12-4-0-download-archive)

### Virtual Environment Setup (optional):
1. In a Windows Command Prompt, navigate to the root "IndiAccess" folder.
2. Create a virtual environment by running the following command:
    ```sh
    py -3.9 -m venv .venv
    ```
3. Activate the created virtual environment by running the following command:
    ```sh
    .\.venv\Scripts\activate
    ```
4. Update pip and install ultralytics using pip by running:
    ```sh
    pip install --upgrade pip
    pip install ultralytics
    ```
5. The included version of torch and torchvision may be incorrect and will need to be uninstalled first by running this command:
    ```sh
    pip uninstall torch torchvision
    ```
6. Install an appropriate version of torch using the command generated by [PyTorch.org](https://pytorch.org/):
    ```sh
    pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
    ```
7. Install the remaining Python modules with the following command:
    ```sh
    pip install pyfiglet keyboard easyocr pyttsx3
    ```
8. Run `IndiAccess.py`. The first run will take a short time to initialize, but subsequent runs will be faster.

### Change Log:
- **v0.1**: Initial functionality and commit.


## Resources
- **GitHub**: [IndiAccess](https://github.com/JPDoesDev/IndiAccess)
