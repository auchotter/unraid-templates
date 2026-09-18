# Valheim Kartograph for Unraid

This repository contains the Unraid Community Applications template for
[Valheim Kartograph](https://github.com/auchotter/valheim-kartograph),
a self-hosted collaborative mapping tool for Valheim.

## Container

Image:

`ghcr.io/auchotter/valheim-kartograph:latest`

Default WebUI port:

`3000`

Persistent application data:

`/mnt/user/appdata/valheim-kartograph` -> `/data`

## Security

Valheim Kartograph does not include built-in authentication.

Use it only on a trusted/private network unless access is protected by an
external authentication layer or reverse proxy.

## Persistent data

The `/data` directory contains the SQLite database used by Valheim Kartograph.

For backups, stop the container before copying the database files so the
SQLite WAL can be cleanly synchronised.

## Licences

The files in this Unraid template repository are licensed under the MIT License.

Valheim Kartograph itself is separately licensed under the Apache License 2.0
with the Commons Clause. See the main project repository for its licence terms.

## Project

https://github.com/auchotter/valheim-kartograph
