# Discord Tool - Black Market Tool (Business Market Tool)

_User Commands - Beginner Commands_

<hr>

<details open>
    <summary><strong>1. Add a Folder | Used to handle timer, channels etc...</strong></summary>
    
```diff
!!folder add FOLDER_NAME
```
</details>

<br>

<details open>
    <summary><strong>2. Set Timer | Continue looping after messages sent forever ~</strong></summary>
    
```diff
!!timer set THE_TIME
```
The timer should be in the format of `1s`, `2m`, `3h`, `4d` (a.k.a 1 second, 2 minutes, 3 hours, 4 days).
<br>
Eg: `!!timer set 5m` # Sets the folder's timer to 5 minutes
</details>

<br>

<details open>
    <summary><strong>3. Add a Channel | Where to send to.</strong></summary>
    
```diff
!!channel add CHANNEL_ID
```
*You can add multiple channels at once by leave whitespace each ids like `!!channel add id1 id2 id3`...*
</details>

<br>

<details open>
    <summary><strong>4. Set Message | What to send.</strong></summary>
    
```diff
!!message set MESSAGE_CONTENT
```
</details>

<br>

<details open>
    <summary><strong>[Optional] 5. Set Image as attachment.</strong></summary>
    
```diff
!!attachment set (+ upload images at the same time with the command)
```
*Note: Both actions must be performed at the same time.*
<br>
*Note 2: Attachments only accept images with these format types: `png`, `jpg`, `jpeg`, `gif`, `webp`.*
</details>

<br>

<details open>
    <summary><strong>6. Enable the Folder | All Set, head over to turn on the auto.</strong></summary>
    
```diff
!!folder on
```
</details>

<hr>

After those steps, you have finished setting up an automation for looping messages.

From now on, you can type `!!list` to see upcoming message sending time.

> **Note: Before you continue to do any steps on above again to make more folders, you should understand how exactly folder works on multiple channels by reading [System Handler](SystemHandler.md).**

### So if you good at all of above, head to [Full Commands](FullCommands.md) to read more advanced/fully commands.
