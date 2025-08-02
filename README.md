# Firmware-OpenWRTInvasion-Xiaomi-Mi-4A-R4AC-NO-Internazional-
The OpenWRTInvasion firmware for Xiaomi Mi 4A R4AC (No International) is based on OpenWRT 23.05.05 and is needed because the official OpenWRTInvasion GitHub repository lacks firmware for this model. It ensures compatibility, optimization, and the use of the latest OpenWRT features.

**Description:**

The **OpenWRTInvasion firmware for Xiaomi Mi 4A R4AC (No International)** is a custom version based on OpenWRT 23.05.05, specifically created for the **R4AC** model. This version is necessary because the official **OpenWRTInvasion** GitHub repository lacks the specific firmware for this model in the firmware folder. Therefore, the custom OpenWRTInvasion version for the **Mi 4A R4AC** ensures proper functionality and performance optimization, supporting the latest features and improvements of **OpenWRT 23.05.05**. It is an essential solution for those who wish to install OpenWRT on this router without compatibility issues.

**Installation:**
https://github.com/acecilia/OpenWRTInvasion.git


cd /tmp

wget http://github.com/ilblogdicristiangallo/Firmware-OpenWRTInvasion-Xiaomi-Mi-4A-R4AC-NO-Internazional-/blob/main/openwrt-23.05.5-ramips-mt76x8-xiaomi_mi-router-4a-100m-squashfs-sysupgrade.bin # Put here the URL you want to use to download the firmware

./busybox sha256sum openwrt-23.05.5-ramips-mt76x8-xiaomi_mi-router-4a-100m-squashfs-sysupgrade.bin # Verify the firmware checksum before flashing, very important to avoid bricking your device!

mtd -e OS1 -r write openwrt-23.05.5-ramips-mt76x8-xiaomi_mi-router-4a-100m-squashfs-sysupgrade.bin OS1 # Install OpenWrt
