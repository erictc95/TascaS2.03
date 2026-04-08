# TascaS2.03 - MongoDB Backups and Data Models

This repository contains MongoDB database backups along with their corresponding data model diagrams.

## Repository Structure

Each folder represents an independent database:

TascaS2.03/
│
├── optics_cul_dampolla/
│ ├── *.bson
│ ├── *.metadata.json
│ └── diagrama.drawio
│
├── optics_cul_dampolla-Glasses/
│ ├── *.bson
│ ├── *.metadata.json
│ └── diagrama.drawio
│
├── La_Pampara_TakeAway/
│ ├── *.bson
│ ├── *.metadata.json
│ └── diagrama.drawio


## Contents

Each database folder includes:

- `.bson` files → collection data  
- `.metadata.json` files → collection structure  
- `diagrama.drawio` → visual representation of the data model  

## Data Source

Backups were generated using MongoDB with Docker:

mongodump --out /dump


## Diagrams

Diagrams were created using Draw.io and represent:

- Collections  
- Fields  
- Relationships between entities  

## Restore Example

To restore a database:

mongorestore /path/to/folder

Example:

mongorestore ./optics_cul_dampolla


## Author

Eric Tarres Cabrisas
