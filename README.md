> [!info] **Guide Version: 1.0**, Last Updated: 5/30/2024
> Tested on MacMini M2 2024, Macbook Air M2 2023
> 
> EdenXI Installation Guide Created By: @DungeonGoat
> - Discord: @DungeonGoat:7084
> - Instagram: https://www.instagram.com/dungeongoat/
> - FFXI: Dungeongoat, Hiddenmagik
> - Linkshell: Ragamuffins of Eden
> 	- Discord https://discord.gg/kpNDqZfd

> [!info] EdenXI 
> Website: https://edenxi.com
Discord: https://discord.com/invite/S3EAWr2Jec
## Index
[[#1. EdenXI Files]]
[[#2. Homebrew Install]]
[[#3. Whisky Install]]
[[#4. Whisky Configuration]]
[[#5. EdenXI Installation]]
[[#6. Whisky/EdenXI Pins Setup]]
[[#7. Configure EdenXI Server Hairpin]]
[[#8. EdenXI Window Configuration]]
[[#9. Controller Configuration]]
[[#10. Playing EdenXI]]

---
### 1. EdenXI Files
Go to: https://edenxi.com/install, Download the `Alternative Download` files.
![](_attachments/Pasted image 20240528112218.png|400)

>[!info] Note
![[Pasted image 20240530080436.png|250]]
>This will open a Google Drive download.
>It will download as a .zip. It should auto-unzip.
>You should have `Installer.exe`, and `data.pak` files.
>![[Pasted image 20240530081813.png|350]]
![[Pasted image 20240530081915.png|250]]
### 2. Homebrew Install
Using Terminal: Install Homebrew:  https://brew.sh
``` Terminal
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Press ENTER to continue and agree to the XCode license.
![[Pasted image 20240530084216.png|400]]

>[!Note]
>Homebrew may ask you to accept an XCode license agreement:
>Use this command in the Terminal to accept: 
>``` Terminal
>sudo xcodebuild -license accept
>```

>[!info] Note
>If you already have Homebrew installed, be sure to `brew update`

### 3. Whisky Install
Using Terminal: Install Whisky: https://github.com/Whisky-App/Whisky
``` Terminal
brew install --cask whisky
```

![[Pasted image 20240530084717.png|400]]

Open Whisky with either:
	1. Finder -> Applications -> Whisky
	2. Spotlight: CMD + Space -> type Whisky
![[Pasted image 20240530084811.png|50]]

> [!info] Note
> Click `Open` if this dialogue pops up.
![[Pasted image 20240530084936.png|150]]

Click Next to install dependencies.
![[Pasted image 20240530085310.png|400]]

### 4. Whisky Configuration
1. Click Create Bottle
![[Pasted image 20240530085604.png|400]]

2. Set the follow settings, then press Create. This may take a while to complete.
Bottle Name: EdenXI
Windows Version: Windows 10
Bottle Path: Leave as default
![[Pasted image 20240530085637.png|400]]

3. Click Winetricks
![[Pasted image 20240530085827.png|400]]

4. Click DLLs -> `dotnet40` -> Run
![[Pasted image 20240530090032.png|400]]

Allow if asked.
![[Pasted image 20240530090102.png|150]]

Check the ToS and Install. This may come up a few times and takes a while to complete.
![[Pasted image 20240530090149.png|250]]
![[Pasted image 20240530090409.png|250]]

### 5. EdenXI Installation
Click Run -> Select Installer.exe from the EdenXI download.
![[Screenshot 2024-05-30 at 10.03.28 AM.png|400]]

Allow if asked.
![[Pasted image 20240530100827.png|150]]

Click Continue on the Eden Installer.
![[Pasted image 20240530100857.png|250]]

Accept the ToS
![[Pasted image 20240530100923.png|250]]

You will see popups as it verifies the dotnet runtime.
![[Pasted image 20240530100937.png|250]]

This may take a while.
![[Pasted image 20240530101208.png|250]]

It should auto-progress to the Install Location when dotnet is done.
Leave the installation at `C:\Eden`, click Install
![[Pasted image 20240530112048.png|350]]

Wait for the installer to finish
![[Pasted image 20240530101512.png|250]]

Click Finish
![[Pasted image 20240530102205.png|400]]

Verify your folder structure has `Eden` at the root of C:\
![[Pasted image 20240530113152.png|400]]
### 6. Whisky/EdenXI Pins Setup
> [!info] Note: If you see Ashita pinned, right click and Unpin it.
![[Pasted image 20240530102249.png|250]]

1. Create `Config` Pin
Click the + button to create a new pin called `Config`
Click Browse and navigate to `Eden/Square Enix/FINAL FANTASY XI/ToolsUS/FINAL FANTASY XI Config.exe`
Click Pin to confirm.
![[Screenshot 2024-05-30 at 10.24.16 AM.png|400]]

2. Create `Controller Config` pint
Click the + button to create a new pin called `Controller Config`
Click Browse and navigate to `Eden/Square Enix/FINAL FANTASY XI/ToolsUS/FINAL FFXiPadConfig.exe`
Click Pin to confirm.
![[Pasted image 20240530102809.png|250]]

3. Create the `EdenXI` game launcher pin
Click the + button to create a new pin called `EdenXI`
Click Browse and navigate to `Eden/Ashita/ffxi-bootmod/xiloader.exe`
Click Pin to confirm.
![[Pasted image 20240530103015.png|400]]

Click the Refresh symbol to refresh the Whisky UI and show the icons. You should have the these 3.
![[Pasted image 20240530103305.png|400]]

### 7. Configure EdenXI Server Hairpin

Right click the `EdenXI` pin and click `Config` 
![[Pasted image 20240530103358.png|150]]

Add to the arguments: `--server play.edenxi.com --hairpin`
(This tells the launcher to connect to the EdenXI server)
Then click the Back Arrow.
![[Pasted image 20240530103437.png|250]]

### 8. EdenXI Window Configuration

Right click and Run the pinned Config
![[Pasted image 20240530103625.png|150]]

Change the window mode to `Windowed mode`
> [!info] Note: Full Screen mode is not supported.

![[Pasted image 20240530103653.png|250]]

Adjust screen size as desired in the Screen Size tab.
![[Pasted image 20240530112623.png|250]]

Click OK and say Yes to save the settings.
![[Pasted image 20240530103752.png|250]]

### 9. Controller Configuration
Right Click > Run the Controller Config pin
![[Pasted image 20240530115955.png|150]]

Check the Enable Gamepad box
![[Pasted image 20240530120101.png|400]]

Click Test Gamepad and confirm your controller works.
Click OK and save changes.

![[Pasted image 20240530120207.png|400]]
### 10. Playing EdenXI
1. Right Click the EdenXI pin and click Run
![[Pasted image 20240530103855.png|100]]

The Terminal will open with some options.
If you see this, you're on the right path. Otherwise, you messed up somewhere.
![[Pasted image 20240530103932.png|400]]

2. Select to create an account or login.

Once logged in the game will launch:
![[Pasted image 20240530112729.png|400]]

> [!info] Note: The audio may be janky.