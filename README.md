<h1 align="center">iOS Text Messages</h1>

## About
Hello and welcome! This is the iOS text messages that I coded to be used for my fics, but feel free to use them if you want (all i ask is for some sort of acknowledment or credit or something)
### Fanfics + Examples
This code has been used in the following fanfics of mine (plus an example from said fics):
1. [Echoes of a Name](https://archiveofourown.org/works/68759771)

<img width="250" height="500" alt="image" src="https://i.postimg.cc/nhWxdTXW/Screenshot-2025-07-30-193848.png" alt="An image containing coded iOS-style text messages. It says that the time is 10:34 and shows some texts in a group chat called The CDF Den. It has two text messages from around Tuesday 10:32 AM. Dad: Urban Studies sounds like an exciting major! | Papa: let us know if you ever wanna design us a garden :D"/>

2. [Shelved Hearts](https://archiveofourown.org/works/73408191)

<img width="250" height="500" alt="image" src="https://i.postimg.cc/BZB8k1RP/Screenshot-2025-10-30-164710.png" alt="An image containing coded iOS-style text messages. It says that the time is 12:20 and shows some texts in a group chat called three geniuses and alex. It has four text messages from around Monday 12:20 PM. Alex: made it to the library | everything is so old | also there's this guy | he could murder with silence alone"/>

## How to Add to Your Own Fic!
### Preparation
1. Download the **index.html** and **style.css** files from above
2. Put them in a folder (this will make it easy to keep track of them!)
3. Open the **index.html** file
4. This should show in your browser:
<img width="250" height="500" alt="image" src="https://github.com/user-attachments/assets/f750ee26-ba17-4c7d-ad65-09f5b30bba61" alt="An image containing coded iOS-style text messages. It says that the time is 9:41 and shows some texts in a group chat called Group Chat. It has five text messages from around Monday 10:32 AM. User1: AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAH | Sender: AAAAAAAAAAAAAAAAH | AAAAAAAAAAAAAAAAH | User2: AAAAAAAAAAAAAAAAH | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAH"/>

### Customizing
#### In Order to Customize the Time:
1. Use the find function (usually CTRL/CMD + F) to find this part of the code: `<div class="time">9:41</div>`
2. Change the `9:41` part to whatever time you desire
3. Save the file
4. Reload the page in your browser
5. The 9:41 should now be changed to your desired time!
#### In Order to Customize the Group Chat Name:
1. Use the find function (usually CTRL/CMD + F) to find this part of the code: `<div class="group-name">Group Chat</div>`
2. Change the `Group Chat` part to whatever name you desire
3. Save the file
4. Reload the page in your browser
5. The Group Chat should now be changed to your desired name!
#### In Order to Customize the Group Chat Image:
1. Use the find function (usually CTRL/CMD + F) to find this part of the code: `<img src="https://em-content.zobj.net/source/apple/419/fox_1f98a.png" alt="Fox Icon" />`
2. Replace the `https://em-content.zobj.net/source/apple/419/fox_1f98a.png` with an image url of your choice
3. Save the file
4. Reload the page in your browser
5. The fox image should now be changed to your desired image!
#### In Order to Customize the Background of the Group Chat Image:
1. Open the **style.css** file (this is really the only thing that needs the css to be changed, everything else should be done through the html)
2. Use the find function (usually CTRL/CMD + F) to find this part of the code:
```
    .group-icon {
      width: 50px;
      height: 50px;
      background: linear-gradient(to bottom, #ffd1a6, #fca85d);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      border: 1px solid #ccc;
    }
```
3. Replace the `#ffd1a6` and `#fca85d` in `background: linear-gradient(to bottom, #ffd1a6, #fca85d);` with the hex codes of your desired colors
4. Save the file
5. Reload the page in your browser
6. The orange-ish background should now be changed to your desired color!
#### In Order to Customize the Timestamp:
1. Use the find function (usually CTRL/CMD + F) to find this part of the code:
`<div class="timestamp">Monday 10:32 AM</div>`
2. Change the `Monday 10:32` part to whatever time you desire
3. Save the file
4. Reload the page in your browser
5. The Monday 10:32 AM should now be changed to your desired name!
#### In Order to Customize the Text Messages:
1. Use the find function (usually CTRL/CMD + F) to find this part of the code:
`<div class="chat-container">`
2. Underneath `<div class="timestamp">Monday 10:32 AM</div>` should be the following part of code:
```<div class="timestamp">Monday 10:32 AM</div>
    <div class="bubble-wrapper left"><div class="sender-name">User1</div><div class="bubble last">AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAH</div></div>
    <div class="bubble-wrapper right"><div class="bubble">AAAAAAAAAAAAAAAAH</div></div>
    <div class="bubble-wrapper right"><div class="bubble last">AAAAAAAAAAAAAAAAH</div></div>
    <div class="bubble-wrapper left"><div class="sender-name">User1</div><div class="bubble last">AAAAAAAAAAAAAAAAH</div></div>
    <div class="bubble-wrapper left"><div class="bubble last">AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAH</div></div>
```
3. DELETE THIS!
4. In the same place you just deleted do the following:

	**For a Text Message That is Being Recieved:**
	1. Enter the following code: `<div class="bubble-wrapper right"><div class="bubble">AAAAAAAAAAAAAAAAH</div></div>`
	2. Replace the `AAAAAAAAAAAAAAAAH` with a text of your choice
 	3. Save the file
	4. Reload the page in your browser
 	5. Your text message should appear!

	*If You Want to Add a Sender Name:*
	1. Add `<div class="sender-name">User1</div>` between `<div class="bubble-wrapper left">` and `<div class="bubble">`
	2. Replace the `User1` with a name of your choice
 	3. Save the file
	4. Reload the page in your browser
 	5. A sender name should be shown above the text message!

	*If You Want to Add the Tail Part:*
	1. Replace `<div class="bubble">` with `<div class="bubble last">`
 	2. Save the file
	3. Reload the page in your browser
 	4. Your text message should have a tail to the left of it!

	**For a Text Message That is Being Sent:**
	1. Enter the following code: `<div class="bubble-wrapper right"><div class="bubble">AAAAAAAAAAAAAAAAH</div></div>`
	2. Replace the `AAAAAAAAAAAAAAAAH` with a text of your choice
 	3. Save the file
	4. Reload the page in your browser
 	5. Your text message should appear!

	*If You Want to Add the Tail Part:*
	1. Replace `<div class="bubble">` with `<div class="bubble last">`
 	2. Save the file
	3. Reload the page in your browser
 	4. Your text message should have a tail to the right of it!

5. Add as many text messages as desired (while the container will change its height depending on how many text messages are in it, there is a limit. if it cuts off, then you'll need to take a screenshot of what you have, delete the text messages and continue where you left off)

### Adding to the Fic
1. Take a screenshot of the text messages
2. Go to [postimages.org](https://postimages.org/) (or any image hosting website)
3. Upload your screenshot
4. Take the url that you are given
5. Go to your fic on AO3 (make sure you're in html and not rich text!)
6. Put the following code in your desired spot: `<img src"postimages.org">` (make sure to replace the postimages.org with the url that you were given!)
7. If you want to change the width of the image, just simply add width="100" (make sure it is within the <> and change the 100 to the width you want your image to be!)
8. If you want to change the height of the image, just simply add height="100" (make sure it is within the <> and change the 100 to the height you want your image to be!)
9. If you want to add an alternative text to the image (for accessibility or in case your image doesn't load properly), just simply add alt="alt text here" (make sure it is within the <> and change the alt text here to the alternative text you want to add to your image! here's an example of an alt text that i use: An image containing coded iOS-style text messages. It says that the time is 10:34 and shows some texts in a group chat called The CDF Den. It has two text messages from around Tuesday 10:32 AM. Dad: Urban Studies sounds like an exciting major! | Papa: let us know if you ever wanna design us a garden :D)
