# Realtime Lisner v1.1

## Overview
This application fetches data from the CMS TCP connector on the configured ports and dumps it into an SQL database. It provides functionality for automated table creation during the first-time installation. Please ensure that the database is created before deploying the application.

## Features
- Service runs as windows executable file (.exe)
- Fetches realtime data from the CMS server on the configured ports
- Supports a maximum of two ports for data retrieval
- Dumps the fetched data into an SQL database configured in the config file
- Automatically creates tables in the database if they are not present during the first-time installation

## Configuration
Make sure to update the configuration file with the necessary settings before running the application. The configuration file should include the following details:
- Port numbers for the CMS TCP connector
- SQL database connection details (e.g., host, port, database name, username, password)

## Installation
1. Clone the repository to your local machine.
2. Create a virtual environment using a tool like `venv` or `virtualenv`. Run the command: `python -m venv myenv`. Replace `myenv` with the desired name for your virtual environment.
3. Activate the virtual environment:
   - For Windows: `myenv\Scripts\activate`
   - For macOS/Linux: `source myenv/bin/activate`
4. Navigate to the project directory.
5. Create the SQL database and ensure that the necessary credentials are available.
6. Update the configuration file with the appropriate settings.
7. Install the required dependencies by running the command: `pip install -r requirements.txt`.
8. Start the application using the command: `python main.py`.

## Usage
1. Ensure that the application is running and connected to the CMS TCP connector.
2. The application will automatically fetch data from the configured ports.
3. The fetched data will be stored in the SQL database specified in the configuration file.
4. If tables do not exist in the database, they will be automatically created during the first-time installation.

## About
This application is designed and developed by Future Technology. The author of this application is Shivanand.

## Support and Feedback
For any issues or feedback, please reach out to [smasne@alyousuf.com].
