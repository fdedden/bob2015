---
layout: standalone
title: Information on how stream directing works at BOB 2022
head: 2022
language: en
---

## How to direct

### Setup

checkout the git repo: ```ssh://git@gitlab.active-group.de:1022/ag/bob.git```
if you have already cloned the repo be sure to pull.
run the script `setup.sh` in the directory `obs`
e.g. `./setup.sh <ldap-name>`

### OBS Setup
Import the scene collection via `Scene Collection > Import`
Enable `Studio Mode` in the bottom left corner.
Click on the Gear Icon to the right of the transition button in the
middle of the screen. Ensure that the checkmark for `Duplicate Scene` is set
and the checkmark for `Swap Preview/Output Scenes After Transitioning` is **not** set.

#### Streaming Setup
Goto `File > Settings > Stream`.
As Service select `YouTube - RTMPS`.
As Server `Primary YouTube ingest server`
Click `Use Stream Key (advanced)` and enter the room specific
stream key.
The stream keys are in the bob repo under `obs`

Goto `Video` and make sure base and output resolutions are set to
`1920x1080`.


### Allocation

- **Talks #1**: Felix (Backup: Heli)
- **Talks #2**: Raoul (Backup: David)

### Preparations

- set the YouTube steam key in vdo
  - go to **File** -> **Settings** -> **Stream**
  - select ```YouTube - RTMP```, ```Primary YouTube ingest server``` and enter the stream key for your room
  - ask Felix for the stream key for your room / pinned comment in mattermost BOB-Regie
- set stream qualitiy in vdo
  - go to **File** -> **Settings** -> **Video**
  - Set ``Output Scaled Resolution`` to 1280x720
- create [`vdo.ninja`](https://vdo.ninja) room for your track
  https://vdo.ninja/?director=bob_talks_1&password=bobig_talks_1&codirector=bobig_director_1
  https://vdo.ninja/?director=bob_talks_2&password=bobig_talks_2&codirector=bobig_director_2
  - room name: ```bob_talks_1``` or ```bob_talks_2```
  - password: ```bobig_talks_1``` or ```bobig_talks_2```
  - Screen share your OBS application to the room
  - Backup directors should also join the room as directors
- schedule
  - Talk #1: [`https://bobkonf.de/2022/program-talk-1.html`](https://bobkonf.de/2022/program-talk-1.html)
  - Talk #2: [`https://bobkonf.de/2022/program-talk-2.html`](https://bobkonf.de/2022/program-talk-2.html)

### In case of a Problem
- write in ```BOB-Regie``` so your backup can take control

### Stream start

- Stream starts 8:30
- Show scene: ```Welcome```

### Introduction and Keynote

- is only streamed in **talks #1**, in **talks #2** show slide `Talk Derek Dreyer`
- Prepare scene: ```Welcome to BOBKonf```
- Mike joins **talks #1** with **video**
- From **talks #1** copy Mike's link into Mike's source
- Show scene:  ```Welcome to BOBKonf```
- Mike will welcome everyone and then announce the keynote
- Prepare scene: ```Keynote```
- when Mike is done with the announcement switch scenes to ```Keynote```
- Show scene: ```Keynote```
- Start a local timer to keep track of the end of the talk
- Prepare scene: ```Q&A```
- Speaker joins **talks #1** with **video** and **screen sharing**
- From **talks #1** copy Speaker's **video** and **screen sharing** links into
  the speaker and slides sources of the ```Q&A``` scene
- give the speaker and moderator a heads up towards the end of the talk
- Show scene: ```Q&A```
- Prepare scene: ```Break```
- after the ```Q&A``` switch to the appropriate ```Break``` scene
- Show scene: ```Break```

### Every Talk

- Prepare scene: ```Talk Announcement```
- Moderator joins **vdo.ninja room** with **video**
- From **vdo.ninja room** copy moderator's **video** into moderator's source
- Show scene: ```Talk Announcement```
- Prepare scene: ```Talk```
- After the moderator's introduction start talk
- Show scene: ```Talk```
- Start a local timer to keep track of the end of the talk
- Prepare scene: `Q&A`
- Speaker joins **vdo.ninja room** with **video** and **screen sharing**
- From **vdo.ninja room** copy speaker's **video** and **screen sharing** links
  into the speaker and slides sources of the ```Q&A``` scene.
  Some talks have two speakers, be sure to insert both **video** links into the correct
  source.
- Announce end of the talk to speaker and moderator
- Show scene: `Q&A`

### Outro
- streams only in **talks #1**, in room **talks #2** show `Outro`
- Prepare scene: `Outro`
- Mike joins **talks #1** with **video**
- From **talks #1** copy Mike's link into Mike's source
- Show scene: `Outro`

### In case of problems

In case of problems switch to the last scene `Technical Difficulties`


### In case of stream failure

If a stream fails, the backup director selects the `Technical Difficulties` scene
and then starts streaming.
Recreate the last state from the stream and switch it live.
In case the stream fails during a talk, you can edit the properties of
the video source be double clicking the source.
Deselect the checkbox `Restart playback when source becomes active` and save by clicking `Ok`.
Then you can scrub through the video to the point where the stream failed.


### Live Stream Links

#### Youtube
- ```Talks #1```: https://www.youtube.com/watch?v=BKEy1HEnMZY
- ```Talks #2```: https://www.youtube.com/watch?v=e74TE0b4xEM

#### BOB
- ```Talks #1```: https://bobkonf.de/2022/stream-1.html
- ```Talks #2```: https://bobkonf.de/2022/stream-2.html

#### Backup Video Links
As a backup the videos are already uploaded to YouTube and marked unlisted.

##### Keynote

Keynote is live
 
##### Talks #1

- Michael Sperber - Event Sourcing without Responsibility
  https://www.youtube.com/watch?v=7nDAazdGozY

- Susanne Braun, Annette Bieniusa - Keeping CALM
  https://www.youtube.com/watch?v=rWlsEz19hBs

- Annegret Junker - Event-getriebene Architekturen
  https://www.youtube.com/watch?v=Xq6BD-4xsLs

- Tim Digel - Infrastructure as Code
  https://www.youtube.com/watch?v=8V1-mq-pAC8

- Gernot Strake - Tiger kommt: Weglaufen!
  https://www.youtube.com/watch?v=hW3IxjnHnAs

- Ben Clifford - Python Gradual Typing
  https://www.youtube.com/watch?v=1ssiBVOzCBk

- Ju Liu - An Enigma Machine in Elm
  https://www.youtube.com/watch?v=q7j3QST_n-Q

##### Talks #2

- Markus Schlegel - Composable UI components
  https://www.youtube.com/watch?v=953PB0L5cL4

- Greg Pfeil - Compiling Anything to Categories
  https://www.youtube.com/watch?v=VUBj8NW7uMA

- Philipp Kant - Concurrent programs in Haskell
  https://www.youtube.com/watch?v=uedUGeWN4ZM

- Joachim Breitner - Specification-driven design
  https://www.youtube.com/watch?v=_YyCUiBgEJQ

- Albert Krewinkel - Haskell ❤️ Lua
  https://www.youtube.com/watch?v=Zc07Xxb6FJs

- Laura M Castro, Brujo - Detecting Oxbow Code in Erlang
  https://www.youtube.com/watch?v=ipV8zpAb0y0

- Ragnar Mogk - Local-First Distributed Applications
  https://www.youtube.com/watch?v=6_l1iAGSl4g