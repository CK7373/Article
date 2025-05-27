Article Management System

A Python-based system for managing relationships between Authors, Articles, and Magazines using SQLite database.

Features
Manage Authors, Articles, and Magazines
Track relationships between entities
Query articles by author or magazine
Find contributing authors and their works
Analyze magazine publishing statistics
Setup
Create a virtual environment:
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
Install dependencies:
pip install pytest
Set up the database:
python scripts/setup_db.py
Seed the database with sample data:
python lib/db/seed.py
Usage
Interactive Debug Console
Run the debug console to interact with the system:

python lib/debug.py
Available commands:

List all authors
List all magazines
List all articles
Find author by name
Find magazine by name
Find articles by author
Find articles by magazine
Get magazine contributors
Get author's magazines
Get top publisher
Running Tests
Run the test suite:

pytest
Project Structure
code-challenge/
├── lib/                    # Main code directory
│   ├── models/            # Model classes
│   │   ├── author.py      # Author class
│   │   ├── article.py     # Article class
│   │   └── magazine.py    # Magazine class
│   ├── db/               # Database components
│   │   ├── connection.py  # Database connection
│   │   ├── seed.py       # Seed data
│   │   └── schema.sql    # Database schema
│   └── debug.py          # Interactive console
├── scripts/              # Helper scripts
│   └── setup_db.py       # Database setup
└── tests/               # Test directory
Database Schema
The system uses SQLite with the following schema:
authors: Stores author information
magazines: Stores magazine information
articles: Links authors and magazines with articles

Contributing
Fork the repository
Create a feature branch
Commit your changes
Push to the branch
Create a Pull Request

Languages
Python
100.0%
Footer
© 2025 GitHub, Inc.
Footer navigation
Terms
Priva
