
Desktop Application Install Guides
===================================

Mattermost desktop applications are available for Windows, Mac and Linux operating systems. They support all the features of the web experience, plus: 

 - Connect to multiple Mattermost servers from a single interface, and switch with shortcut keys.
 - Auto-start Mattermost when a user logs into their machine
 - (Windows) Add Mattermost to Start menu, taskbar and system tray
 - (Mac) Add Mattermost to the applications Dock
 - (Linux) ``Desktop Entry`` for the application to more easily `integrate into a desktop environment <https://wiki.archlinux.org/index.php/Desktop_entries>`_

Below is a list of additional resources:

 - `Guide for configuring your desktop app experience <https://docs.mattermost.com/help/apps/desktop-guide.html>`_
 - `Changelog <https://docs.mattermost.com/help/apps/desktop-changelog.html>`_
 - Contributor’s guide (coming soon)
 - `Source code <https://github.com/mattermost/desktop>`_

You can `download the apps directly from our downloads page <https://about.mattermost.com/downloads/>`_. You may also use the following installation guides for Windows, Mac and Linux.

.. contents::
    :backlinks: top

Windows 10+, Windows 8.1+, Windows 7+
--------------------------------------------------

1. Download latest version of the Mattermost desktop app:

   - `64-bit version of Windows <https://releases.mattermost.com/desktop/3.5.0/mattermost-setup-3.5.0-win64.exe>`_
   - `32-bit version of Windows <https://releases.mattermost.com/desktop/3.5.0/mattermost-setup-3.5.0-win32.exe>`_

2. From the ``\Downloads`` directory right-click on the file ``mattermost-setup-3.5.0...`` and select **Open**.

This will start an installer for the app. Once finished, the Mattermost desktop app will open automatically.
 
Mac OS X 10.9+
--------------------------------------------------

1. Download `latest version of the Mattermost desktop app <https://releases.mattermost.com/desktop/3.5.0/mattermost-desktop-3.5.0-osx.tar.gz>`_

2. From the ``/Downloads`` directory, find ``/mattermost-desktop...`` folder.

   - If one doesn’t exist, from the ``/Downloads`` directory, find a file ending in ``-osx.tar.gz`` and double-click on the file. The ``/mattermost-desktop...`` folder should now be created.

3. From the ``/mattermost-desktop...`` folder, right-click on ``Mattermost`` package and select **Open**. If you see a dialog to confirm the application, choose **Open**.

The Mattermost desktop should open automatically.

Linux (Beta)
--------------------------------------------------

1. Download latest version of the Mattermost desktop app:

   - `x64.tar.gz <https://releases.mattermost.com/desktop/3.5.0/mattermost-desktop-3.5.0-linux-x64.tar.gz>`_
   - `ia32.tar.gz <https://releases.mattermost.com/desktop/3.5.0/mattermost-desktop-3.5.0-linux-ia32.tar.gz>`_

2. Extract the archive, then execute ``Mattermost`` which is located inside the extracted directory.

3. If you need a Desktop Entry for the application to integrate into a desktop environment, please refer to https://wiki.archlinux.org/index.php/Desktop_entries

To download the unofficial, community-driven .deb packages for the desktop application:

1. Download latest version of the Mattermost desktop app:

   - `amd64.deb <https://releases.mattermost.com/desktop/3.5.0/mattermost-desktop-3.5.0-linux-amd64.deb>`_
   - `i386.deb <https://releases.mattermost.com/desktop/3.5.0/mattermost-desktop-3.5.0-linux-i386.deb>`_

2. Open a terminal and execute the command ``sudo dpkg -i mattermost-desktop-<VERSION>-<ARCH>.deb``

3. Open **Dash** (located at top left corner) and input ``mattermost``, then click the Mattermost icon. The Mattermost desktop should open automatically.

Troubleshooting
--------------------------------------------------

Possible solutions to issues encountered when using the Desktop App.

"Installation has failed" dialog
    The app data might be corrupted - remove all the files in `C:\Users...\AppData\Local\mattermost`, then try re-installing the app.

Desktop App window is black and doesn't load the page
    - First try to clear cache and reload the app from **View** > **Clear Cache and Reload** or by pressing CTRL/CMD+SHIFT+R.
    - Next, quit the app and restart it to see if the issue clears.
    - If neither of the above works and you are using a special video driver such as Optimus, try disabling it to see if the problem is resolved.
    - Finally, try disabling GPU hardware acceleration by using the `--disable-gpu <http://peter.sh/experiments/chromium-command-line-switches/#disable-gpu>`_ Chromium command line switch.

    If none of the above steps resolve the issue, please open a new ticket in the `Mattermost Troubleshooting Forum <https://forum.mattermost.org/t/how-to-use-the-troubleshooting-forum/150>`_. 
