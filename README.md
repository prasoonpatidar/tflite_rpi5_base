# TFLite Raspberry Pi zero 2w Base

A TensorFlow Lite image classification project for Raspberry Pi zero2w using the MobileNet V1 quantized model.

## Requirements

- Python 3.9+
- Raspberry Pi zero 2w (or compatible device)

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url> tflite_rpi0_2w_base
   cd tflite_rpi0_2w_base
   ```

2. Install dependencies using uv:
   ```bash
   uv sync
   ```

   Or using pip:
   ```bash
   pip install numpy==1.23.5 pillow tflite-runtime
   ```

## Usage

Run the image classification test:

```bash
python test_tflite.py
```

This will classify `test.jpg` using the MobileNet model and output the predicted label with confidence score.

## Project Structure

- `test_tflite.py` - Main classification script
- `main.py` - Entry point
- `mobilenet_v1_1.0_224_quant.tflite` - Quantized MobileNet model
- `labels_mobilenet_quant_v1_224.txt` - ImageNet class labels
- `test.jpg` - Sample test image
