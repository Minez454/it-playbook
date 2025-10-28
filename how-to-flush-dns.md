# How to Flush the DNS Cache

This guide explains how to clear the Windows DNS cache, which often fixes "site can't be reached" errors.

## 1. The Problem

A user reports they cannot access a specific website that you know is online. Their internet connection seems fine, but they get a DNS error. This can be caused by a corrupt or outdated local DNS cache on their computer.

## 2. The Solution (Windows)

1.  Click the **Start** button.
2.  Type **`cmd`**.
3.  You will see **"Command Prompt"**. Right-click on it and select **"Run as administrator"**.
4.  A black terminal window will open.
5.  Type the following command exactly and press **Enter**:

    ```
    ipconfig /flushdns
    ```

6.  You should see a message: "Successfully flushed the DNS Resolver Cache."
7.  Have the user close and re-open their web browser.
