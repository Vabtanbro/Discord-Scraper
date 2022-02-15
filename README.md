# Discord Scraper
  
## Configuring

### Desktop Application:

**Step 1:**
Open your Discord app and enter the user settings.
![https://imgur.com/HnNnmRT](https://i.imgur.com/HnNnmRT.png "Step 1")

**Steps 2 and 3:**
Traverse to appearance and enable developer mode if it is not enabled.
![https://imgur.com/LTrGjVX](https://i.imgur.com/LTrGjVX.png "Step 2")
![https://imgur.com/7ItCXBV](https://i.imgur.com/7ItCXBV.png "Step 3")

**UPDATE:**
It appears that the developers of the Discord desktop application have implemented another method by which to keep people from normally being able to access the developer tools.
![https://i.imgur.com/BuZf2qn.png](https://i.imgur.com/BuZf2qn.png "Step 3.5")

This doesn't necessarily prevent us from being able to make use of this script but I'm definitely going to have to figure something out that doesn't require you to have to put in your passwords or any two-factor authentication tokens; this is the most convenient method for me to implement for the time-being but it's becoming increasingly difficult to continue on like this given that people have accidentally pushed their own authorization tokens to their own public forks of this repository in the past which only serves to reinforce decisions like this from the Discord staff.

### Website:

**Step 4:**
Open the developer tools by pressing CTRL + SHIFT + I *(Command + Shift + I on macOS)* and navigate to the network tab to gather your authorization token by moving about the interface *(in this example I jumped to the Nitro tab and back to generate the "science" request)*.
![https://imgur.com/o9Sf0CH](https://i.imgur.com/o9Sf0CH.png "Step 4")


**Step 5:**
Gather the guild ID that you want to scrape from by right-clicking on the icon for the guild on the left-side of the Discord window and selecting *"Copy ID"*.
![https://imgur.com/14ysTcN](https://i.imgur.com/14ysTcN.png "Step 5")

If you're wanting to grab from a direct message instead, then this method won't return the correct ID that is needed by the script.

The only real way to get this with ease through the Discord app is to open the direct message you want to scrape from and then open the developer tools to see the correct ID in the title bar of the developer tools window and paste it into the JSON file.

**Step 6:**
Gather the channel ID that you want to scrape from by right-clicking on the channel name to the right of the guild icons and selecting *"Copy ID"*.
![https://imgur.com/cdpTLCG](https://i.imgur.com/cdpTLCG.png "Step 6")
