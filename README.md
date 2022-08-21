# home-assistant-osgdb
Opensource Dishes Database (compatible with Home Assistant)

![How nice would it be if you find dished on the internet in your Home Assistant console? ]<img width="611" alt="ha_console" src="https://user-images.githubusercontent.com/34937329/185789871-87385463-601d-4350-a3c9-46f7b3c0807c.png">

Find in your console a nice dish and send the shoppinglist to your Home Assistant Shopping List.

# Quick Start
- Create a new dashboard
- Open your new dashboard
- Select 'Configure UI'
- Select 'Empty Dashboard'
- Add en new card
- Select in the GUI a webpage card
- Omit the title
- Add in URL: https://osgdb.nl
- Add in aspect ratio: 100%
- Save your card
- Back in your dashboard select the second pencil in your upper right corner
- Select in display type: Panel (1 card)
- Save this view
- Now your ready

```
views:
  - theme: Backend-selected
    title: Home
    type: panel
    badges: []
    cards:
      - type: iframe
        url: https://osgdb.nl
        aspect_ratio: 100%
```

# Known Issues
I tested only on Apple OSX and Apple IOS. 

If you run this program in the Home Assistant Application then you are not able to log in into your own account. Sessions inside iFrames don't work anymore.
If there is somebody who can tell me how I can disbale Private Security for iFrames I would be very happy.

If you run this program in the Home Assistant Application then you are not able to change the language setting. Because the language setting is saved into a cookie. Default Thirth Party Cookies are not allowed.

If you run this program in the Home Assistant Application then you are not able to use the Shoppinglist. Because the language setting is saved into a cookie. Default Thirth Party Cookies are not allowed.

Work around for these issues.
1. Open Home Assistant in Saffari
2. Open your Dishes Dashboard
3. Enable in Safari the Developer-Menu (Preferences -> Advanced Tab -> Show developer-menu in menubar)
4. Open the Developer-Menu
5. Select 'Disable Cross-Origin Restriction'
6. Disable 'Prevent Cross-Sitetracking' (Be Careful! This is a privacy setting)
7. Now you are able to select a country. Create/Save/Login your account. Save the CSS of Home Assistant in https://osgdb.nl 

