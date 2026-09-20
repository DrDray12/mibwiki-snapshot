# Clean APG unit

\

:::warning
Never login to normal RCC and MMX. There are scripts and watchdogs running on the unit which will brick the unit.

:::


Log into [Emergency IFS](/doc/enter-rcc-blue-efu-emergency-ifs-u6Pt9h5acV) and [manually flash complete RCC, MMX + APP](/doc/manual-firmware-restore-NglgI1RK9n).

Full SDWL FW update is recommended after reboot to make sure that all components are up to date.



:::info
After firmware restore, is necessary to delete the FEC link (is a link to `/protect/FEC` that doesn't exist)

:::


 ![](attachments/fe3d1ad1-c90e-487a-a784-ddbd91c09779.png)for delete and restore

```bash
rm -rf /mnt/efs-persist/FEC
mkdir /mnt/efs-persist/FEC
```


After this you can patch with [M.I.B](/doc/mib-more-incredible-bash-CO492qmzLk)