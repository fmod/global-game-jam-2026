---
title: Working with Unreal Engine
layout: default
parent: Development Team
nav_order: 3.2
---
# Working with Unreal Engine

You can find a detailed breakdown of working with [FMOD for Unreal from our integration tutorial](https://www.youtube.com/watch?v=dgaFfvyTss0)

For additional reference, here are the steps you'll need to follow:

1. Log in to [www.fmod.com](https://fmod.com) (creating an account is free & only requires an email)
2. Download the FMOD for Unreal integration from [Downloads Page](https://www.fmod.com/download#fmodforunreal). Make sure this matches the version that your Audio Team member is using exactly
3. Before adding the integration, add our [starter ignore](unreal-ignore.html) to your repositories `.gitignore`
4. Add the contents from the FMOD for Unreal zip to your Unreal project - [ProjectName]/Plugins/
5. Add the banks supplied from the Audio Team to [ProjectName]/Content/FMOD/. <br> Ensure the Platform names are included, for example [ProjectName]/Content/FMOD/Desktop
6. Restart the Unreal editor to have UE generate the required .uassets

## Further documentation:

- [FMOD for Unreal User Guide](https://www.fmod.com/docs/2.03/unreal/user-guide.html)
- [FMOD for Unreal - Making Sounds section](https://www.fmod.com/docs/2.03/unreal/user-guide.html#making-sounds)
- [FMOD for Unreal - Programming Support](https://www.fmod.com/docs/2.03/unreal/user-guide.html#programming-support)
- [FMOD for Unreal - API](https://www.fmod.com/docs/2.03/unreal/api-reference.html)
- [FMOD for Unreal - Blueprint Reference](https://www.fmod.com/docs/2.03/unreal/blueprint-reference.html)
