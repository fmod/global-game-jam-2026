---
title: Working with Unity
layout: default
parent: Development Team
nav_order: 3.1
---
# Working with Unity

You can follow our [FMOD for Unity tutorial video](https://www.youtube.com/watch?v=9ehp1aqtDuI)

We'll also outline the steps required here for you as well:

### Setting up Source Control

First, make sure your version control has the correct ignores set up:
- [Github Setup](https://ggj.fmod.com/docs/Development/Unity/working-with-unity.html#git-ignore-setup) <br>
- [SVN Setup](https://ggj.fmod.com/docs/Development/Unity/working-with-unity.html#svn-ignore-setup)

## Getting the Integration

There are two options when grabbing the FMOD integration:

### Using Unity Package Manager

1. Through the Unity Package Manager:
    - Add the Unity Integration to your Unity Account:
        [Version 2.2](https://assetstore.unity.com/packages/tools/audio/fmod-for-unity-2-02-161631)
        [Version 2.3](https://assetstore.unity.com/packages/tools/audio/fmod-for-unity-2-03-311497)
    - In the Unity Editor
    - Open the Package Manager
        ![Unity Package Manager Open](/assets/Unity/PackageManagerUnity.png)
    - In `My Assets` search for `FMOD for Unity`
    - Add your desired Major version
        ![FMOD for Unity](/assets/Unity/FMODinPM.png)

Or

### Directly from FMOD Downloads

1.  Log in to [www.fmod.com](https://fmod.com) (creating an account is free & only requires an email)
2.  Head to [FMOD Downloads](https://www.fmod.com/download#unity) to download specific sub versions if required.
3.  Navigate to Package Manager, then import Custom Package and import the contents of the FMOD for Unity zip.

## Setting up the Integration

1. Add the banks supplied from the Audio Team to [ProjectName]/Assets/FMOD/ <br> Ensure the Platform names are included, for example [ProjectName]/Content/FMOD/Desktop
2. Navigate to the FMOD menu in Unity, then Edit Settings & Expand "Bank Import"
3. Set Build Path to the folder you added the Bank files to. <br> If you're using Multiple Platform Build, then ensure you point to the folder including the platform names, for eg "[ProjectName]/Content/FMOD/Desktop"

### Note:
If you have devs working on different operating systems, we suggest adding a `.gitattributes` to avoid issues:

```
Assets/Plugins/FMOD/**/*.bundle text eol=lf
Assets/Plugins/FMOD/**/Info.plist text eol=lf
```

## Version Control Ignore Setup

## Git Ignore Setup

add our [starter ignore](unity-ignore.html) to your repositories `.gitignore`

## SVN Ignore setup

If using SVN, you'll need to grab the [fmod_unity_svn_ignore.txt](fmod-for-unity-svn-ignore.html) file, put it in your project's parent folder and run the following commands from that same folder:
```
svn propset svn:ignore -F fmod_unity_svn_ignore.txt Assets/Plugins/FMOD
svn propset svn:ignore -F fmod_unity_svn_ignore.txt Assets/StreamingAssets
```

# Further documentation:

- [FMOD for Unity User Guide](https://www.fmod.com/docs/2.03/unity/user-guide.html)
- [FMOD for Unity - Adding Sounds](https://www.fmod.com/docs/2.03/unity/user-guide.html#adding-fmod-studio-content-to-your-unity-project)
- [FMOD for Unity - Visual Scripting](https://www.fmod.com/docs/2.03/unity/user-guide.html#visual-scripting)
- [FMOD for Unity - Scripting API](https://www.fmod.com/docs/2.03/unity/api.html)
