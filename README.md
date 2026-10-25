# UniPicker

A desktop app that helps UK students shortlist and compare universities based on what matters to them. Built in Python with CustomTkinter as my A level Computer Science NEA project.

## Screenshot of home page
<img width="2940" height="1789" alt="image" src="https://github.com/user-attachments/assets/10c6afe4-ef61-491f-9fd1-4297dda5f909" />



## Features

- **Accounts:** sign up and log in, with input validation and hashed passwords stored in SQLite
- **Preference quiz:** 9 questions covering location, city vs campus, cost, nightlife and extracurriculars
- **Saved universities:** build a shortlist, which is stored per user
- **Side-by-side comparison:** compare two universities, with sections ordered by your quiz answers (if cost matters most to you, costs come first)
- **Map view:** shows your home postcode on a map (in progress)

## Tech

- Python 3, [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) for the UI
- SQLite (`sqlite3`) for users, quiz answers and saved universities
- [tkintermapview](https://github.com/TomSchimansky/TkinterMapView) and [pgeocode](https://github.com/symerio/pgeocode) for the map and postcode lookup
- University data for 10 UK universities in `university_data.json`

## Running it

1. Clone the repo:
   git clone https://github.com/samuelgrimshaw/UniPicker.git
   cd UniPicker
2. Install the dependencies:
   pip install -r requirements.txt
3. Run the app:
   python main.py

The database (`login.db`) is created automatically on first run.

## What I learned

- (2–3 bullets in your own words, for example: structuring a multi-page GUI, designing a database schema, why passwords are hashed)

## Planned improvements

- Finish the map: plot saved universities and add navigation back
- Salted password hashing 
- Automated tests and CI
