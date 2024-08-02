# FortiClientAutoLogin

FortiClientAutoLogin is a script designed to automatically open FortiClient VPN after the operating system starts and log in using a predefined username and password. This tool simplifies the process of connecting to your VPN by automating the login procedure.

## Features

- **Automated VPN Connection**: Opens FortiClient VPN and logs in automatically.
- **Predefined Credentials**: Uses predefined username and password for login.
- **Logging**: Logs all activities and actions taken by the script for easy monitoring.

## Requirements

- **Windows OS**: Ensure you have a Windows operating system.
- **Windows Script Host (WSH)**: Ensure WSH is enabled and properly configured.
- **FortiClient**: Ensure FortiClient VPN is installed and accessible from the script.

## Installation

1. **Clone the Repository**:

    ```sh
    git clone https://github.com/sqhard08/FortiClientAutoLogin.git
    cd FortiClientAutoLogin
    ```

2. **Create the Script File**:

    Save the following script as `FortiClientAutoLogin.wsf`:

3. **Run the Script**:

    Execute the script to automatically open FortiClient VPN and log in:

    ```sh
    wscript FortiClientAutoLogin.wsf
    ```

## Configuration

- **tunnelName**: The name of the VPN tunnel.
- **userName**: Your VPN username.
- **password**: Your VPN password.
- **fortiClientPath**: Path to the FortiClient executable. Modify if necessary.

## Example Task Scheduler Entry

To run the script on startup, you can add a task to the Windows Task Scheduler:

1. Open Task Scheduler.
2. Create a new task.
3. Set the trigger to "At startup".
4. Set the action to run the Windows Script Host with the `FortiClientAutoLogin.wsf` script.
