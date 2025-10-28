# How to Troubleshoot an Offline Printer

## 1. The Problem

A user tries to print, but the document won't come out. When they check the print queue, the printer's status says "Offline."

## 2. The Solution

This is a very common issue that can be caused by software or network problems. Follow these steps in order.

1.  **Physical Checks:** Ask the user to check that the printer is turned on and that the USB or network (Ethernet) cable is securely plugged into both the printer and the computer or wall port.

2.  **Restart the Printer:** Ask the user to turn the printer off, wait 10 seconds, and turn it back on. This simple step fixes a majority of printer issues.

3.  **Restart the Print Spooler:** This is a Windows service that manages print jobs.
    * Press **Windows Key + R** to open the "Run" dialog.
    * Type **`services.msc`** and press **Enter**.
    * Scroll down the list to find **"Print Spooler"**.
    * Right-click on "Print Spooler" and choose **"Restart"**.

4.  **Check Network (if applicable):** If it's a network printer, find its IP address from the printer's own settings screen. From the user's computer, open Command Prompt (`cmd`) and type `ping [printer_ip_address]` (e.g., `ping 192.168.1.50`). If you get a "Request timed out" error, there is a network problem.

5.  **Re-add the Printer:**
    * Go to Windows "Settings" > "Bluetooth & devices" > "Printers & scanners."
    * Click on the printer and select "Remove device."
    * Click "Add device" and let Windows re-discover and install the printer.
