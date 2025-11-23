# Library Management System

A simple command-line library management system built with Python that allows you to manage books, issue them to members, and track returns using CSV files for data storage.

## Features

- **Add Books**: Add new books to the library with unique Book IDs
- **Issue Books**: Issue available books to library members
- **Return Books**: Process book returns and update availability
- **View Books**: Display all books with their availability status

## Requirements

- Python 3.x
- No external dependencies (uses built-in `csv` and `os` modules)

## Installation

1. Download the `library_management.py` file
2. No additional installation required

## Usage

Run the program from your terminal:

```bash
python library_management.py
```

### Main Menu Options

1. **Add Book** - Add a new book to the library collection
2. **Issue Book** - Issue an available book to a member
3. **Return Book** - Process a book return
4. **View All Books** - Display the complete book inventory
5. **Exit** - Close the application

## Data Storage

The system uses two CSV files to store data:

- `books.csv` - Stores book information (Book ID, Title, Author, Total Quantity, Available Quantity)
- `issued_books.csv` - Tracks issued books (Book ID, Title, Member Name)

These files are automatically created when you first run the program.

## Example Workflow

1. **Adding a Book**
   - Select option 1
   - Enter Book ID (e.g., B001)
   - Enter Title (e.g., "The Great Gatsby")
   - Enter Author (e.g., "F. Scott Fitzgerald")
   - Enter Total Quantity (e.g., 5)

2. **Issuing a Book**
   - Select option 2
   - Enter Book ID of an available book
   - Enter Member Name
   - The available quantity decreases by 1

3. **Returning a Book**
   - Select option 3
   - Enter Book ID
   - Enter Member Name
   - The available quantity increases by 1

4. **Viewing Books**
   - Select option 4
   - See all books with their availability status

## Notes

- Book IDs must be unique
- Books can only be issued if available quantity is greater than 0
- Returns require both Book ID and Member Name to match an issued record
- All data persists in CSV files between sessions

## License

Free to use and modify.# library-management-system.py
