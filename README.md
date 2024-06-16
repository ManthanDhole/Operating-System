Creating your own Operating System <br><br>
This code base for development of OS is being followed on as per demonstrated in the playlist by Viktor Engelmann
Link to playlist: https://www.youtube.com/playlist?list=PLHh55M_Kq4OApWScZyPl5HhgsTJS9MZ6M <br>
<br>
For the development setup you'll require the following packages: <br>
sudo apt install g++ <br>
sudo apt install binutils <br>
sudo apt install libc6-dev-i386 <br>
sudo apt install virtualbox <br>
sudo apt install grub-coreboot grub2-common:i386 grub-efi-amd64:i386 <br>
sudo apt  install xorriso <br>
sudo apt install mtools <br>

Create a VM using VirtualBox

![image](https://github.com/ManthanDhole/Operating-System/assets/85555944/162aad12-321a-4a4f-9d47-a9cc6e1c90b8)

![image](https://github.com/ManthanDhole/Operating-System/assets/85555944/091e7fd8-5f2c-4272-968e-ce1f7192c5bd)


Build the code using the following commands: <br>
make kernel.o <br>
make loader.o <br>
make kernel.bin <br>
make run <br>

This process will build the kernel.cpp and loader.s code files and merge them using the Linker to finally create a kernel.bin file which will be loaded with the system boots up.
Also we'll be creating an kernel.iso file and use that in the Virtual Box by setting it in the Storage section as follows:

![image](https://github.com/ManthanDhole/Operating-System/assets/85555944/33af3957-c07f-4bc7-8ac9-3bc95e9c5e10)

![image](https://github.com/ManthanDhole/Operating-System/assets/85555944/de2478bc-5478-4971-bcbc-04f5dc5da8e2)
