# FFT Algorithm Analysis

This project presents a comparative analysis of Fast Fourier Transform (FFT) techniques, focusing on their computational efficiency and scalability. The study explores the theoretical and practical aspects of different FFT approaches and benchmarks their performance using a range of input sizes. FFT is a foundational algorithm in signal processing, with broad applications in fields like audio processing, image analysis, and data compression.

The accompanying report evaluates three main variants:

* **Recursive FFT** using the Cooley-Tukey divide-and-conquer strategy
* **Iterative FFT** with an in-place bottom-up design
* **FFTW3 Library** as an industry-standard, hardware-optimized baseline

## 📊 Results & Observations

* **Recursive FFT** provides clarity in structure but scales poorly with input size due to recursive overhead.
* **Iterative FFT** performs significantly better for large inputs, offering a good balance between speed and simplicity.
* **FFTW3** consistently outperforms both custom methods, achieving the lowest execution times thanks to cache-aware and SIMD-based optimizations.

The benchmarking results demonstrate that while custom implementations help in understanding FFT mechanics, production-grade applications benefit most from using mature, optimized libraries like FFTW.
