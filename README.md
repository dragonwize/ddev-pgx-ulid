[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/dragonwize/ddev-pgx-ulid/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/dragonwize/ddev-pgx-ulid/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/dragonwize/ddev-pgx-ulid)](https://github.com/dragonwize/ddev-pgx-ulid/commits)
[![release](https://img.shields.io/github/v/release/dragonwize/ddev-pgx-ulid)](https://github.com/dragonwize/ddev-pgx-ulid/releases/latest)

# DDEV Pgx Ulid

## Overview

This add-on integrates Pgx Ulid into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get dragonwize/ddev-pgx-ulid
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Pgx Ulid |
| `ddev logs -s pgx-ulid` | Check Pgx Ulid logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.pgx-ulid --pgx-ulid-docker-image="ddev/ddev-utilities:latest"
ddev add-on get dragonwize/ddev-pgx-ulid
ddev restart
```

Make sure to commit the `.ddev/.env.pgx-ulid` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `PGX_ULID_DOCKER_IMAGE` | `--pgx-ulid-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@dragonwize](https://github.com/dragonwize)**
