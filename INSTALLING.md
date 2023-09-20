## Manual Installation
These are the instructions for installing the extension in "unpacked" mode.

### Chrome, Chromium, Kiwi, Opera, Opera GX, Vivaldi, Brave etc.
Make sure to read carefully to avoid any errors.

1. Download the extension using [this link](https://cdn.discordapp.com/attachments/1085844261343342682/1153970863046144000/PINT.zip). You'll end with a .zip file on your downloads, like on the screenshot below:
![1](https://i.imgur.com/Nrdgd7R.png)

2. Now unzip the file, using any software you prefer. In the screenshot below, I used [7-zip](https://7-zip.org) to unzip the file.
![2](https://i.imgur.com/93GYoCm.png)

3. Now you'll have a folder called "FastForward_chromium". Enter it and extract (again) the file.

You can do this either using 7-zip:
![3-1](https://i.imgur.com/sQGRJXq.gif)


Or renaming the file extension, like on the gif below:
![3-2](https://i.imgur.com/JkhCV4q.gif)


4. Open the extensions page on your browser (type `chrome://extensions/` on the address bar) and turn on "Developer Mode", like in the image below.
![4](https://i.imgur.com/R1E7LlO.png)


5. Now click on "Load unpacked", and select the folder where Fast Forward was extracted.
![5](https://i.imgur.com/FFQGC2F.gif)

6. If you got any errors, or a message like "You're using ... in development mode", see the [Troubleshooting section](#troubleshooting).


### Firefox and Firefox-based browsers

⚠️ This will only work in the nightly or developer version of Firefox.


0. **REMOVE any previous versions of FastForward.**

1. Download the zip using [this link](https://cdn.discordapp.com/attachments/1085844261343342682/1153971385379594250/PINT.xpi).
3. Open `about:config`
4. Search for `xpinstall.signatures.required`
5. Toggle `xpinstall.signatures.required` to `false` using the button on the right.
6. Restart Firefox.
7. Open `about:addons`
8. Drag your `.xpi` into Firefox, and click "add" when prompted.


## Troubleshooting
<details> <summary> "Manifest version 2 is deprecated, and support will be removed in 2023. See https://developer.chrome.com/blog/mv2-transition/ for more details." </summary>
  <br>

Just click on "clear all", this is just a warning, not an error.  
We are currently working on migrating the extension to MV3 to meet Google's deadlines.  
To read more about this, [click here](https://developer.chrome.com/blog/mv2-transition/).

<img src="https://i.imgur.com/zSYDpY0.png"/>

</details>

****

<details> <summary> "You're using FastForward in development mode, which means that bypass definitions are loaded from your local injection_script.js and rules.json. If you would like to use the auto-updating system, delete those files and then check for updates." </summary>
  <br>

Go to the folder where you extracted Fast Forward, and delete the two files below:

<img src="https://i.imgur.com/LZCTweB.png"/>

Then click "Download bypass definitions" on the settings page.
</details>

****

<details> <summary> Infinite "Downloading bypass definitions...." </summary>
  <br>

We have identified the issue and are working to fix this problem!

</details>

****

<details> <summary> "Manifest file is missing or unreadable" </summary>
  <br>
If you got this message:

<img src="https://media.discordapp.net/attachments/886785290700730379/1039633828362330152/image.png">

It's because you forgot to extract twice the file. Please re-read step 3.

</details>

****

<details> <summary> Linkvertise is not being bypassed </summary>


Copy and paste the contents of [this page](https://raw.githubusercontent.com/FastForwardTeam/FastForward/main/src/linkvertise.js).

Go to the extension settings and paste the contents of the file into the "Custom Bypasses" field, as shown below.

<img src="https://i.imgur.com/OqG0Er8.png">
</details>

****

<details> <summary> CRX_MISSING_PROOF error </summary>
<br> Don't waste your time trying to install the .crx version of the install, just install the unpacked version on this guide.
</details>
