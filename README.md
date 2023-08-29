# Automated Time Management System using Python and SQL

This repository contains the code to automate your time management using Python and SQL. By following the steps outlined here, you can set up an automated system to track your coding hours and events in Google Calendar.

## Prerequisites

Before you get started, make sure you have the following:

1. **Python**: You'll need Python installed on your system. If not, you can download it from [python.org](https://www.python.org/downloads/).

2. **Google Calendar API Credentials**: Obtain your Google Calendar API credentials by following these steps:
   - Go to the [Google Cloud Console](https://console.developers.google.com/).
   - Create a new project or select an existing project.
   - Enable the Google Calendar API for your project.
   - Create credentials for a "Desktop App".
   - Download the credentials JSON file and rename it to `credentials.json`.
   - Make sure to replace `'YOUR_CALENDAR_ID'` in the code with your actual Google Calendar ID.

3. **SQLite Database**: SQLite is used for storing your coding hours data. Make sure you have the SQLite library available in your Python environment.

## Setup

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/time-management.git
   cd time-management

2.  Install the required Python packages:
  ```bash
 pip install -r requirements.txt
```
3. Create a virtual environment (recommended):
 ```bash
 python -m venv venv
source venv/bin/activate      # On Windows, use: venv\Scripts\activate.
```
4. Initialize the SQLite database:
   ```bash
   python createTable.py

## Usage
### Add Calendar Event
To add an event to your Google Calendar, run the following command:
```bash
python timeManager.py add <duration_in_hours> <event_description>
```
- Replace <duration_in_hours> with the duration of the event in hours and <event_description> with a brief description of the event.
  
## Commit Coding Hours
To commit your coding hours for the day to the SQLite database, run:
```bash
python timeManager.py commit
```
## Get Total and Average Hours
To get the total and average coding hours for the last <number_of_days>, run:
```bash
python timeManager.py getHours <number_of_days>
```
Replace <number_of_days> with the desired number of days.

## Notes
- Make sure your credentials.json and token.json files are in the same directory as the script files.
- The provided token in the comments is a placeholder. You should replace it with the actual token obtained after authentication.
- Adjust the time zone (YOUR_TIMEZONE) and other settings as needed.

## Disclaimer
- This code is provided as-is and may require adjustments to fit your specific environment. Use it responsibly and ensure that your Google Calendar API credentials are kept secure.
