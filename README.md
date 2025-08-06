# First DevSecOps Project: Secure V-Server Setup

This repository documents my very first DevSecOps project, completed during my training with the Developer Akademie.  
The project involved setting up and securing a virtual server (V-Server) and hosting a simple alternative website using **Nginx**.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Server Information](#server-information)
3. [Steps and Implementation](#steps-and-implementation)
    - [1. SSH Key Authentication Setup](#1-ssh-key-authentication-setup)
    - [2. Nginx Installation and Alternative Website Hosting](#2-nginx-installation-and-alternative-website-hosting)
4. [Security Considerations](#security-considerations)
5. [Conclusion](#conclusion)

---

## Project Overview
The goal of this project was to:
- Set up a secure remote connection to the server using **SSH keys**.
- Disable password authentication to reduce brute-force attack risks.
- Install and configure **Nginx** to host a basic alternative website on a non-standard port.

---

## Server Information
- **IP Address:** `159.69.106.42`
- **Operating System:** Ubuntu Server
- **Web Server:** Nginx

---

## Steps and Implementation

### 1. SSH Key Authentication Setup
1. **Generate an SSH key pair (ED25519 format):**
   ```bash
   ssh-keygen -t ed25519
2. **Copy the public key to the server:**
   ```bash
   ssh-copy-id -i ed25519KEY.pub USER@159.69.106.42


### 2. Nginx Installation and Alternative Website Hosting
