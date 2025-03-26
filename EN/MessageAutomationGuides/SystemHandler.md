# Discord Tool - Black Market Tool (Business Market Tool)

_Knowledge Guides - System Handler_

<hr>

> We have limit creating folder's maximum to 25 folders, so you must organize your folders on channels properly by follow the below.

<hr>

## There are 3 ways to control the creating folders

-   First (Mostly recommended): Create folder name that follow group type (like `selling` or `buying`...).

-   Second (Recommended): Create folder name that follow the timer (like `5m` or `10m`...).

-   Third (Bad): Create a folder name that combines both group type and timer (like `selling5m` or `buying10m`...).

<i>Depends on the folder name, you can add channels related to that folder and handle easily by the same message content that to be sent.</i>

<br>

## Handle folder's timer (In case of wrong working timer on folder)

Sometimes there's a small bugs that the timer doesn't work properly, so if you have many channels in a folder, you must follow the rule below for better folder handling.

```csharp
if there are more than 30 channels, set the timer to 5m.
if there are more than 40 channels, set the timer to 7.5m.
if there are more than 50 channels, set the timer to 10m.
```

> _Each 10 channels will increase the timer by 2.5 minutes._

## Cooldown controller

You don't need to mind about what if the channel's cooldown (on Discord Channel) is too short or too long for a folder, we made it automatically for you like the following.

```csharp
if folders timer = 5m, while channels cooldown = 30m, system will select 30m instead.
if folders timer = 1h, while channels cooldown = 30m, system will select 1h instead.
```

> _The system will always select the highest value between the folder's timer and the channel's cooldown._
