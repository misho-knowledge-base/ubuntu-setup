# USB mount fix
Fix for error `wrong fs type, bad option, bad superblock on /dev/sdb1, missing codepage or helper program, or other error` on opening mounted USB drive with NTFS in Ubuntu 24.04.

# Steps to fix
1. Install the necessary tools:
```bash
sudo apt update
sudo apt install ntfs-3g
```
2. Get the UUID of the drive:
```bash
sudo blkid /dev/sdb1
```
3. Edit the `/etc/fstab` file:
Add this at the end:
```bash
UUID=XXXX-YYYY /media/$USER/Data ntfs-3g noauto,x-systemd.automount,uid=1000,gid=1000,dmask=022,fmask=133 0 0
```
4. Create the mount point:
```bash
sudo mkdir -p /media/$USER/Data
```
