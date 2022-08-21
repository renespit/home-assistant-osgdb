# home-assistant-osgdb
Opensource Dishes Database (compatible with Home Assistant)

![How nice would it be if you find dished on the internet in your Home Assistant console? ]<img width="611" alt="ha_console" src="https://user-images.githubusercontent.com/34937329/185789871-87385463-601d-4350-a3c9-46f7b3c0807c.png">

Find in your console a nice dish and send the shoppinglist to your Home Assistant Shopping List.

#Quick Start
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


