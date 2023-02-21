# Kiwi Ubuntu Builder
How to use Kiwi to create a customized Ubuntu installation ISO

To create a custom ISO installation of Ubuntu you also have to use Ubuntu to create it. For simplicity, you can also use Ubuntu WSL on Windows.

These are the steps:

    apt update
    apt install -y python3-pip debootstrap qemu-utils mtools xorriso
    pip3 install kiwi
    cd Kiwi
    kiwi-ng --profile Disk --type oem system build --description ubuntu --target-dir /home/iso

Now you can get your Ubuntu ISO file in /home/iso
