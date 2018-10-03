This is a modified rtl8188 driver source for getting the TL-WN722 USB Antenna to work on the TK1

TL-WN722N Antenna and rtl8188 Driver Setup
        1. Copy custom driver zip from https://github.com/Falimonda/custom_rtl8188 to Downloads and unzip
        2. Copy linux-grinch-21.3.4 to /usr/src (find source online or from thumb drive in the lab)
        3. sudo chmod 755 -R on linux-grinch-21.3.4 to enable execution of binaries
        4. go to unzipped driver folder
        5. make clean
        6. sudo make all ARCH=arm #you might have to 'sudo date MMDDHHSSYYYY.00' to avoid clock skew errors
        7. sudo make install
        8. TL-WN722N should work after reboot
