# BitNetMCU
There's a growing buzz around large language models (LLMs) with "1 Bit" or "1.58 Bit" weight quantization of neural network weights, suggesting that with Quantization Aware Training (QAT), LLMs can maintain quality while drastically reducing memory requirements. This is particularly relevant for microcontrollers like CH32V003, known for their low cost and limited resources.

By leveraging low-bit quantization, memory requirements for storing weights are minimized, and inference operations can be simplified to additions, making it feasible to run neural networks on microcontrollers lacking hardware multipliers like CH32V003.

The challenge lies in developing a pipeline that optimizes both training and inference processes to achieve high accuracy within the constraints of the microcontroller's capabilities. This project aims to document and experiment with various approaches towards this goal using the MNIST dataset.

**Objective:**

The goal is to create a pipeline for training and inference of low-bit quantized neural networks suitable for running on a CH32V003 RISC-V microcontroller. Using the MNIST dataset, the aim is to achieve high test accuracy while leveraging the microcontroller's limited resources effectively.

**Required:**

- CH32V003X.
- Proficiency in developing and training neural networks.
- Knowledge of the MNIST dataset and its preprocessing.
- Ability to optimize inference for low-resource environments.

### VSD Squadron Mini Board Specifications

| Feature                      | Description                                                                                      |
|------------------------------|--------------------------------------------------------------------------------------------------|
| **Board**                    | VSDSquadron Mini                                                                                 |
| **Microcontroller**          | CH32V003F4U6 chip with 32-bit RISC-V core based on RV32EC instruction set                        |
| **USB connector**            | USB 2.0 Type-C                                                                                   |
| **Built-in LED Pin**         | 1x onboard user LED (PD6)                                                                        |
| **Digital I/O pins**         | 15x                                                                                              |
| **Analog I/O pins**          | 10-bit ADC, PD0-PD7, PA1, PA2, PC4                                                               |
| **PWM pins**                 | 14x                                                                                              |
| **External interrupts**      | 8 external interrupt edge detectors, mapped to any one of 18 external I/O ports                  |
| **USART**                    | 1x, PD6 (RX), PD5 (TX)                                                                           |
| **I2C**                      | 1x, PC1 (SDA), PC2 (SCL)                                                                         |
| **SPI**                      | 1x, PC5 (SCK), PC1 (NSS), PC6 (MOSI), PC7 (MISO)                                                 |
| **Programmer/Debugger**      | Onboard RISC-V programmer/debugger, USB to TTL serial port support                               |
| **I/O voltage**              | 3.3V                                                                                             |
| **Input voltage (nominal)**  | 5V                                                                                               |
| **Source Current per I/O Pin** | 8mA                                                                                            |
| **Sink Current per I/O Pin** | 8mA                                                                                              |
| **Clock speed**              | Processor: 24MHz                                                                                 |
| **Memory**                   | SRAM: 2kb on-chip volatile SRAM, 16kb external program memory                                    |



![image](https://github.com/princesuman2004/BitNetMCU/assets/128327318/b2db779d-715c-419e-82d6-fa8269d62f3b)

### Connections:
- A camera connected to the board to relay data.( For testing ,once the MNIST data has been tested)
- An LED Display to output the data.
- Power Connection.
  
![image](https://github.com/princesuman2004/BitNetMCU/assets/128327318/66a747e9-77bc-4df5-82db-ca1e9cb58949)


