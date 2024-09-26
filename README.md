
# Lenovo Thinkpad L590

## Opencore Hackintosh

I'm creating this repository for those who might be trying to Hackintosh a computer that is similar to mine. I have reached what I beleive to a moderate level of stability with this EFI, and I am unlikely to update this repo until after the puclic release of MacOS 13.6.6 Ventura. Happy Hacking!

#### Hardware Config:

    1. Make and Model: Lenovo Thinkpad L590
    2. Processor and Chipset: Intel Core i7 8565U / Intel Whiskey series chipset
    3. Graphics: Intel UHD 620
    4. Monitor: 1920x1080p FHD
    5. Storage: SSD 256 GB no name
    6. RAM: 24 GB DDR4 2666
    7. 1 x PS/2 Trackpad + Trackpoint
    8. 1 x PS/2 Keyboard
    9. 2 x USB 3.0 type A ports
    10. 2 x USB 3.1 type C ports
    11. 1 x HDMI port
    12. 1 x 3.5mm mic/headphone jack
    13. Wifi + BlueTooth: Intel AC 9260 + I219-V


#### Currently functioning:
- All basic functions including sleep/wake and boot without error including iCloud Services
- Trackpoint and Trackpad with gesture support and Keypad buttons function as well
- USB type A ports with USB 3.0 and USB type C ports support
- HDMI output is perfect work with L590
#### Untested:
- Display port support because I was lazy, but i will update when i have a freetime
- Can use Boardcom to change for Thinkpad L590 Wifi card (For using Airdrop & Handoff)
- WWAN (No need for me)
- Smart Card Redear (No need for me)
#### Installation Instructions:
1. Please follow Dortania OpenCore Vanilla guide to create ACPI, gather Kexts, and create installer. I would recommend reading through the entire process even if you are going to just copy paste this repo into your EFI folder; it will give you the ability to debug and upgrade your OC install in the future.
2. For those of you with a different CPU please use the post-install guide on Power Management how to generate new "YourCustomCPU.kext".
3. To enable Apple services for you computer, you must fill in the Serial Number/ MLB/ SmUUID which are currently blank on the EFI Please refer to config.plist guide on OC configuration on how to properly generate this information for your hackintosh.
4. Find some help from Hackintosh community, expert person.
#### BIOS Settings

    1. Config
        - USB UEFI Bios Support -> Enabled
        - Keyboard Mouse
            + Trackpoint -> Enabled
            + Trackpad -> Enabled
        - Display
            + Total Graphics Memory -> 512 MB
            + Boot Time Extension -> Disabled
    2. Security
        - Fingerprint
            + Predesktop Auth -> Disabled
            + Security Mode -> Normal
        - Security Chip
            + TPM 2.0
            + Security Chip -> Disabled/All
        - Memory Protection -> Enabled
        - Virtualization
            + Intel Virtualization -> Enabled
            + Intel VT -d -> Disabled
        - I/O port access -> Enable All
        - Secure Boot -> Disabled
        - Intel SGX -> Disabled
        - Device Guard -> Disabled
    3. Startup
        - UEFI/Legacy -> UEFI only
        - CSM Support -> No

## Screenshots

![image](https://github.com/user-attachments/assets/f2ae41b1-bc6e-4614-9423-952e20797ded)




