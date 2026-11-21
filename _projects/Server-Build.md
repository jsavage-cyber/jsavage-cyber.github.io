---
layout: project
title: "My Home Server Build"
description: "My journey in server building"
tags: [Computing, Hardware, Self-Hosting, Minecraft-Server-Hosting]
---

## Overview

One of my personal projects has been building and configuring my own home server. The original idea was relatively simple: build a machine that I could use to learn more about Linux, networking and server administration while also hosting some of my own services.

Rather than relying on third-party hosting providers for everything, I wanted to experiment with running my own infrastructure and understanding what happens behind the scenes.

What started as a small home server project has gradually developed into a machine capable of hosting Minecraft servers, managing Docker containers and providing a foundation for future projects.

## My Specification

| Component | Specification | Reason for Choosing |
|---|---|---|
| CPU | AMD Ryzen 7 5700X | 8 cores and 16 threads provide sufficient processing power to run multiple services and Minecraft servers simultaneously. |
| Motherboard | Gigabyte B550M K | An affordable AM4 motherboard with the essential connectivity and expansion options needed for a home server. |
| Memory | 32GB DDR4 | Provides sufficient memory for multiple Docker containers, Minecraft servers and background services. |
| Storage | M.2 NVMe SSD (500GB+) | Fast storage for the operating system, applications and Minecraft worlds, helping reduce loading times. |
| Additional Storage | 2TB HDD | Provides inexpensive additional storage for backups, archived files and server data. |
| Graphics | Dedicated graphics card (GTX 1070) | Required because the Ryzen 7 5700X has no integrated graphics. Provides display output for installation and troubleshooting. |

![Here is a picture of my build](\images\f5063951-d349-4aaa-ab05-cf2f5e1d91af.jpg)

## Operating System and Software

The server runs Ubuntu Server LTS, providing a lightweight Linux environment without the overhead of a traditional desktop operating system.

Some of the main technologies and tools used throughout the project include:

- **Ubuntu Server:** The underlying operating system.
- **Docker:** Used to run and manage isolated server applications in containers.
- **itzg/minecraft-server:** Docker image used to deploy Minecraft servers.
- **Fabric:** Modding platform used for the modded Minecraft server.
- **UFW:** Linux firewall used to control incoming and outgoing network traffic.
- **Fail2ban:** Helps protect services against repeated unauthorised login attempts.
- **Tailscale:** Provides private remote access to the server without relying on traditional port forwarding.
- **SSH:** Allows remote administration from my main Windows PC.

## What I learned & Further Plans

Throughout this project, I've developed a much better understanding of Linux system administration, networking and server management. I've gained practical experience installing and configuring Ubuntu Server, managing applications through Docker containers, setting up firewall rules and securing remote access using SSH and Tailscale.

I've also learned how to troubleshoot hardware and software issues, manage server resources and maintain backups of important data. Perhaps most importantly, the project has taught me how different areas of computing work together to create and maintain a functioning server environment.

There is still plenty more I want to explore, but this project has provided a valuable foundation in practical IT infrastructure and system administration.

