# apt

APT repository for the Cyber CTF desktop launcher.

## Overview

A static Debian/Ubuntu package repository (`dists/` and `pool/`) with the signing key `cyberctf-apt.asc`. The landing page (`index.html`) lists the commands to add the repository and install the launcher. It is published at https://cyber-courses.github.io/apt.

## Getting started

Install on Debian or Ubuntu (amd64), as shown on the landing page:

```bash
curl -fsSL https://cyber-courses.github.io/apt/cyberctf-apt.asc | sudo gpg --dearmor -o /usr/share/keyrings/cyberctf.gpg
echo "deb [signed-by=/usr/share/keyrings/cyberctf.gpg] https://cyber-courses.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/cyberctf.list
sudo apt update
sudo apt install cyber-ctf
```
