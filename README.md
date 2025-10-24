# Dockerized-app-with-Lets-Encrypt


# dkljajo.github.io - Full Dockerized Site with HTTPS

This repository contains the updated and fully working version of your GitHub Pages site, **dockerized** and configured to run locally or on any server with **automatic HTTPS** using **Caddy**, **DuckDNS**, and **Let's Encrypt**.

---

## Project Overview

Originally, this project was a static site hosted on GitHub Pages. The goal was to:

1. Serve a static website (`index.html` and other assets).
2. Use **Caddy** for a local or server-based deployment.
3. Automate HTTPS certificates via **Let's Encrypt**.
4. Use **DuckDNS** for dynamic DNS support.
5. Containerize the project using **Docker** and **Docker Compose**.

---

## Features

- Static site served via **Caddy** web server.
- **Automatic HTTPS** via Let's Encrypt.
- **DuckDNS** integration for dynamic domains.
- Fully **dockerized** for easy deployment.
- Corrected previous configuration issues:
  - Fixed environment variable usage (`${DUCKDNS_DOMAIN}`).
  - Resolved Caddyfile syntax errors (heredocs, reverse proxy).
  - Working Dockerfile and docker-compose setup.

---

## Repository Structure

.
├── Dockerfile # Builds Docker image for Caddy
├── Caddyfile # Caddy configuration with DuckDNS
├── docker-compose.yml # Docker Compose setup
├── site/ # Static site files
│ └── index.html # Homepage
├── README.md

yaml
Copy code
