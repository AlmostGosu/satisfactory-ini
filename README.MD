CHANGE SETTINGS ON YOUR GAME AT YOUR OWN RISK
I PROVIDE NO SUPPORT AND ASSUME NO RESPONSIBILITY FOR ANYTHING YOU BREAK TRYING THIS

Browse to `%AppData%\..\Local\FactoryGame\Saved\Config\Windowsnoeditor\` and modify your files with ONLY these parameters:

Step 1: Edit your .ini files with the bandwidth settings
Step 2: right click --> Properties --> "read only"
Step 3: change network quality in game to medium
Step 4: change network quality in game to ultra

`Engine.ini`
```[/Script/Engine.Player]
ConfiguredInternetSpeed=104857600
ConfiguredLanSpeed=104857600

[/Script/OnlineSubsystemUtils.IpNetDriver]
MaxClientRate=104857600
MaxInternetClientRate=104857600

[/Script/SocketSubsystemEpic.EpicNetDriver]
MaxClientRate=104857600
MaxInternetClientRate=104857600```

`Game.ini`
```[/Script/Engine.GameNetworkManager]
TotalNetBandwidth=104857600
MaxDynamicBandwidth=104857600
MinDynamicBandwidth=10485760```

`Scalability.ini`
[NetworkQuality@3]
TotalNetBandwidth=104857600
MaxDynamicBandwidth=104857600
MinDynamicBandwidth=10485760

