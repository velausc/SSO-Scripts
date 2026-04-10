# Advanced Commands

A detailed collection of advanced commands for various gameplay features.

---

## Table of Contents  
1. [World Settings](#world-settings)  
2. [Camera Modes](#camera-modes)  
3. [Horse](#horse)  
4. [Environment Settings](#environment-settings)  
5. [Bypass Restrictions](#bypass-restrictions)  
6. [UI](#ui)
7. [Special Horse Appearances](#special-horse-appearances)
8. [Item Spawning](#items-spawning)

---

## World Settings

| **Command**                                     | **Description**          |
|-------------------------------------------------|--------------------------|
| `/World.SetWorldDrawGlobalSpace(0);`            | Xray On                  |
| `/World.SetWorldDrawGlobalSpace(1);`            | Xray Off                 |
| `global/Network.SetNetworkHideSlaves(1);`       | Hides all players        |
| `global/Network.SetNetworkHideSlaves(0);`       | Shows all players        |

---

## Camera Modes 

| **Command**                                                                                                    | **Description**                  |
|----------------------------------------------------------------------------------------------------------------|----------------------------------|
| `global/CutSceneCamera.Start(); global/CutSceneCamera.Move(global/Player); global/CutSceneCamera.SetOrientationByObject(global/Player); global/CutSceneCamera.AddPosition(0, 0.5, -0.5);`                                                               | Switch to first-person mode. |
| `global/Player/Camera.Start();`                                                                               | Restore third-person mode. |
| `global/CutSceneCamera.Start(); global/CutSceneCamera.SetPosition(0, 0, 0);`                                  | Camera Position (change the O, O, O). |

---

## Horse  

| **Command**                                                                                            | **Description**                           |
|--------------------------------------------------------------------------------------------------------|-------------------------------------------|
| `global/Horse.CloneHorseAppearance(0);`                                                                | Modify the horse's appearance (client-side only). |
| `global/HorseForSaleInfoWindow/RenderViews/RenderTargetView/Scene/Animation/Horse.CloneHorse(0, 0); global/HorseForSaleInfoWindow/RenderViews/RenderTargetView/Scene/Animation/Horse.HorseForSaleStartBuyWindow();` | Open the horse purchase window. |
| `global/Button_GlobalHorseStore.Start();`                                                              | Open the global horse store. |
| `global/Horse.HorseRestoreAppearance();`                                                               | Restore the horse's default appearance. |
| `global/Horse/Skin/Pelvis.SetSkinMeshSubsetMaterial("HorseBody", "Horse coat name");`                  | Set horse body and coat appearance. (e.g ("HorseBody", "GH96_Body_04");) |
| `global/Network.NetworkHorseFreeWellbeing();`                                                          | Free horse well being. |
| `global/Player.PlayerTPNetEnterVehicle(global/Horse);`                                                 | Teleports you onto horse. |
| `global/Horse.SetRelativeLinearVelocity(0,10,20);`                                                     | Makes your horse fly. |
| `global/Player.SetScale(0,0,0);`                                                                       | Set scale for horse. |
| `global/ShopManager/Episode1/HorseHairStyleShop1.ShopOpen();`                                          | Open horse stylist shop. |
   
---

## Environment Settings

| **Command**                          | **Description**          |
|--------------------------------------|--------------------------|
| `global/GlobalTimer.SetTimerTime(12);` | Set the day to noon. |
| `global/Player/Pelvis.SetScale(0, 0, 0);` | Set scale for the character. |
| `global/ViewportEffect.SetEnableRainEffect(1);` | Rain effect. |
| `global/MoodManager/Mood_X_X.Start();` | Mood effect. [Check Mood Manager List](#mood-manager-list) |
| `global/World.SetTerrainSnowMode(1);global/ViewportEffect.SetEnableSnowEffect(1);` | Snow effect. |

---

## Bypass Restrictions 

| **Command**                                                              | **Description**                         |
|--------------------------------------------------------------------------|-----------------------------------------|
| `global/ForcePlayerFromRestrictedArea.Delete(); global/ForcePlayerBackToMoorland.Delete(); global/GlobalSpaceObjects/WorldBlockCollsion.Delete();` | Bypass restricted areas. |
| `global/Horse.SetHorseMaxFallTime(99999);`                               | Disable fall damage. |
| `global/SwimActionBar.Delete();`                                         | Disable swimming timer restrictions. |

---

## UI

| **Command**                          | **Description**          |
|--------------------------------------|--------------------------|
| `global/MyStableWindow.Start();`     | Open the wardrobe. |
| `global/MakeupChangeWindow.Start();` | Open the makeup window. |
| `global/HairStyleChangeWindow.Start();` | Open the hairstyle window. |
| `global/PlayerName.SetDataString("xxx");` | Change player's name temporarily. |
| `global/HorseName.SetDataString("xxx");` | Change horse's name temporarily. |
| `global/PlayerStarMoney.SetDataInt(number);` | Change Star Coins amount (client-sided only). |
| `global/Player.SetPlayerTPNetLevel(number);` | Change player's level temporarily. |
| `global/Horse.SetHorseLevel(number);` | Change horse's level temporarily. |
| `global/EmoteWindow.Start(); global/ChatWindow/SmileMenu.Start();` | Emojis Window. |
| `global/Debug_ChampionshipStarterWindow.Start();` | Championship Window. |


---

## Special Horse Appearances  

| **Command**                                                                                           | **Description**      |
|-------------------------------------------------------------------------------------------------------|----------------------|
| `global/Horse.HorseAppearanceCustomBody(1,1,0); global/Horse.HorseAppearanceCustomHair(15,1,0);`      | Old gray deer.       | 
| `global/Horse.HorseAppearanceCustomBody(1,2,0); global/Horse.HorseAppearanceCustomHair(15,1,0);`      | Old white deer.      | 
| `global/Horse.HorseAppearanceCustomBody(1,3,0); global/Horse.HorseAppearanceCustomHair(15,1,0);`      | Old Rudolph deer.    | 
| `global/Horse.HorseAppearanceCustomBody(1,4,0); global/Horse.HorseAppearanceCustomHair(15,1,0);`      | Old brown deer.      | 
| `global/Horse.HorseAppearanceCustomBody(1,1,0); global/Horse.HorseAppearanceCustomHair(20,1,0);`      | Yule goat.           | 
| `global/Horse.HorseAppearanceCustomBody(1,1,0); global/Horse.HorseAppearanceCustomHair(22,1,0);`      | Female deer.         | 
| `global/Horse.HorseAppearanceCustomBody(1,1,0); global/Horse.HorseAppearanceCustomHair(23,1,0);`      | Bear.                | 
| `global/Horse.HorseAppearanceCustomBody(1,1,0); global/Horse.HorseAppearanceCustomHair(24,1,0);`      | Moose.               | 
| `global/Horse.HorseAppearanceCustomBody(10,0,0);`                                                     | Zee.                 | 
| `global/Horse.HorseAppearanceCustomBody(2,-1,0); global/Horse.HorseAppearanceCustomHair(3,-1,0);`     | Easter Coats.        |
| `global/Horse.HorseAppearanceCustomBody(0,0,0); global/Horse.HorseAppearanceCustomHair(35,0,0);`      | Shark.               |

---
## Items Spawning
| **Command**                                                                                           | **Description**      |
|-------------------------------------------------------------------------------------------------------|----------------------|
| `global/QuestManager/Episode1/Chain6004/E01_Quest_L01_C6004_010.QuestComplete(); global/PlayerItemManager/Pet/Pet/CompanionBread_AprilsFools_2018.SetMovable(1);` | April Fool's Bread |

---

## Mood Manager List
Mood_1_HollowWoods
Mood_2_MistyMountains
Mood_3_SnowyMountains
Mood_4_Firgrove
Mood_5_ScarecrowHill
Mood_6_CauldronQuagmire
Mood_7_MagicValley
Mood_8_DevilsGap
Mood_9_GreendaleForest
Mood_10_PandorianAmbience
Mood_11_HiddenDinosaur
Mood_12_Ashland
Mood_13_Volcano
Mood_14_ForgottenFields.Stop
Mood_15_MistyMountains
Mood_16_GreyDewMountainsSecretPath
Mood_17_OldHillcrest
Mood_18_SouthHoofHeath
Mood_19_Mistfall
Mood_20_MistfallCoast
Mood_21_MistfallCoastSwamp
Mood_23_ElisabetsMemorial
Mood_24_GoldenHillsValleyForest
Mood_25_GoldenHillsValleyForest
Mood_26_GoldenHillsValley
Mood_27_AideensWhisper
Mood_28_HussarsDrop
Mood_29_AideensAscent
Mood_30_WildwoodsArea1
Mood_31_WildwoodsArea2
Mood_33_SentinellTreeCorruption
Mood_32_HalloweenTrailRide
Mood_34_WildwoodsMysticsArea
Mood_35_Empty
Mood_36_WildwoodsWarriorsArea
