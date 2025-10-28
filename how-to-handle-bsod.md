# How to Troubleshoot a Blue Screen of Death (BSOD)

## 1. The Problem

A user's computer suddenly crashes and displays a solid blue screen with an error message. This is a "Stop Error" or "Blue Screen of Death" (BSOD) and can be caused by faulty hardware, bad drivers, or corrupt system files.

## 2. The Solution

The immediate goal is not to fix it, but to **gather the error information** so you can diagnose the problem.

1.  **Do Not Restart Immediately:** Ask the user to look at the blue screen.
2.  **Find the Stop Code:** On the screen (usually near the bottom), there will be a **"Stop Code"** or an error message in all caps (e.g., `DRIVER_IRQL_NOT_LESS_OR_EQUAL`).
3.  **Write Down the Code:** Have the user write down this exact Stop Code. This is the most important piece of information.
4.  **Restart the PC:** Ask the user to hold down the physical power button until the computer turns off, then turn it back on.
5.  **Analyze the Code:** Once the computer is back on (or if it won't boot), you can use a different computer to search for the Stop Code (e.g., search for `"DRIVER_IRQL_NOT_LESS_OR_EQUAL"`). The search results will usually point to the cause, such as:
    * A specific driver (like a WiFi or graphics driver) that needs to be updated.
    * Faulty RAM (memory).
    * A recently installed piece of hardware.

6.  **Next Steps:** Based on the code, you can try booting into **Safe Mode** to update or remove the bad driver.
