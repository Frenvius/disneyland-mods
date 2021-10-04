Injects skills into Valheim's skill system. Handles adding to the list and both the cheat options (Raise/Reset). Leaves you to handle getting XP and actually applying effects.  You will need to pick a unique number for your skill id. I'd stick with numbers > 200.

Usage:
```
    ﻿[BepInDependency("com.pipakin.SkillInjectorMod")]
    public class MySkillMod: BaseUnityPlugin
    {
        const int SKILL_TYPE = 299;
        ﻿...

        void Awake()
        ﻿﻿{
        ﻿SkillInjector.RegisterNewSkill(SKILL_TYPE, "MyCoolSkill", "Doing Cool Stuff", 1.0f, null, Skills.SkillType.Unarmed);
        ﻿﻿}

        ...
    ﻿}
```

the parameters are:

* `id` - the numeric id for your skill. MUST BE UNIQUE.
* `name` - the name of your skill.
* `description` - the description of your skill.
* `increment` - the increment to adjust your skill by when increasing.
* `icon` - the icon for your skill (Unity Sprite). Can be null if you use a template skill to base your icon on.
* `template` - the skill to copy the icon from if you don't provide an icon.


Known issues:
* Doesn't support multiple languages for the skill name (working on it).

Github link:
https://github.com/pipakin/PipakinsMods/tree/master/SkillInjector


All my mod code on GitHub: https://github.com/pipakin/PipakinsMods