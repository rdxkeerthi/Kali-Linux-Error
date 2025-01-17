# Kali-Linux-Error
Fix Kali Linux


# Fix initramfs when booting in Kali Linux


first Use 

``` blkid ```

![image](https://github.com/user-attachments/assets/a7ac7c52-9bad-4c10-a07b-164567187a86)
![image](https://github.com/user-attachments/assets/f26c4d8b-1ade-4707-bf29-a6c0525c56d8)


In my case the name of the partition is nvme0n1p2. Don’t forget to add the -y to avoid typing it multiple times. If you have multiple partitions ext2 or ext4 type you can run this for each one.

```fsck /dev/nvme0n1p2 -y```

![image](https://github.com/user-attachments/assets/9368c763-fde1-40f9-9f2e-80afcf2a33e7)


When it finishes you can just reboot and that will take you to the login screen as usual.

```reboot -f```

![image](https://github.com/user-attachments/assets/1e3fa928-2cd6-4f2a-b3d2-c31094e90ce3)
