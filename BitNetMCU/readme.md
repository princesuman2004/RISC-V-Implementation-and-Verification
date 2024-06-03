**Objective:**

The goal is to create a pipeline for training and inference of low-bit quantized neural networks suitable for running on a CH32V003 RISC-V microcontroller. Using the MNIST dataset, the aim is to achieve high test accuracy while leveraging the microcontroller's limited resources effectively.

**Required:**

- Understanding of Quantization Aware Training (QAT) techniques.
- Familiarity with the CH32V003 microcontroller specifications.
- Proficiency in developing and training neural networks.
- Knowledge of the MNIST dataset and its preprocessing.
- Ability to optimize inference for low-resource environments.

**Motivation:**

There's a growing buzz around large language models (LLMs) with "1 Bit" or "1.58 Bit" weight quantization, suggesting that with Quantization Aware Training (QAT), LLMs can maintain quality while drastically reducing memory requirements. This is particularly relevant for microcontrollers like CH32V003, known for their low cost and limited resources.

By leveraging low-bit quantization, memory requirements for storing weights are minimized, and inference operations can be simplified to additions, making it feasible to run neural networks on microcontrollers lacking hardware multipliers like CH32V003.

The challenge lies in developing a pipeline that optimizes both training and inference processes to achieve high accuracy within the constraints of the microcontroller's capabilities. This project aims to document and experiment with various approaches towards this goal using the MNIST dataset.
