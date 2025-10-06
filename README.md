# Note CLI

A simple command-line application written in Go for creating and saving notes.

## Description

This application allows users to create notes by providing a title and content via the command line. The note is then displayed and saved as a JSON file in the current directory.

## Installation

1. Ensure you have Go installed (version 1.24.6 or later).
2. Clone or download the project.
3. Run `go mod tidy` to download dependencies (none in this case).

## Usage

Run the application:

```bash
go run main.go
```

You will be prompted to enter:
- Note title
- Note content

The note will be displayed and saved as a JSON file named after the title (spaces replaced with underscores, lowercase).

Example output:
```
Note title: My First Note
Note content: This is the content of my note.
Your Note titled My First Note has the following content:
This is the content of my note.
Created at: 2023-10-01 12:00:00 +0000 UTC
Saving the note succeeded!
```

The file `my_first_note.json` will be created.

## Project Structure

- `main.go`: Entry point of the application.
- `note/note.go`: Package containing the Note struct and methods.
- `go.mod`: Go module file.

## License

MIT License
