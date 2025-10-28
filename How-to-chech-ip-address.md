# How to Troubleshoot "No Internet Access"

## 1. The Problem

A user's computer is on and connected to the network (either by Wi-Fi or cable), but they cannot access any websites or network resources. The network icon in the taskbar might have a yellow triangle or globe icon.

## 2. The Solution

The first step is to check if the computer has a valid IP address. If it doesn't, it can't communicate with the network.

1.  Click the **Start** button.
2.  Type **`cmd`** and press **Enter** to open the Command Prompt.
3.  In the black terminal window, type the following command and press **Enter**:

    ```
    ipconfig
    ```

4.  Look at the results for your "Ethernet adapter" or "Wireless LAN adapter".
5.  Find the line that says **"IPv4 Address"**.

### How to Read the Results:

* **Good IP:** If the address looks something like `192.168.1.10` or `10.1.10.50`, the computer has a valid address from the network. The problem is likely elsewhere (like DNS or the firewall).

* **Bad IP (APIPA):** If the address starts with **`169.254...`**, it's an "APIPA" address. This means the computer tried to get an IP address from the network router (DHCP server) but failed.

### How to Fix a Bad IP:

1.  Ask the user to restart their computer (this fixes it most of the time).
2.  If it's a wired connection, have them unplug and replug the Ethernet cable.
3.  If it's Wi-Fi, have them "Forget" the network and reconnect.
