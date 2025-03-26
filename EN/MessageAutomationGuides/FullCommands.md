# Discord Tool - Black Market Tool (Business Market Tool)

_User Commands - Advanced/Full Commands_

<hr>

Table of Contents

-   [1. Folder commands guides](#1-folder-commands-guides)
-   [2. Timer commands guides](#2-timer-commands-guides)
-   [3. Channel commands guides](#3-channel-commands-guides)
-   [4. Message commands guides](#4-message-commands-guides)
-   [5. Attachment commands guides](#5-attachment-commands-guides)
-   [Dynamic folder on commands calling](#dynamic-folder-on-commands-calling)

<hr>

## 1. Folder commands guides

> Used to handle timer, channels that you added, message that you setted and many purposes for the auto.

_Click each section below to expand and see the details._

<details>
    <summary><strong>Select folder | Because of you can add many folders, so we will control specific folder by select it.</strong></summary>
    
```diff
!!folder select FOLDER_NAME
```
</details>

<details>
    <summary><strong>Create folder | Create a new folder and automatically select to it (Max 25 folders could be create).</strong></summary>
    
```diff
!!folder add FOLDER_NAME
```
</details>

<details>
    <summary><strong>Rename a folder.</strong></summary>
    
```diff
!!folder rename OLD_FOLDER_NAME NEW_FOLDER_NAME
```
</details>

<details>
    <summary><strong>Delete a folder.</strong></summary>
    
```diff
!!folder delete FOLDER_NAME
```
</details>

<details>
    <summary><strong>Show folders | show folders that you have added before.</strong></summary>
    
```diff
!!folder show
```
</details>

<details>
    <summary><strong>Turn on a folder | Enable functional to active the automation.</strong></summary>
    
```diff
!!folder on
```
</details>

<details>
    <summary><strong>Turn off a folder | Disable/Stop functional.</strong></summary>
    
```diff
!!folder off
```
</details>

<details>
    <summary><strong>Reset folders | Complete delete all folders at once.</strong></summary>
    
```diff
!!folder reset
```
</details>

## 2. Timer commands guides

_Click each section below to expand and see the details._

<details>
    <summary><strong>Set timer | Set the time for messages looping.</strong></summary>
    
```diff
!!timer set THE_TIME
```
The timer should be in the format of `1s`, `2m`, `3h`, `4d` (a.k.a 1 second, 2 minutes, 3 hours, 4 days).
<br>
Eg: `!!timer set 5m` # Sets the folder's timer to 5 minutes
</details>

## 3. Channel commands guides

_Click each section below to expand and see the details._

<details>
    <summary><strong>Add channels.</strong></summary>
    
```diff
!!channel add CHANNEL_ID
```
*You can add multiple channels at once by leave whitespace each ids like `!!channel add id1 id2 id3`...*
</details>

<details>
    <summary><strong>Show channels | Show all channels (as mention it) that you've added to the folder.</strong></summary>
    
```diff
!!channel show
```
</details>

<details>
    <summary><strong>Show channel ids | Show all channels (as id only) that you've added to the folder.</strong></summary>
    
```diff
!!channel showid
```
</details>

<details>
    <summary><strong>Delete channels.</strong></summary>
    
```diff
!!channel delete CHANNEL_ID
```
*You can delete multiple channels at once by leave whitespace each ids like `!!channel delete id1 id2 id3`...*
<br>
*If you do delete a channel that not in the current folder, the system will extend/across to all folders and delete it if found.*
</details>

<details>
    <summary><strong>Reset channels | Complete delete all channels at once in the folder.</strong></summary>
    
```diff
!!folder reset
```
</details>

## 4. Message commands guides

_Click each section below to expand and see the details._

<details>
    <summary><strong>Set message | Set the message content that used to send.</strong></summary>
    
```diff
!!message set MESSAGE_CONTENT
```

Slash Command is supported but only do single command like `/sound` but not like `/sound on`.

```diff
!!message set /{BOT_ID} {COMMAND}
```

Command Example: I want to do **`daily`** command with bot id **`123`**, the input should be `!!message set /123 daily`.

</details>

<details>
    <summary><strong>Show message | Show the message content that you've set.</strong></summary>
    
```diff
!!message show
```
</details>

## 5. Attachment commands guides

To be updated...

## Dynamic folder on commands calling

Some commands are supported to call directly on the command (by using minus `-`) without need to select the folder first.

#### For example, if you want to turn on a folder, you must to do the two commands below:

```diff
!!folder select FOLDER_NAME
!!folder on
```

But from now, you can simply do it in one command to run one or multiple folders at once:

```diff
!!folder on -FOLDER1 -FOLDER2 -FOLDER3 -FOLDER_N+1...
```

We also supports for `all` keyword to do the command to all folders at once:

```diff
!!folder on -all
```

#### For example with message set command:

```diff
!!message set -FOLDER1 -FOLDER2 -FOLDER3 -FOLDER_N+1... MESSAGE_CONTENT
```

#### For example with channel add command:

```diff
!!channel add -FOLDER1 id1 id2 id3
```

> **Note**: The dynamic folders on commands must be put before putting any value (such as message content, channel id, etc).

## Some commands that related to reset, limit to do only for a folder will be restricted to use dynamic folder on calling, you could try some if any bugs, feedback to me, Neko ~
