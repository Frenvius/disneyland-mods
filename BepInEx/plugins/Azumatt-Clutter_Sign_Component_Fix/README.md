# Description

## Meant to fix the issue with the Sign Component used on the Diaries used in the Clutter mod. This mod is meant to be used with the Clutter mod, but might also fix other signs that are old.


`This mod is not needed on a server. It's client only. Install on each client that you wish to have the mod load.`

### Why is this needed?
Due to the older assets that Clutter uses, the mod is not compatible with the newer TextMeshProUGUI component, thus, causing crashes when using a mod like AzuSigns or ComfySigns that utilize the new component. This mod fixes that issue by converting the old Text component to the newer TextMeshProUGUI component at runtime.


### How this mod works (Technical Explanation)

The purpose of this mod is to convert the old Text component in the Sign class to the newer TextMeshProUGUI component at runtime, ensuring compatibility with the updated script.

Code for this mod can be found here: https://github.com/AzumattDev/ClutterTempFix

Here's a step-by-step explanation of the patch the mod uses to achieve this:
1. The Prefix method is executed before the original Awake method of the Sign class.

2. The oldTextGameObject is found by searching for a child object named "Text" within the Sign instance.

3. If the oldTextGameObject is found, the script checks if it has a Text component (the old component type).

4. If the Text component is present, a new GameObject named "Text" is created to hold the TextMeshProUGUI component.

5. The new GameObject's parent, local position, local rotation, and local scale are set to match the original oldTextGameObject.

6. The TextMeshProUGUI component is added to the new GameObject, and its properties (such as text, font, font size, color, and alignment) are set to match the original Text component.

7. The m_textWidget field in the Sign class is updated to reference the new TextMeshProUGUI component.

8. The old Text component is removed by destroying its GameObject.

9. The Postfix method is executed after the original Awake method of the Sign class.

10. In the Postfix method, the Sign script is re-enabled if it was disabled for any reason during the process. During my testing this was the case under certain circumstances, but it may not be the case for everyone.

By following these steps, the mod ensures that the old Text component is replaced with the newer TextMeshProUGUI component at runtime, maintaining compatibility with the updated script.

`Feel free to reach out to me on discord if you need manual download assistance.`


# Author Information

### Azumatt

`DISCORD:` Azumatt#2625

`STEAM:` https://steamcommunity.com/id/azumatt/

For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>
***

> # Update Information (Latest listed first)

| `Version` | `Update Notes`    |
|-----------|-------------------|
| 1.0.0     | - Initial Release |