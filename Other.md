/World.SetWorldDrawGlobalSpace(0); - Xray
/World.SetWorldDrawGlobalSpace(1); - Xray
global/CutSceneCamera.Start();global/CutSceneCamera.Move(global/Player);global/CutSceneCamera.SetOrientationByObject(global/Player);global/CutSceneCamera.AddPosition(0, 0.5, -0.5); - First person
global/Player/Camera.Start(); - Restore third person
global/Horse.CloneHorseAppearance(0); - Clientside horse appearance
global/HorseForSaleInfoWindow/RenderViews/RenderTargetView/Scene/Animation/Horse.CloneHorse(0, 0);global/HorseForSaleInfoWindow/RenderViews/RenderTargetView/Scene/Animation/Horse.HorseForSaleStartBuyWindow(); -Horse buy window
global/Horse.HorseRestoreAppearance(); - Restore horse appearance
global/GlobalTimer.SetTimerTime(12); - Day time
global/ForcePlayerFromRestrictedArea.Delete();global/ForcePlayerBackToMoorland.Delete();global/GlobalSpaceObjects/WorldBlockCollsion.Delete(); - Bypass restricted area
global/Horse.SetHorseMaxFallTime(99999); - Bypass fall damage
global/SwimActionBar.Delete(); - Bypass swim timer
global/Network.NetworkHorseFreeWellbeing(); - Horse care
global/MyStableWindow.Start(); - Open wardrobe
global/MakeupChangeWindow.Start(); - Open makeup window
global/HairStyleChangeWindow.Start(); - Open hairstyle window
