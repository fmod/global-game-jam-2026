---
title: FMOD Project Setup
layout: default
parent: Audio Team
nav_order: 2.1
---
# FMOD Project setup

## Steps:

1. Log in to [www.fmod.com](https://fmod.com) (creating an account is free & only requires an email)
2. Download the latest version of FMOD Studio from our [Downloads Page](https://www.fmod.com/download#fmodstudio)
    Latest version is 2.03.12 currently
3. Install FMOD Studio, open & create a new project.
4. Save your project in a dedicated folder per game project
    For eg, GGJ/GameName1/FMOD Project
5. Add any assets you have & create your events (see tutorials & documentation links below)

## Delivering sounds to the Development Team

1. When finished, build your project using Ctrl / Cmd + F7 to build all platforms
2. There will now be a "Build" folder under your FMOD Project folder containing Bank files.
    For eg, GGJ/GameName1/FMOD Project/Build
3. Deliver the folders inside this Build folder to your development team
    Note: The Development Team doesn't require the full FMOD Studio project, only the files in the Build folder.
4. Any time you make changes to your FMOD Studio project or add new sounds or events, you just need to press Ctrl / Cmd + F7 and send the Development Team the updated Bank files each time.

## If you're using Source Control

If you've been added to your Development Team's source control, you only need to push your Bank files.

To do this, you just need to go to Edit - Preferences, switch to the Build tab and set your "Built banks output directory" to one of the following:

For Unity, set it to `[ProjectName]/Assets/FMOD`

For Unreal, set it to `[ProjectName]/Content/FMOD`

If you can't see those locations, find one of the FMOD support crew & we'll help you out!

### Further Documentation

- [FMOD Studio - Events video](https://www.youtube.com/watch?v=gQFZ4HhoT4A)
- [FMOD Studio - Parameters video](https://www.youtube.com/watch?v=pp8k3pM7Ies)
- [FMOD Studio Quick Start tutorial](https://www.fmod.com/docs/2.03/studio/quick-start-tutorial.html)
- [Getting Started FMOD Basics video playlist](https://www.youtube.com/playlist?list=PLp4vT3ssm5SUgEJpDeA0Nb-1BKGxnDu2m)
- [FMOD Building Blocks video playlist](https://www.youtube.com/playlist?list=PLp4vT3ssm5SUwiP_T0Yt8ugio5M9di1Em)