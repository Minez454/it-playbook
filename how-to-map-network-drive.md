# How to Map a Network Drive

## 1. The Problem

A user needs frequent access to a shared folder on the company network (a "network share"). Opening it by typing the full network path (e.g., `\\Server\Share`) every time is inconvenient.

## 2. The Solution

You can "map" the network share to a drive letter (like Z:). This makes it appear in "This PC" just like a local C: drive.

1.  Open **File Explorer** (the yellow folder icon).
2.  Right-click on **"This PC"** on the left-hand side.
3.  Select **"Map network drive..."**.
4.  A new window will open.
5.  **Drive:** Choose an available drive letter from the dropdown menu (e.g., `Z:`).
6.  **Folder:** Type the full network path to the shared folder.
    * **Example:** `\\ServerName\SharedFolder`
7.  **Reconnect at sign-in:** Make sure this box is **checked** so the drive reconnects every time the user logs in.
8.  Click **"Finish"**.

The new network drive (Z:) will now appear in "This PC" for easy access.
