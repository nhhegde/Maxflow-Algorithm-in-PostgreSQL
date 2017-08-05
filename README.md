# Maxflow-Algorithm-in-PostgreSQL

## Description
Calculates the maximum flow through a graph stored on disk in PostgreSQL using Kruskal's Algorithm. 
Written in python.

## Requirements
`python3`
`PostgreSQL` (Version 9+)

## Usage

`python3 test.py"

Or hookup your own PostgreSQL database. You will need to create the following tables and populate them with valid graph data. See test.py for more information.

`CREATE TABLE original_edge (id SERIAL, src int, dst int, capacity int);`
`CREATE TABLE edge (id SERIAL, src int, dst int, capacity int);`
`COPY original_edge(src,dst,capacity) FROM %s DELIMITER ',' CSV HEADER;`
`COPY edge(src,dst,capacity) FROM %s DELIMITER ',' CSV HEADER;`
