---
created: 2024-06-09T20:45:49-04:00
modified: 2024-06-09T20:52:09-04:00
---

# SMB-macos-optimizations-atto-tbolt-gigabit

Pagers of detailed tweaks to speed up SMB shares on macos (SMB-macos-optimizations-atto-tbolt-gigabit) are in dell powerscale-nas pdf titled "PowerScale OneFS: macOS Client Performance and User Experience Optimization June 2023 H17613.3"

https://www.delltechnologies.com/asset/en-us/products/storage/industry-market/h17613-wp-powerscale-mac-os-performance-optimization.pdf

Note: has dead link on page 22... correct link to atto techbulletin below:

▪ This ATTO technical bulletin shows which Thunderbolt ports to use on various types of Apple hardware to avoid disconnects and performance issues:

https://www.atto.com/wp-content/uploads/WebCollateral/tech-bulletin/ATTO_ThunderLink_Technical_Bulletin.pdf

TL/DR: The physical port on the mac that you connect tbolt-ethernet adapter must be on "Thunderbolt Route String 1". The pdf has photos identifying the port to use for 2016-2019 macs. Not sure if known-issue is resolved on newer macs, but pdf says how to verify:

To verify if the ATTO product (or other tbolt-ethernet adapter) is connected to a Thunderbolt Route String 1 port:
  * Go to the macOS System Information
  * Select Thunderbolt
  * Select the Thunderbolt Bus that the ATTO product is attached to.
  * Look under the “ThunderLink” in question and look for “Route String”. (There is a screenshot in the pdf linked above).
