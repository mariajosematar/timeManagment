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

