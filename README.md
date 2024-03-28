# Fourier Transform-Based Image Denoising Project

## Overview
This project focuses on the development and evaluation of an image denoising algorithm as part of CSC3831. Drawing inspiration from current literature and incorporating Fourier Transform techniques, this work aims to effectively reduce noise in images while preserving critical details like edges and textures. The project assesses various denoising methods against a set of images with differing noise levels, utilizing quantitative metrics and visual analysis for evaluation.

## Introduction
Image denoising is essential across numerous applications, from enhancing medical imaging for better diagnosis to improving astronomical images for clearer celestial body visualization. This project's goal is to explore and implement an effective denoising algorithm that balances noise reduction with the preservation of image integrity.

## Literature Review
Key references that guided the development of this project include:
- Richard Wenzhe Xu's exploration of Fourier Transform in denoising,
- Naveen S. and Aiswarya V. A.'s work on Fourier Block Processing and Wiener Filtering,
- Navarro and Molimard's study on Directional Denoising using Fourier Spectrum Cloning.

These studies provide a foundational understanding and innovative approaches to image denoising, influencing this project's methodology.

## Methodology
### Algorithm Development
- **Fourier Transform-based Wiener Filter**: Utilizes the Fourier Transform to isolate and reduce noise in the frequency domain, preserving main image features.
- **Comparative Analysis**: Benchmarks against mean and median filters, and VisuShrink wavelet denoising, for a comprehensive evaluation.

### Preprocessing Steps
- **Image Normalization**: Standardizes pixel intensity values across images.
- **Gaussian Blur**: Applied as an initial noise reduction step to mitigate high-frequency noise components.

### Evaluation Metrics
- **Mean Squared Error (MSE)**: Quantifies the deviation from the original image, aiming for lower values.
- **Structural Similarity Index (SSIM)**: Assesses similarity in terms of luminance, contrast, and structure, with higher values indicating better performance.

## Results
The denoising algorithm's performance is detailed through MSE and SSIM metrics across various noise levels (`Noisy10`, `Noisy25`, `Noisy50`), revealing its effectiveness in low to moderate noise environments and challenges at higher noise levels. Visual comparisons and statistical analysis highlight the algorithm's strengths and areas for improvement.

## Key Findings
- The algorithm demonstrates robust noise reduction capabilities at lower noise levels, effectively maintaining image detail.
- Performance diminishes at higher noise levels, indicating the need for further optimization to balance noise reduction with detail preservation.
- Comparative analysis underscores the algorithm's versatility and potential applicability in diverse scenarios.

## Conclusions
This project showcases a promising approach to image denoising, particularly effective in low to moderate noise conditions. Future work will explore advanced techniques to enhance performance across all noise levels, expanding the algorithm's application scope.

## Running the Project
Ensure all dependencies are installed, and execute the provided Jupyter Notebook (`Part3.ipynb`) to replicate the analysis and observe the denoising effects across the dataset.

## Acknowledgments
- Special thanks to the CSC3831 course team for their guidance and the Berkeley Segmentation Dataset and Benchmark for providing the images.
- This project was influenced by contributions from Richard Wenzhe Xu, Naveen S., Aiswarya V. A., Navarro, and Molimard, whose works provided invaluable insights into effective denoising strategies.

## References
Please refer to the `Part3.pdf` for a detailed list of references and methodologies.

