# 1. Download Fedora
- Go to https://getfedora.org
- Download Fedora Workstation ISO

# 2. Create bootable USB (on Windows)
- Insert USB (≥8GB)
- Use Rufus:
  - Select Fedora ISO
  - Partition scheme: GPT
  - Target: UEFI
  - Start

# 3. Prepare BIOS/UEFI
- Reboot
- Press F2/F10/F12/Del (depends on laptop)
- Disable Secure Boot if needed
- Set USB drive first in Boot Order
- Save and reboot

# 4. Boot Fedora Live
- Select "Try Fedora" → then "Install to Hard Drive"

# 5. Installation setup
- Language: English
- Keyboard: US (or your choice)
- Timezone: Africa/Porto-Novo (adjust for location)

# 6. Disk setup
- Choose your main SSD
- Select "Erase Disk" (if full switch from Windows)
- Confirm

# 7. Install system
- Set full name: Caleb
- Username: calebelie
- Password: ********
- Root password optional

# 8. Reboot after installation
- Remove USB
- Fedora boots directly

# 9. First terminal setup
sudo dnf update -y
sudo dnf install git -y
sudo dnf install gcc make -y
sudo dnf install gnome-tweaks -y
sudo dnf groupinstall "Development Tools" -y

# 10. Optional
sudo dnf install neofetch htop vim -y
