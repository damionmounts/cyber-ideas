# cyber-ideas

A repository to hold ideas and notes about potential cyber security projects.

---

#### Clipboard Copier (Cross-platform)

A small tool that displays the clipboard history with time-stamps.

* Python
    * Library: pyperclip
    
* Simple UI (Tk)
    * Clear log
    * Pause updating
    * Poll-rate selection
    * Save to file

**Purpose:** The clipboard is not a secure means of passing information between applications as it can be read freely.
It provides no access control like that of User Interface Privilege Isolation in Windows. This tool only serves to 
monitor clipboard history. Perhaps it can be utilized as a diagnostic tool in the case of a malicious piece of software 
that overwrites the clipboard without user intervention.

---

#### Focus Keeper (Linux)

A tool that prevents applications from stealing focus. Focus would only be allowed to shift if the user explicitly
clicked the new window or they used hot-keys to switch to it. Windows attempting to steal focus will automatically be
minimized and a notification will be passed to the user.

* Python
    * Libraries: keyboard, mouse, (something for notifications)
    * Interface to the X Window System

* Simple UI (Tk)
    * Configure allowed hot-key combinations
    * Notification settings
    * Full-screen windows allowed or not

**Purpose:** This tool serves as an anti-nuisance measure. Not too long ago, I was having issues in Linux Mint 19.2.
The focus-stealing prevention settings within the desktop environment were doing nothing to stop MATLAB from stealing 
focus every time it opened. There were a couple times where I would open MATLAB and then KeePass right after - MATLAB
would finally open and steal focus as I was half-way through typing my password.

---
