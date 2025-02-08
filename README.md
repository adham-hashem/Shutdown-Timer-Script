# Shutdown Timer Script

This is a simple batch script that schedules a system shutdown after a specified time.

## Usage

By default, this script will shut down your computer in **1 hour**.

### Steps to Use:
1. **Download** the script.
2. **Run** the script (`.bat` file) by double-clicking it.
3. A message will appear indicating that the system will shut down in 1 hour.

## Customization

You can edit the number of hours by modifying the `shutdown` command in the script:

```batch
shutdown /s /t 3600
```

- `3600` represents **1 hour** (in seconds).
- If you want to change the duration, replace `3600` with the desired number of seconds.
  - **Example:** To shut down after 2 hours, use:
    
    ```batch
    shutdown /s /t 7200
    ```

## Cancelling the Shutdown

If you need to cancel the scheduled shutdown, open **Command Prompt** and type:

```batch
shutdown /a
```

This will **abort** the scheduled shutdown.

## Troubleshooting

### 'shutdown' is Not Recognized as a Command
If you receive an error stating that `shutdown` is not recognized as an internal or external command, ensure that **System32** is included in your system's **PATH** environment variable:

1. Open **System Properties** → **Advanced** → **Environment Variables**.
2. Under **System Variables**, find **Path**, edit it, and add `C:\Windows\System32`.
3. Try again, and if there is the same error, then restart your computer and try running the script again.

## License

This script is provided under the **MIT License**. Feel free to modify and share it!

