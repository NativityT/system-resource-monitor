# System Resource Monitor
This application works as a python based System Resource Monitor, which identifies and analyzes computer processes. This application aids in the proper management and upkeep of computer systems, from Disk Usage to a live monitor to display real-time CPU Usage and Monitor Status.

## Features
    - Live Monitor Display
    - Monitor Processing Systems:
        a. View Current System Status
        b. View Top Processes
        c. View System Information {OS, Computer names, processor, Python version}
        d. Save Current Snapshot

## Technologies
    - Python Version: 3.14.8
    - Imported Libraries used: "psutil"
    - Standard Libraries Used: "os", "platform", "socket", and "time"

## Project Structure

```text
system-resource-monitor/
    logs/
        - snapshots.csv         # Timestamp record when each row of snapshots have been saved
        - logger.py             # Saves resource snapshots to a CSV file for the System Resource Monitor.
        - main.py               # Menu and user interactions for the TB System Resource Monitor.
        - monitor.py            # System information, resource monitoring, warnings, and live monitor for the TB System Resource Monitor.
        - README.md             # General Information and Portfolio for the System Resource Monitor
        - .gitinore             # Code ignored by Git to keep personal and junk files from the System Resource Monitor
        - requirements.txt      # List of neccessary Libraries for the System Resource Monitor

```

## Installation
git clone https://github.com/NativityT/system-resource-monitor.git
cd system-resource-monitor
python -m pip install -r requirements.txt

## How to Run
Start application from Project Folder by running

```bash
python main.py
```

## Main Options

1. **View Current System Status:** Realtime Snapshot of CPU, memory, and disk usage percentages as well as capacities.
2. ** Start Live Resource Monitor:** Continuous refreshing of system resource processing information in the terminal until session is terminated with 'Ctrl+C'
3. **View Top Processes:** List of top running processes by memory consumption sorted by PID, Name, and Memory %
4. **Save Current Snapshot:** Records current snapshot of resource metric with a timestamp into the file 'logs/snapshots.csv'.
5. **View System Information:** Displays saved System Information in the terminal
6. **Exit:** Closes the application

## Screenshots / Demo

![Live monitor running](screenshots/live-monitor.png)

## Known Limitations

**OS Memory Differences:** Calculations of memory usage may vary across operating systems like Windows, macOS, and Linux.

## Optional Features Added

None yet. 

## What I Learned

Going into this Project, I had no experience in coding, however now I understand the neccessary components to creating a viable code. Using Python Version 3.14.8 I was able to understand the advantage in using libraries like 'os' and 'psutil' which store pre-written code that I can utilize, rather than having to write everthing from scratch. I also learned the importance of files such as 'main.py', 'scratch.py, and '.gitinore' to create a location for my stored data, keeping the code organized and easier to review/debug.

