# Process Monitoring Script


This Python script monitors the creation of processes on a Windows system. It logs details of each new process to a CSV file, including the command line, executable path, parent process ID (PID), process ID (PID), user, and privileges.

## Features

- Monitors the creation of new processes in real-time.

- Logs the following information for each new process:

  - CommandLine

  - Time of creation

  - Executable path

  - Parent process ID (PID)

  - Process ID (PID)

  - User associated with the process

  - Privileges associated with the process

- Logs information into a CSV file (`process_monitor_log.csv`).

## Requirements

Ensure Python 3.x is installed. Install the required dependencies with the following command:
`pip install pywin32 wmi`

## How to Use

1. Clone or copy the script to your local machine.
2. Open a terminal or command prompt with administrator privileges (required for monitoring processes).
3. Navigate to the directory where the script is saved.
4. Run the script using:

`python process_monitor.py`

5. The script will continuously monitor for new processes. Each time a new process is created, it will log the details to the CSV file (`process_monitor_log.csv`).
6. To stop the script, press `Ctrl+C`.

## Importance

- **Security Monitoring**: This script is useful for system administrators or security professionals who want to monitor new processes running on a system to detect any suspicious or unauthorized activity.
- **Process Auditing**: It helps in auditing system processes to understand what is being executed on a machine and when.
- **Forensic Investigations**: The CSV logs can be used in forensic investigations to track the execution of unauthorized processes.

## CSV Log Format

Each row in the CSV log represents a new process and contains the following fields:

|CommandLine|Time|Executable|Parent PID|PID|User|Privileges|
|---|---|---|---|---|---|---|
|...|...|...|...|...|...|...|

## Example CSV Entry
`"cmd.exe", "2024-12-11T14:55:00", "C:\\Windows\\System32\\cmd.exe", 1234, 5678, "JohnDoe", "N/A"`

## Notes
- The script only logs processes created after it starts running.
- Ensure the script is run with administrator privileges to access all necessary process information.
- If you experience any issues with WMI or permissions, check that your system has the required access to monitor processes.

## License
This script is licensed under the MIT License. See the LICENSE file for more details.
## Contributing
Feel free to open issues or submit pull requests for improvements or bug fixes.

``This is the complete `README.md` content written in one continuous section as per your request. It includes installation, usage instructions, and other necessary information for running the script.``

