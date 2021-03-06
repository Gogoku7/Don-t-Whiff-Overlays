# Super Smash Bros. Ultimate - Singles - Alternative Overlay

When deployed to IIS, change the baseUrl variable to 'localhost' or 'localhost/livestreamproductionmanager' (depending on which url Livestream Production Manager runs) in FightingGames/SuperSmashBros/JavaScript/OverlayManager.js and Web.config of the application to ensure the WebSocket connection to work.

To learn how to enable IIS, use: https://www.itnota.com/install-iis-windows/

Deploying to IIS and running can be done manually or using Visual Studio tools

**How to use in Open Broadcaster Software (OBS Studio):**
- Add a new Browser source to your scene
- Check the Local file checkbox and click Browse
- Select GameOverlay.html in this folder
- Set the resolution and framerate. (1920 x 1080 at 60 FPS recommended)
- Check Shutdown source when not visible and Refresh browser when scene becomes active checkbox

**The alternative default overlay can also be used for other formats:**
- Crew battle - Treat the Sponsor as Crew name and the Player name as Player of that crew currently active
- Squad Strike

**Selectors of manageable elements defined in the generated CSS/Content.css:**
- #roundText
- #player1NameText
- .player1Sponsor
- #player2NameText
- .player2Sponsor
- #player1Score
- #player2Score

If you have experience with HTML, CSS, JavaScript and Photoshop, you can create your own fully custom overlay using these Selectors