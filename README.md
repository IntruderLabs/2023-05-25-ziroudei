# IntruderLabs ZirouDei Project
Date: 2023-05-25

Discoverer: Alan Lacerda (ifundef)

Exploit Coder: Alan Lacerda (ifundef) | Yueslly Lisbooa (0xC4CTU$)

## Vulnerability
Mk-Auth Remote Command Execution (RCE) via Unrestricted Upload

## Product Description
Mk-Auth is a Brazilian Management System for Internet Service Providers used to control client access and permissions via a web interface panel.

## Vulnerability Description
It is possible to upload a crafted .htaccess files to the Virtual Disk. This vulnerability may be used to gain Remote Command Execution to the server.

## Additional Information:
The application does not allow .php files to be uploaded but, by sending a crafted .htaccess an attacker may instruct the server to use php interpreter to any other file extention (even a random one like *.labs).

## Vulnerability Type:
CWE-434: Unrestricted Upload of File with Dangerous Type

## Vendor:
Mk-Auth

## Affected Product:
MK-Auth <= 23.01K4.9

## Affected Component:
Virtual Disk

## Attack Vector:
Remote

## Code Execution:
Yes

## Attack Vector:
Any client of the Internet Service Provider that has access to the platform (to download billings and request for support) and has the Virtual Disk feature, may exploit this vulnerability.

## Reference:
http://mk-auth.com.br/
