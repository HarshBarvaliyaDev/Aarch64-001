
# Operating System for Aarch64(ARM64)

This project is for my learning purpose

In this project I am going to write a kernel for ARM Cortex-a72 from scratch




## Roadmap

- Writing Boot Script which will load the kernel to Ram

- Receiving data from Raspberry pi 4

- ARM 64 Fundamentals

- Memory Management 

- File System

- Process



## Acknowledgements

 - [Udemy](https://www.udemy.com/course/raspberry-pi-write-your-own-operating-system-step-by-step/learn/lecture/24008854?start=390#overview)



## Feedback

If you have any feedback, please reach out to me at harsh.barvaliya01@gmail.com


## Run Locally

Run below commands to install prerequisites (Ubuntu or WSL)

1) Install compiler for aarch64.

```bash
  sudo apt install gcc-aarch64-linux-gnu
```
check if it is installed correctly by

```bash
  aarch64-linux-gnu-gcc -v
```
if above command shows version correctly then it is installed correctly

2) Install QEMU
```bash
  sudo apt install qemu-system-arm
```
check if QEMU is installed run:
```bash
  qemu-system-aarch64
```
if the above command shows "machine not specified" then it is installed correctly

3) Clone the project

```bash
  git clone https://github.com/HarshBarvaliyaDev/Aarch64-001.git
  cd Aarch64-001
```
4) build the project and run it
```bash
  chmod +x build.sh
  ./build.sh
  qemu-system-aarch64 -M raspi4 -serial stdio -kernel kernel8.img
```
