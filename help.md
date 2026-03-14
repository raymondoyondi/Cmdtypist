# CMD TYPIST HELP MENU

## Cmdtypist Commands:


| Command | Description |
| :--- | :--- |
| `select "lesson-number"` | Selects a specific lesson by number. Run at the `cmdtypist` prompt. |
| `cmdtypist mkuser "username"` | Creates a new user and stores the username. **Mandatory for first-time users.** Overwrites the current user data if one exists. |
| `cmtypist ls` | Lists available lessons for typing. Must be followed by `select "lesson number"`. |
| `cmtypist --help` | Displays this help menu. |
| `cmtypist man` | Displays the README file, which includes description, license (GNU GPL version 3 or later), installation, and features. |
| `cmdtypist select "lesson number"` | Automatically selects a lesson (1-15) for typing without listing them first. Requires an existing user. |
| `cmdtypist sound` | Activates (`--on`) or deactivates (`--off`) the beep sound on wrong character press. |
| `cmdtypist /myown` | Opens a user's personal text file for typing in standard mode. Supports only ASCII 7-bit characters. |
| `cmtypist cchl` | Resets the current lesson file to the program's default lesson file. |
| `cmdtypist mkstd` | Changes the typing mode to standard (chronological order). |
| `cmdtypist mkrand` | Changes the typing mode to random, choosing lesson blocks randomly. |
| `cmdtypist chblock "lesson number"` | Sets the number of lines to type per lesson (2-45). |
| `cmdtypist reset` | Performs a soft reset to default settings, preserving user files. |
| `cmdtypist reset raw` | Performs a hard reset, deleting all user data and saved speed details. Use with caution. |

## HELP IN QUESTIONS AND ANSWERS

### 1) What does it mean to type in standard mode?

Typing in standard mode means you type the lesson in the exact chronological order it appears in the lesson file. After each block, session results are displayed, and typing continues from where it ended.

### 2) I keep on getting the "Fatal Error, Some files are missing", what's happening?

This usually indicates a required program file is missing or inaccessible.
*   Ensure no other program is preventing `cmdtypist` from accessing its files. Close potentially interfering applications.
*   Make sure you are running the program correctly using the required `begin;` command (if applicable, per your description).
*   You can attempt to fix it with `cmdtypist reset raw`, but be sure to save your `user_speed` file first.
*   If the problem persists, the files may be permanently deleted, and you will need a fresh copy of the application.

### 3) Sound command produces no beep on wrong characters:

If the command was typed correctly, the issue is likely due to your system volume being low, your terminal not supporting beeps, or having beeps deactivated in your terminal settings.

### 4) How do i know i have come to the end of a lesson block?

The last line of each lesson block is colored blue. When you type the final character (ENTER), a session speed report is displayed.

### 5) Is it possible to know my speed details for yesterday? if yes, how?

Yes, all your typing speed history is stored in the `user_speed` info file located in the `cmdtypist` directory. The most recent speed is boxed.

### 6) Do i have to set mode to rand each time i want to type in random mode?

No. `cmdtypist` uses a hidden `.conf` file to save user settings persistently. You only need to run the `mkrand` command once. Use the `reset` command if settings become corrupted.

### 7) Do i have permission to copy lessons in the cmdtypist lesson file?

Yes, the lesson file is open source. Any copies must adhere to the terms of the GNU GPL version 3 or later license.

***

**NOTE:** All prompts ending in `[y/n]` require `y` for yes and `n` for no.
