Source code for YMDK Melody 96 Pro (YMD96v3 PCB w/ underglow)

# Credits #

Thanks to TheDordo, HarD, and Naitoshedo @ [SignalRGB](https://www.signalrgb.com/) for creating this source enabling everyone with a capable keyboard to use QMK + SignalRGB together!

Thanks to Nick @ [YMDK] for providing the keyboard source code!

Thanks to Spartan/Bubbles for final troubleshooting, networking, instructions, and assembly!

### Help with this source ###

**Support can be provided either on the Github repository ([**Issues**](https://github.com/SRGBmods/QMK-Binaries/issues)) here or the QMK channels of this** [**Discord**](https://discord.com/invite/J5dwtcNhqC) **(Discord will be faster in most cases).**

**Please keep support requests to either of those locations only, thanks!**

**NOTE: this may change to provide greater stability under certain situations. this is still a work in progress though it will work for most scenarios**

**qmk_firmware holds all files necessary to allow for SignalRGB as well as 0.21.0 QMK. Keyboard source code is also in this folder under keyboards.**

**JSON updated to support VIA v3, Javascript file is custom plugin for SignalRGB. Please double check vendor and product ID using chrome://usb-**

### Installation Instructions ###

**1. Please delete any existing qmk_firmware folder first if not 0.21.0**

**2. Open QMK MSYS and type in "git clone --recurse-submodules https://github.com/qmk/qmk_firmware.git" (without quotes)**

**3. Drag and drop or copy/paste qmk_firmware from zip into C:\Users\{your user name}\qmk_firmware\**

**4. Open QMK MSYS again and type in "cd qmk_firmware/" (without quotes)**

**5. After the previous resolves, type in "qmk compile -kb ymdk/melody96rgb -km via" (without quotes)**

**6. If this does not compile, you will need to repeat steps 1 and 2. Stop there, DO NOT MOVE ON TO STEP 3. Please contact the dev team at SignalRGB (https://discord.gg/rukKkKpBJ6) for help in manually patching your firmware**

**7. If it does compile successfully, open QMK Toolbox and select the desired firmware file**

**8. Put your keyboard in DFU/Bootloader mode, if usual key shortcuts do not work there are 2 leads exposed by a hole in the bottom acrylic cover.**

**8a. Short these leads with something metal like tweezers and then plug it in. wait 1 or 2 seconds before removing and you should be in DFU mode. (ignore if you were able to enter DFU mode normally)**

**9. Click flash to flash firmware onto your keyboard.**

**10. All done! Now you must ensure the product and vendor IDs are correct on VIA JSON and SignalRGB JS.**

**The vID and pID may be different for your specific board.**

**Type in your web browser: "chrome://usb-internals" or "edge://usb-internals" (w/out quotes), depending on your chosen browser.**

**View your connected devices and note the ID numbers listed.**

**Replace the Product and Vendor ID (PID/VID) values with those listed ID numbers. If they are the same, you can ignore this step.**

**Save and reload the JSON into VIA.**

**Save and reload the JS into SignalRGB. You may need to restart the app completely or provide admin access**

**Set up your macros and keyboard layout in VIA, customize and synchronize the LEDs with SignalRGB, OpenRGB, or manual QMK code!**

**DUE TO STABILITY ISSUES: Please lower your brightness to 50% ESPECIALLY when using white LED effects. Too bright of a setting can result in keyboard crashing or plugin crashing due to power draw.**

**Exceeding 50% may work for your specific device or RGB setup, but requires testing on user's part**
