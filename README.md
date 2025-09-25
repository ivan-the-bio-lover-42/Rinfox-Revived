# Rinfox-Revived
Rinfox is an Internet Explorer 7-8 theme for Firefox 115esr. It was last forked in 2024 and has since received no updates. This fork introduces new visual elements and exposes some native Firefox features which were hidden in previous iterations of the Rinfox theme. For convenience, I have included the necessary files for easy installation. Enjoy!
This is my update fork of Rinfox, the Internet Explorer 7/8 theme for Firefox 115esr originally conceived by travy-patty in 2023. It is for the latest Firefox 115esr release, 115.28.0esr. I based my fork off of the newer 2024 update fork by yuvia08. This is my first Github repo so bear with me please :)

A thing to note: my fork is strictly an IE8 theme, so the IE7 theme remains unchanged.

For simplicity's sake, I have provided most of the files so that you can run the theme on the go.

Here is a rough list of changes:

- With the expection of the forward, back, and history buttons, the buttons in the navigation bar (e.g. identity buttomn (secure or insecure page), notification buttons (share   location, save password or card info), refresh, stop, urlbar dropdown, search button, and search dropdown) all have fading hover animations now. This was done to more   accurately emulate the button hover animations seen in real IE8, and to make the theme seem more "native" and give the illusion of integration with the Windows shell.
- New icons that have been pulled straight from Windows 7 system files such as shell32.dll, explorerframe.dll, ieframe.dll, and icardres.dll.
  - The notification icon that appears when saving credit card information is from Windows Cardspace
  - The save login notification icon is from slui.exe. 
  - The allow site notifications icon is from IE8.
  - The share location notiifcation icon is from IE8.
  - New tab, new window, and InPrivate tasks in the taskbar jumplist are now styled to use IE8 icons. 
- Firefox's reader mode button, a page action button which was previously hidden in the Rinfox theme, is now exposed and will become visible when Firefox determines a page can   be adapted to be more readable. The button uses the compatibility mode icon from IE8. 
- A dropdown chevron has been added to the urlbar and will expand the urlbar when clicked to show results and suggestions. 
- The statusbar will now display URLs when links are hovered and will also display loading progress strings instead of just saying "Done" when a page is done loading.
- The InPrivate badge will no longer disappear when the urlbar is expanded in InPrivate mode. Additionally, the URL placeholder text says "about:InPrivate" in private browsing   tabs.
- The overflow new tab button now looks the same as the non-overflow new-tab button and is accurate to real IE8 behavior
- The issue of thin glass being visible when playing videos in fullscreen in the browser has been fixed. The fullscreen video will now properly take up the whole screen as   expected.
- Perhaps one of the things I am most proud of: the PDF viewer has been styled. Windows 7 and IE8 never had a PDF viewer. I have made a Windows/IE8-themed PDF viewer that aims   to visualize what a Windows PDF viewer would've looked like. THe viewer has been styled after Microsoft Word 2010.
- Various Firefox loading wheels (in the PDF viewer and in the printing GUI) have been replaced with the spinning aero wheel.
- The help button will now open Windows 7 Help and Support - ASSUMING YOU HAVE RESTORED IT. Otherwise the button will throw an error message reminding the user to restore the   Help and Support infrastructure. I have no clue how to make the button open Help and Support to the right help topic - but it's a step. This was also done to increase the   "integrated" feel of the theme. 

Installation Instructions:

For user convenience, I have included all the files necessary to get the theme going. The two directories you will modify are the profile and installation folders.
- Installation Directory (C:\Program Files\Mozilla Firefox)
  - xul.dll: This is the native controls patch (credit to Isabella) for Firefox 115ESR. I have patched it to function with 115.28.0esr, the latest 115esr release.
  - config.js
  - firefox.exe: This is the firefox executable, but patched to use icons from IE8.
  - browser folder: Replace the original folder (you can rename the original) with the one from the pack
  - defaults folder: Rename omni.ja and replace it with this one.
- Profile Directory (C:\Users\[USER]\AppData\Roaming\Mozilla\Firefox\Profiles\[Profile])
  - Place the chrome folder from the pack in this directory. This contains all the assets, scripts, and visual style rules to get the theme working.
  - Rename the original prefs.js file in this directory and replace it with the one from the pack. This contains all the about:config changes necessary to get the theme running. I did it so you don't have to <3

Hope you enjoy it, this was a fantastic project to work on and I amm glad to be able to share it with the community.

Gallery:
- PDF Viewer with Reader Mode:
<img width="1100" height="671" alt="image" src="https://github.com/user-attachments/assets/22ea9bd9-3d40-4ce0-bd35-81dbf8d87406" />


Notification Icons:
- Allow notifications:
<img width="386" height="63" alt="image" src="https://github.com/user-attachments/assets/ff132ee9-2fb2-4f5d-85d1-3fd4e6be847b" />


- Save login:
<img width="261" height="66" alt="image" src="https://github.com/user-attachments/assets/256450c7-4e8f-44f3-96dd-3df76cab8073" />


- Share location:
<img width="425" height="179" alt="image" src="https://github.com/user-attachments/assets/68dd06ab-c685-4e2d-bed2-efb3b039c8a9" />


- Save card info:
<img width="455" height="227" alt="image" src="https://github.com/user-attachments/assets/af878315-975d-4ad8-8d24-0df7ce60cc1f" />


- Taskbar jumplist icons:
<img width="247" height="187" alt="image" src="https://github.com/user-attachments/assets/9cd332db-8625-4d4b-9478-eea1874ca21d" />

Additional Stuff:

You can get the feed toolbar button here. It is the Feedbro extension by Nodetics: https://addons.mozilla.org/en-US/firefox/addon/feedbroreader/

You can get the all tabs button here. It is TipTab by William Wong: https://addons.mozilla.org/en-US/firefox/addon/tip-tab/

Clicking the help button may trigger an error message saying Help and Support isn't installed. If this happens on Windows 7 or if you've already restored 7 Help and Support on 10, edit the HelpButtonun.uc.js script in the chrome folder and find the user path - edit it to your username and then clear the Firefox startup cache. This should fix the issue.

Credits:
Rinfox - travy patty, yuvia08
Native Controls patch - ImSwordQueen, kawapure
FeedBro - Nodetics
All Tabs - William Wong
