# Project Title: FreeRTOS Basic Task Output

## Introduction
This project implements a periodic task creation and execution structure using **FreeRTOS**. A single task is designed to output my student ID and name to the terminal every 1,000ms using the `vTaskDelay()` function. Through this implementation, I explored the core principles of **RTOS scheduling** and the process of **task state transitions** (Running to Blocked). 

## Environment
* **IDE**: Visual Studio 2022 
* **OS**: FreeRTOS Windows Simulator 

## Key Features
1. **Single Task Management**: Successfully initialized and registered a standalone task named `JUNTask` using the `xTaskCreate()` API. 
2. **Deterministic Periodic Logging**: Implemented a precise 1-second (1,000ms) output interval by combining `vTaskDelay()` with the `pdMS_TO_TICKS()` macro. 
3. **Safe Parameter Handling**: Prevented compiler warnings and ensured code stability by explicitly casting the unused `pvParameters` to `void`. 
4. **Minimalist System Configuration**: Streamlined the execution environment by enabling 'mainCREATE_SIMPLE_BLINKY_DEMO_ONLY', focusing strictly on the core task logic.
## Results
<img src="https://github.com/user-attachments/assets/16c0097d-b7bf-4400-84bf-0b3a8309ea99" width="667" />
**Logging**- 시스템의 동작 상태나 실시간 데이터를 기록하는 과정 ex) printf
