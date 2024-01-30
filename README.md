# Plex-Media-Server-Backup-How-To
How-To Backup your Plex Media Server.

***

# Back Up Main Plex Media Server Data

Steps:

1. Run and Open you Plex Media Server in your browser, go to `Settings > Library` and disable `Empty trash automatically after every scan`.
2. Close the running instance of your server (usually in the `notification area` part of you taskbar, right-click Plex Media Server > click `Exit`).
3. Make a backup of the main Plex Media Server data directory.
4. Navigate to `%LOCALAPPDATA%` and there should be a folder called `Plex Media Server`.
5. Zip this folder (we are zipping the folder as it may be large with thousands of files so copying-pasting the folder is not as reliable nor as fast as having a zip backup).
6. Once the folder has completed zipping, move the zipped folder to an external drive where it can serve as a backup.
7. Part 1 done.

# Back Up Additional Settings

Steps:

1. Open the `Registry Editor`
2. Navigate to `HKEY_CURRENT_USER\Software\Plex, Inc.\Plex Media Server`
3. Right click on the `Plex Media Server` folder > Export
4. Name it something like `Plex Setting`
5. Move this exported Registry Key to the same location as the above zip folder to serve as a backup on an external drive.

**BACKUP DONE**

# Restore Plex Media Server Data & Settings

Steps:

1. Make sure `Plex Media Server` is installed but not currently running.
2. Navigate to `%LOCALAPPDATA%` and there should be a folder called `Plex Media Server`, delete this folder.
3. Copy your data zip folder backup to `%LOCALAPPDATA%`.
4. Extract the zipped `Plex Media Server` folder.
5. Once the extraction is complete:
6. Copy the Registry Key backup from your external drive to somewhere on your system drive (Like the `Desktop` for example).
7. Run the Registry Key.
8. Restore is now done.
9. You can run `Plex Media Server` app and all your metadata and view states should be just as it was when you backed it up.
10. Remember to: Run and Open you Plex Media Server in your browser, go to `Settings > Library` and ENABLE `Empty trash automatically after every scan`.
11. Ba-boom!

ENJOY!

***

SOURCES:

[Backing Up Plex Media Server Data](https://support.plex.tv/articles/201539237-backing-up-plex-media-server-data/)

[How to Backup or Move Your Plex Media Server](https://www.youtube.com/watch?v=1mhOkM_Du-4)

