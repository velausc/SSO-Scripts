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

---

## World Settings

| **Command**                                     | **Description**          |
|-------------------------------------------------|--------------------------|
| `/World.SetWorldDrawGlobalSpace(0);`            | Xray On                  |
| `/World.SetWorldDrawGlobalSpace(1);`            | Xray Off                 |

---

## Camera Modes 

| **Command**                                                                                                    | **Description**                  |
|----------------------------------------------------------------------------------------------------------------|----------------------------------|
| `global/CutSceneCamera.Start(); global/CutSceneCamera.Move(global/Player); global/CutSceneCamera.SetOrientationByObject(global/Player); global/CutSceneCamera.AddPosition(0, 0.5, -0.5);` | Switch to first-person mode. |
| `global/Player/Camera.Start();`                                                                               | Restore third-person mode. |

---

## Horse  

| **Command**                                                                                            | **Description**                           |
|--------------------------------------------------------------------------------------------------------|-------------------------------------------|
| `global/Horse.CloneHorseAppearance(0);`                                                                | Modify the horse's appearance (client-side only). |
| `global/HorseForSaleInfoWindow/RenderViews/RenderTargetView/Scene/Animation/Horse.CloneHorse(0, 0); global/HorseForSaleInfoWindow/RenderViews/RenderTargetView/Scene/Animation/Horse.HorseForSaleStartBuyWindow();` | Open the horse purchase window. |
| `global/Horse.HorseRestoreAppearance();`                                                               | Restore the horse's default appearance. |
| `global/Horse/Skin/Pelvis.SetSkinMeshSubsetMaterial("HorseBody", "horse coat name");`                  | Set horse body and coat appearance. |
| `global/Network.NetworkHorseFreeWellbeing();`                                                          | Free horse well being. |

---

## Environment Settings

| **Command**                          | **Description**          |
|--------------------------------------|--------------------------|
| `global/GlobalTimer.SetTimerTime(12);` | Set the day to noon. |

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

---
