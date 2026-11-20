# Car Rental & Fleet Management System

A Java desktop application for managing a rental fleet. It combines a Swing interface with SQLite persistence and demonstrates core Java programming concepts through vehicle inventory and rental workflows.

## Features

- Add, search, update, and delete vehicles through a graphical interface
- Store vehicle records in a local SQLite database using JDBC and prepared statements
- Model standard and luxury vehicles with classes, inheritance, interfaces, and polymorphism
- Demonstrate collections, generics, exception handling, and multithreading
- Write and read rental agreement data using Java byte streams
- Build and launch with scripts for macOS, Linux, and Windows

## Requirements

- JDK 8 or newer (JDK 17 or newer recommended)
- A graphical desktop session to use the Swing interface

The SQLite JDBC driver is included in `lib/`; no separate database server is needed.

## Run

From the repository root on macOS or Linux:

```sh
chmod +x compile.sh run.sh   # first run only
./compile.sh
./run.sh
```

On Windows, run these from Command Prompt:

```bat
compile.bat
run.bat
```

The launch scripts use the bundled SQLite driver. `rentals.db` is created or updated in the working project directory as the application runs. In a headless environment, the program uses its terminal diagnostic flow instead of opening the GUI.

## Project files

- [Project report (PDF)](JAVA_PROJECT_REPORT.pdf)
- [Run commands and setup guide](RUN_COMMANDS.txt)
- [Java source](Main.java)
- [SQLite JDBC driver](lib/sqlite-jdbc.jar)

## Repository layout

```text
.
├── Main.java                 # Java application and Swing interface
├── lib/sqlite-jdbc.jar       # Bundled SQLite JDBC driver
├── rentals.db                # Local SQLite database
├── compile.sh / compile.bat  # Build scripts
├── run.sh / run.bat          # Launch scripts
├── RUN_COMMANDS.txt          # Setup and execution guide
└── JAVA_PROJECT_REPORT.pdf   # Project report
```

## Academic context

Built as an Advanced Java Programming laboratory project for CSE 307 at SRM University–AP. The code is organized around five units: object-oriented programming, polymorphism and exceptions, threads and byte streams, JDBC and collections, and generics with a Swing GUI.
