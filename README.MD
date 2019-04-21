# Multiplayer bandwidth fix settings for Satisfactory

## Important notes before you get started
I've provided my full .ini files as a reference. __**DO NOT**__ copy my .ini files over your own. Only change the settings provided below in your own.

## The process
* Step 0: Understand that you assume all risk for anything you break on your system making these changes
* Step 1: Open explorer or a run bar and paste this in the text field `%AppData%\..\Local\FactoryGame\Saved\Config\Windowsnoeditor\`
* Step 2: Make a copy of all your original files and move them somewhere safe
* Step 3: Edit your .ini files with the items listed in reference changes
* Step 4: For each file edited, right click --> Properties --> check the box for "read only"
* Step 5: change network quality in game to medium
* Step 6: change network quality in game to ultra

## Reference changes
```
# Engine.ini
[/Script/Engine.Player]
ConfiguredInternetSpeed=104857600
ConfiguredLanSpeed=104857600

[/Script/OnlineSubsystemUtils.IpNetDriver]
MaxClientRate=104857600
MaxInternetClientRate=104857600

[/Script/SocketSubsystemEpic.EpicNetDriver]
MaxClientRate=104857600
MaxInternetClientRate=104857600 ```

# Game.ini
[/Script/Engine.GameNetworkManager]
TotalNetBandwidth=104857600
MaxDynamicBandwidth=104857600
MinDynamicBandwidth=10485760

# Scalability.ini

[NetworkQuality@3]
TotalNetBandwidth=104857600
MaxDynamicBandwidth=104857600
MinDynamicBandwidth=10485760
```

