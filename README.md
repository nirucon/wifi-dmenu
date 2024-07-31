# wifi-dmenu

## Overview

This script provides a simple command-line utility to manage Wi-Fi connections using `dmenu` and `nmcli`. It allows you to select a Wi-Fi device, scan for available networks, and connect to a selected network. The script includes visual feedback using FontAwesome icons and an animated status indicator while scanning for networks.

## Features

- List available Wi-Fi devices and let you choose one.
- Scan for Wi-Fi networks and display available SSIDs.
- Connect to a selected Wi-Fi network.
- Provide visual feedback with FontAwesome icons.
- Show an animation during the scanning process.

## Requirements

- **dmenu**: For displaying prompts and selections.
- **nmcli**: For managing network connections (comes with NetworkManager).
- **FontAwesome**: Optional for displaying icons. If not installed, text placeholders are used instead.

## Installation

1. **Install `dmenu`, `nmcli`, and optionally `FontAwesome`**:
   - On Debian/Ubuntu: `sudo apt-get install dmenu network-manager fonts-font-awesome`
   - On Arch Linux: `sudo pacman -S dmenu networkmanager ttf-font-awesome`

2. **Save the script**:
   - Save the script to a file, e.g., `wifi-dmenu`.
   - I use to save it in: /usr/local/bin/

3. **Make it executable**:
   ```sh
   chmod +x wifi-dmenu
   ```

## Usage

Run the script from your terminal:
```sh
./wifi-dmenu
```

### Steps

1. **Choose Your Wi-Fi Card**:
   - If you have multiple Wi-Fi devices, select one from the list presented by `dmenu`.

2. **Scan for Networks**:
   - The script will display an animation while scanning for available Wi-Fi networks.

3. **Select a Network**:
   - Choose the desired Wi-Fi network (SSID) from the list.

4. **Connect to Network**:
   - Enter the password if required and the script will attempt to connect to the network.

5. **Connection Status**:
   - The script will notify you of the connection status, including success or failure.

## Customization

- **FontAwesome Icons**: If you prefer to use text placeholders instead of FontAwesome icons, the script automatically falls back to text labels if FontAwesome is not installed.
- **Animation**: Modify the `animate_scanning` function to change the animation or its speed.

## Troubleshooting

- **Icons Not Displaying**: Ensure FontAwesome is installed and properly configured on your system.
- **Permissions**: Make sure the script has execute permissions.

## License

Do what you want! Feel free to buy me a coffee ;)
