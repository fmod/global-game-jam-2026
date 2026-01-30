---
title: Working with Unreal Engine
layout: default
parent: Development Team
nav_order: 3.2
---
# Working with Unreal Engine

You can find a detailed breakdown of working with [FMOD for Unreal from our integration tutorial](https://www.youtube.com/watch?v=dgaFfvyTss0)

For additional reference, here are the steps you'll need to follow:

### Setting up Source Control

First, make sure your version control has the correct ignores set up:
- [Github Setup](https://ggj.fmod.com/docs/Development/Unreal/working-with-unreal.html#git-ignore-setup) <br>
- [SVN Setup](https://ggj.fmod.com/docs/Development/Unreal/working-with-unreal.html#svn-ignore-setup)

## Installing the Integration

1. Log in to [www.fmod.com](https://fmod.com) (creating an account is free & only requires an email)
2. Download the FMOD for Unreal integration from [Downloads Page](https://www.fmod.com/download#fmodforunreal). <br> *Make sure this matches the version of FMOD Studio that your Audio Team member is using*
3. Add the contents from the FMOD for Unreal zip to your Unreal project - [ProjectName]/Plugins/
4. Add the banks supplied from the Audio Team to [ProjectName]/Content/FMOD/. <br> *Ensure the Platform names are included, for example [ProjectName]/Content/FMOD/Desktop*
5. Restart the Unreal editor to have UE generate the required .uassets

## Git Ignore Setup

4. Add our [starter ignore](unreal-ignore.html) to your repository's `.gitignore`

*Keep in mind `.gitignore` files use a "Last Match Wins" heirarchy, so ensure our starter ignore entries are added at the bottom of your existing `.gitignore`.*


## SVN Ignore Setup

If using SVN, you'll need to download the [fmod_unreal_svn_ignore.txt](fmod-unreal-svn-ignore.html) file, put it in your project's parent folder and run the following commands from that same folder:
```
svn propset svn:ignore -F fmod_unreal_svn_ignore.txt Content/FMOD
svn propset svn:ignore -F fmod_unreal_svn_ignore.txt "FMOD Project"
```

# Further documentation:

## Videos

- [FMOD for Unreal from our integration tutorial](https://www.youtube.com/watch?v=dgaFfvyTss0)

## Documentation

- [FMOD for Unreal User Guide](https://www.fmod.com/docs/2.03/unreal/user-guide.html)
- [FMOD for Unreal - Making Sounds section](https://www.fmod.com/docs/2.03/unreal/user-guide.html#making-sounds)
- [FMOD for Unreal - Programming Support](https://www.fmod.com/docs/2.03/unreal/user-guide.html#programming-support)
- [FMOD for Unreal - API](https://www.fmod.com/docs/2.03/unreal/api-reference.html)
- [FMOD for Unreal - Blueprint Reference](https://www.fmod.com/docs/2.03/unreal/blueprint-reference.html)
