# Discord Tool - Black Market Tool (Business Market Tool)

_Presence Commands_

<hr>

#### Syntax definitions:

-   `{}` - Required field.
-   `[]` - Optional field | You can leave blank/empty in the command.
-   `URL` - Any URL.
-   `IMAGE_URL` - Raw Image URL (You can also upload image to Discord and get Image URL from it).
-   `TEXT` - Any Text.
-   `TYPE` - Presence types | Such as name, details, state, etc... checkout [Presence Types](presence_example.png) or image below.

#### Presence Types <img id="presence-example" src="presence_example.png" alt="Presence Types" width="600" />

Command example with syntax definitions:

> if the command is `!!command {TEXT}` and you want to `TEXT` to be `Hello`, then you will type `!!command Hello`.
> if the command is `!!set {URL} [TEXT]` and you want to `TEXT` to be nothing, then you will type `!!set https://www.youtube.com/watch?v=dQw4w9WgXcQ`.

<hr>

## Commands

_Click each sections below to expand and see the details._

<details>
    <summary><strong>Show settings | Show your presence settings.</strong></summary>
    
```diff
!!presence show
```
</details>

<details>
    <summary><strong>Set a type | Change specific type in the presence settings.</strong></summary>

Please head over to [Presence types setting up](#presence-types-setting-up) in below to see more commands details.

</details>

<details>
    <summary><strong>Delete a type | Delete specific type in the presence settings.</strong></summary>
    
```diff
!!presence delete {TYPE}
```
</details>

<details>
    <summary><strong>Display presence | Enable to display your presence in your profile.</strong></summary>
    
```diff
!!presence enable
```
</details>

<details>
    <summary><strong>Stop display presence | Stop to display your presence in your profile.</strong></summary>
    
```diff
!!presence disable
```
</details>

<details>
    <summary><strong>Reset settings | Delete all types in the presence settings (leave all blank).</strong></summary>
    
```diff
!!presence reset
```
</details>

## Presence types setting up.

This section is about setting up your presence types by using command, see [Syntax definitions](#syntax-definitions) to see the input command and [CLICK THIS](#presence-types) to see the type which you want to set up.

<details>
    <summary><strong>Type: Name.</strong></summary>
    
```diff
!!presence set name {TEXT}
```
</details>

<details>
    <summary><strong>Type: Details.</strong></summary>
    
```diff
!!presence set details {TEXT}
```
</details>

<details>
    <summary><strong>Type: State.</strong></summary>
    
```diff
!!presence set state {TEXT}
```
</details>

<details>
    <summary><strong>Type: Large (Also with large text).</strong></summary>
    
```diff
!!presence set large {IMAGE_URL} [TEXT]
```
`TEXT` in this command is allowed to empty.
</details>

<details>
    <summary><strong>Type: Small (Also with small text).</strong></summary>
    
```diff
!!presence set small {IMAGE_URL} [TEXT]
```
`TEXT` in this command is allowed to empty.
</details>

<details>
    <summary><strong>Type: Button1.</strong></summary>
    
```diff
!!presence set button1 {URL} {TEXT}
```
</details>

<details>
    <summary><strong>Type: Button2.</strong></summary>
    
```diff
!!presence set button2 {URL} {TEXT}
```
</details>

<details>
    <summary><strong>Type: Time.</strong></summary>
    
```diff
!!presence set time {THE_TIME}
```
In `THE_TIME` field, you are allowed to put one of the following:
- `1` - Display the uptime since the system startup.
- `TIMEZONE` - Display the current time in the specific timezone.
<br>
You can choose your timezone in the link [https://en.wikipedia.org/wiki/List_of_tz_database_time_zones](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)
and put a text from `TZ identifier` on website to the `THE_TIME` field.
<br>
For example: if my timezone with UTC offset is +07:00, I will put `Asia/Ho_Chi_Minh` to the `THE_TIME` field, so it will be:
<br>
`!!presence set time Asia/Ho_Chi_Minh`
</details>

## Note: If your Presence is enabling but you made changes in settings, your Presence will be disabled automatically, and after done with your Settings, please enable it again.
