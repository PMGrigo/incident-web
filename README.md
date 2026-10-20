# Incident Web

## Overview
This is a training project for learning Linux, Git, systemd, and basic web server troubleshooting.

The project uses a Python HTTP server managed by systemd.

## Project Files
- `systemd/incident-web.service` — systemd service configuration.
- `site/health.txt` — a simple file used to check whether the web server responds correctly.

## Health Check
The web server listens on `127.0.0.1:18765`.

To check the service, run:

`curl http://127.0.0.1:18765/health.txt`

Expected response:

`OK`

## Deployment
Git stores the project files and their history. Pushing changes to GitHub does not automatically update the running server.

To deploy changes, the relevant project files must be installed on the server, and the service configuration must be applied when necessary.

