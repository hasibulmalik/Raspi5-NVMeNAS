# Raspi5-NVMeNAS

Build your own Network Attached Storage (NAS) using a Raspberry Pi 5 and NVMe storage. This guide walks you through the setup process, from preparing your SD card to configuring OpenMediaVault (OMV) with ZFS for robust storage solutions.


![demo image 1](https://github.com/user-attachments/assets/8fd377a2-6375-4f0e-b592-596eb3e7a66c)
![demo image 2](https://github.com/user-attachments/assets/52c00685-dc85-4d49-afce-b058dc8a13c1)


---

## Requirements
- Raspberry Pi 5
- SD card (16GB or 32GB recommended)
- NVMe storage device
- A computer for initial setup

  
### Phase 1: Setting Up the Raspberry Pi

Step 1: SD Card:-

1. Format the SD card using a tool like `Balena Etcher` or `Raspberry Pi Imager`.
2. Ensure the card is clean and has no residual partitions.


![1  SD Card](https://github.com/user-attachments/assets/795ed649-2ff8-4405-88e8-da824ba62169)


Step 2: Raspi Downloader:-

1. Download the Raspberry Pi Imager tool from [Raspberry Pi's website](https://www.raspberrypi.com/software/).
2. Use the tool to install the Raspberry Pi OS on your SD card.

![2  Raspi Downloader](https://github.com/user-attachments/assets/82baf798-5410-4ebd-9b96-063fcd50ad6e)

Step 3: Raspi OS:-

1. In the Raspberry Pi Imager, select the operating system you prefer (My personal preference: Raspberry Pi OS Lite for headless setups).
2. Configure network and SSH settings during this step if available.

![3   Raspi OS](https://github.com/user-attachments/assets/da7a8aed-96b9-4083-adf9-90cdc76649d3)


Step 4: OS Customization-

1. Enter advanced options to configure SSH, Wi-Fi credentials, and hostname.
2. Save these settings to the SD card.
   
![4  OS Customization](https://github.com/user-attachments/assets/cd5fe361-70c0-492c-9347-48b8252b0d32)

Step 5: OS Customization Config-

1. set up HOSTname, HOSTusername, HOSTpassword. In my case I names raspi-nas as HOST name. HOSTusername as home and HOSTpassword I won't tell you ;)

![5  OS Customization Config](https://github.com/user-attachments/assets/f0b841d8-5d4a-43d8-946c-74669134184a)



Step 6: Erase Confirmation-

1. Confirm the erasure of existing data on the SD card.

![6  Erase Confirmation](https://github.com/user-attachments/assets/f4769c0f-1d9d-40d5-91bb-e79b348281c5)


Step 7: Preparing Erasing-

1. Wait for the flashing process to complete.
   
![7  Preparing Erasing](https://github.com/user-attachments/assets/2055b748-a680-404a-9a47-8fc19aa27022)

Step 8: Successful boot-

![8  Successful boot](https://github.com/user-attachments/assets/c740e7fe-12d2-46d4-aeb2-f6a036269490)

### Phase 2: Installing and Configuring OpenMediaVault (OMV)

Step 9: OVM after install-

1. Boot your Raspberry Pi with the prepared SD card.
2. Install OpenMediaVault using the [official guide](https://www.openmediavault.org/).

![9  OVM after install](https://github.com/user-attachments/assets/37dfefe6-b977-4db4-be84-bf1f04281749)


Step 10: OVM install final-

![10  OVM install final](https://github.com/user-attachments/assets/5e7db4f5-efe4-4571-bf44-6f11b255ce26)


Step 11: login page omv-

![11  login page omv](https://github.com/user-attachments/assets/14c41eb3-ab8d-47d8-a60b-921981b5dfd7)

Step 12: OMV Homepage-

![12  OMV Homepage](https://github.com/user-attachments/assets/73fdb284-1a41-4ecc-9336-b420834e1516)

Step 13: ZFS plugin search-

1. Search for the ZFS plugin in the OMV interface.

![13  zfs plugin search](https://github.com/user-attachments/assets/2353e632-78e2-4381-b670-1ac9cecc5a22)

Step 14: ZFS download-

1. Download and install the plugin.
   
![14  zfs download](https://github.com/user-attachments/assets/6016dbbe-7a6d-4455-9e04-204c157006c0)

Step 15: ZFS download done-

![15 zfs download done](https://github.com/user-attachments/assets/6420863f-2986-46f1-97a7-061e03434172)

Step 16: ovm update done-

![16  ovm update done](https://github.com/user-attachments/assets/16a8af00-9715-4a40-8404-580d297bb18a)

Step 17: ZFS pool-

![17  zfs pool](https://github.com/user-attachments/assets/d0751a42-2f34-4980-beb4-97c444daaa4b)

Step 18: ZFS add pool-

![18  zfs add pool](https://github.com/user-attachments/assets/41224d7e-1ca5-4b8a-9359-01d73a71b9d3)


Step 19: create pool-

![19  create pool](https://github.com/user-attachments/assets/24a5a152-f41a-4df5-818f-d530c3a91deb)

Step 20: shared folder create-

![20  shared folder create](https://github.com/user-attachments/assets/eac005fa-2137-4388-a86c-fa1ad06d5798)

Step 21: ssh enabled-

![21  ssh enabled](https://github.com/user-attachments/assets/fc2110c7-1bfc-4965-8661-cf4061edc37d)








