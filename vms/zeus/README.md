# Zeus

Zeus is a medium difficulty, boot-to-root Linux VM. The goal is to gain root access and read `user.txt` and `root.txt`. The release was published on 20 April 2019 and was tested on VMware.

## Download

Get the VM from the [Zeus VulnHub release page](https://www.vulnhub.com/entry/zeus-1,304/). VulnHub lists two archives:

| File | Listed size | MD5 | SHA1 |
| --- | --- | --- | --- |
| `zeus-ovf.zip` | 1.4 GB | `35871511556871F51C91955B6ADE32C6` | `ED9C4AEA7862AE153E039ED579182B14B9C98FD6` |
| `zeus.zip` | 1.3 GB | `23900947E76E0D328047CD6CE1008E35` | `33A77BADC4537FAF5FB2CFCF28EE1710989C4DDD` |

Verify the checksum of the archive you download against the value listed on VulnHub before importing it. Download links and availability may change; use the release page for the current mirrors.

## Network setup

The VM has DHCP disabled and uses the static IP address `192.168.131.170`. Place your lab machine on an isolated network that can reach that address. If you use the same subnet, an example lab address is `192.168.131.10/24`; ensure it does not conflict with another device.

Keep the VM off networks that contain devices you do not intend to expose to a deliberately vulnerable machine. The release page lists the image format as a VirtualBox OVA and notes that it was tested on VMware; choose the archive and import method that match your hypervisor.

## Objective

Gain root access and find both flags: `user.txt` and `root.txt`. This page contains no solution spoilers.
