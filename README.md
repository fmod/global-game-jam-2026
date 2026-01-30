# Audio Team

## FMOD Project setup

### Steps:

1. Log in to www.fmod.com (creating an account is free & only requires an email)
2. Download the latest version of FMOD Studio from https://www.fmod.com/download#fmodstudio
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

- FMOD Studio - Events video - https://www.youtube.com/watch?v=gQFZ4HhoT4A
- FMOD Studio - Parameters video - https://www.youtube.com/watch?v=pp8k3pM7Ies
- FMOD Studio Quick Start tutorial - https://www.fmod.com/docs/2.03/studio/quick-start-tutorial.html
- Getting Started FMOD Basics video playlist - https://www.youtube.com/playlist?list=PLp4vT3ssm5SUgEJpDeA0Nb-1BKGxnDu2m
- FMOD Building Blocks video playlist - https://www.youtube.com/playlist?list=PLp4vT3ssm5SUwiP_T0Yt8ugio5M9di1Em

# Development Team

## Working with Unreal Engine

You can find a detailed breakdown of working with FMOD for Unreal from our integration tutorial here - https://www.youtube.com/watch?v=dgaFfvyTss0

For additional reference, here are the steps you'll need to follow:

1. Log in to www.fmod.com (creating an account is free & only requires an email)
2. Download the FMOD for Unreal integration from https://www.fmod.com/download#fmodforunreal
    Make sure this matches the version that your Audio Team member is using exactly
3. Download the starter .gitignore here & add to your existing .gitignore
4. Add the contents from the FMOD for Unreal zip to your Unreal project - [ProjectName]/Plugins/
5. Add the banks supplied from the Audio Team to [ProjectName]/Content/FMOD/
    Ensure the Platform names are included, for example [ProjectName]/Content/FMOD/Desktop
6. Restart the Unreal editor to have UE generate the required .uassets

### Further documentation:

- FMOD for Unreal User Guide - https://www.fmod.com/docs/2.03/unreal/user-guide.html
- FMOD for Unreal - Making Sounds section - https://www.fmod.com/docs/2.03/unreal/user-guide.html#making-sounds
- FMOD for Unreal - Programming Support - https://www.fmod.com/docs/2.03/unreal/user-guide.html#programming-support
- FMOD for Unreal - API - https://www.fmod.com/docs/2.03/unreal/api-reference.html
- FMOD for Unreal - Blueprint Reference - https://www.fmod.com/docs/2.03/unreal/blueprint-reference.html

## Working with Unity

You can follow our FMOD for Unity tutorial video here - https://www.youtube.com/watch?v=9ehp1aqtDuI

We'll also outline the steps required here for you as well:

1. Log in to www.fmod.com (creating an account is free & only requires an email)
2. Download the FMOD for Unity integration from https://www.fmod.com/download#fmodforunity
    Make sure this matches the version that your Audio Team member is using exactly
3. Download the starter .gitignore here & add to your existing .gitignore
4. Navigate to Package Manager, then import Custom Package and import the contents of the FMOD for Unity zip.
5. Add the banks supplied from the Audio Team to [ProjectName]/Assets/FMOD/
    Ensure the Platform names are included, for example [ProjectName]/Content/FMOD/Desktop
6. Navigate to the FMOD menu in Unity, then Edit Settings & Expand "Bank Import"
7. Set Build Path to the folder you added the Bank files to.
    If you're using Multiple Platform Build, then ensure you point to the folder including the platform names, for eg "[ProjectName]/Content/FMOD/Desktop"

### Further documentation:

- FMOD for Unity User Guide - https://www.fmod.com/docs/2.03/unity/user-guide.html
- FMOD for Unity - Adding Sounds - https://www.fmod.com/docs/2.03/unity/user-guide.html#adding-fmod-studio-content-to-your-unity-project
- FMOD for Unity - Visual Scripting - https://www.fmod.com/docs/2.03/unity/user-guide.html#visual-scripting
- FMOD for Unity - Scripting API - https://www.fmod.com/docs/2.03/unity/api.html.
