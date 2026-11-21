# CUDA-Accelerated Batch Image Processing Using GPU Parallel Computing

## Project Overview

This project demonstrates the use of NVIDIA CUDA for GPU-accelerated image processing. It processes multiple images using parallel computing techniques to improve processing efficiency.

Traditional CPU-based image processing handles operations sequentially or with limited parallelism. In this project, CUDA distributes image processing tasks across multiple GPU threads, allowing many pixels to be processed simultaneously.

## Objectives

- Understand GPU parallel computing using NVIDIA CUDA.
- Process multiple images using GPU acceleration.
- Implement image processing operations using CUDA kernels.
- Learn CUDA memory allocation and data transfer.
- Compare CPU and GPU processing performance.

## Technologies Used

- C++
- NVIDIA CUDA
- NVIDIA GPU
- CUDA Runtime API
- OpenCV (for image input/output, if used)
- Makefile

## Image Processing Operations

### 1. Grayscale Conversion
Converts color images into grayscale images by calculating intensity values from RGB pixel components.

### 2. Gaussian Blur
Applies a Gaussian filter to reduce image noise and smooth image details.

## Project Structure

```text
CUDA-Batch-Image-Processing/
│
├── README.md
├── Makefile
├── main.cu
├── image_processing.cu
├── image_processing.h
│
├── input/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── image3.jpg
│
├── output/
│
└── results/
    └── execution_log.txt
```

## How It Works

1. Load multiple input images.
2. Allocate memory for image data.
3. Transfer image data from CPU memory to GPU memory.
4. Execute CUDA kernels for parallel image processing.
5. Transfer processed data back to CPU memory.
6. Save the processed images.
7. Display execution information.

## Compilation

Compile the CUDA program using:

```bash
make
```

## Execution

Run the program using:

```bash
./image_processing
```

If command-line arguments are implemented, an example is:

```bash
./image_processing input/ output/
```

## Expected Output

The program processes multiple input images and generates processed output images.

Expected results include:
- Grayscale images.
- Gaussian-blurred images.
- Number of images processed.
- GPU execution time.

## Learning Outcomes

Through this project, I gained practical knowledge of CUDA programming, GPU memory management, parallel execution, thread indexing, and image processing. I also learned how GPU acceleration can help process large datasets efficiently.

## Author

Lakshanya N

## Project Type

CUDA at Scale for the Enterprise – Independent Project

