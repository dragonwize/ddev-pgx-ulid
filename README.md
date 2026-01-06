[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/dragonwize/ddev-pgx-ulid/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/dragonwize/ddev-pgx-ulid/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/dragonwize/ddev-pgx-ulid)](https://github.com/dragonwize/ddev-pgx-ulid/commits)
[![release](https://img.shields.io/github/v/release/dragonwize/ddev-pgx-ulid)](https://github.com/dragonwize/ddev-pgx-ulid/releases/latest)

# DDEV Pgx Ulid

## Overview

This add-on integrates Postgres extension for ULID [pgx_ulid](https://github.com/pksunkara/pgx_ulid) into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get dragonwize/ddev-pgx-ulid
ddev restart
ddev create-ext-ulid
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description                                     |
| ------- |-------------------------------------------------|
| `ddev describe` | View service status and used ports for Pgx Ulid |
| `ddev logs -s pgx-ulid` | Check Pgx Ulid logs                             |
| `ddev create-ext-ulid` | Add the Postgres extension to your database     |

## Credits

**Contributed and maintained by [@dragonwize](https://github.com/dragonwize)**
