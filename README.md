# Intergalactic Travel System

A database-backed travel management system built with Python and MySQL for a course project.

This application manages planets, space stations, spaceports, routes, spacecraft, and flights in an intergalactic travel scenario. It provides GUI-based data entry and query functions, including itinerary search with transfer and timing constraints.

## Features

- Data entry for planets, space stations, spaceports, routes, spacecraft, and flights
- Spaceport query
- Route query
- Flight finder
- Constraint validation for routes, spacecraft range, and itinerary timing

## Constraints Implemented

- No flights are allowed between spaceports on the same planet
- A spacecraft cannot be assigned to a route longer than its range
- The first flight must depart on or after the requested time and within 3 hours
- Transfer time between connecting flights must be at least 1 hour
- A traveler cannot stay at a stop for more than 6 hours
- Input validation is enforced during data entry

## Tech Stack

- Python
- MySQL
- Tkinter
- SQL

## Repository Structure

- `code_version2/` — final project code
- `schema_intergalactic_travel.sql` — database schema
- `config.example.txt` — example database configuration file

## Setup

1. Install MySQL locally.
2. Create a database named `intergalactic_travel`.
3. Run `schema_intergalactic_travel.sql` to create the tables.
4. Copy `config.example.txt` and create your own local config file with database credentials.
5. Make sure your local config file matches what the Python code expects.
6. Run the main program from the `code_version2` folder.

## How to Run

From inside `code_version2/`, run:

```bash
python main.py
```

## Notes

- This project was developed as a course database application with a local MySQL backend and GUI frontend.
- The repository includes the final version of the code in `code_version2/`.
- Local credential files are not included for security reasons.
