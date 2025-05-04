## .:[ Join Our Discord For Support ]:.

<a href="https://discord.com/invite/U7AuQhu"><img src="https://discord.com/api/guilds/651838917687115806/widget.png?style=banner2"></a>

***
# [CS2] Kill-Sound-GoldKingZ (1.1.2)

### Kill Sound ( Kill , HeadShot , Quake )


![111111](https://github.com/oqyh/cs2-Kill-Sound-GoldKingZ/assets/48490385/327651ba-feda-47a8-88b7-2f928d8df206)


![configs](https://github.com/oqyh/cs2-Kill-Sound-GoldKingZ/assets/48490385/3c08cec9-6e29-4c00-8d74-bc9ae3cf4f85)


## .:[ Dependencies ]:.
[Metamod:Source (2.x)](https://www.sourcemm.net/downloads.php/?branch=master)

[CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp/releases)

[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json)

[MySqlConnector](https://www.nuget.org/packages/MySqlConnector)

## .:[ Configuration ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Kill-Sound-GoldKingZ\config\config.json                                           
>

> [!NOTE]
> To Use Modify Version And Lower Volume                                                                                                                              
> Download https://github.com/Source2ZE/MultiAddonManager  With Gold KingZ WorkShop                                                                                                                             
> https://steamcommunity.com/sharedfiles/filedetails/?id=3230015783                                                                                                                             
> mm_extra_addons 3230015783                                                                                                                             
> OtherWise Use Normal Sounds https://github.com/oqyh/cs2-Kill-Sound-GoldKingZ/blob/main/sounds/sounds.txt                                                                                                                              

```json
{
  //Enable Kill_Settings.json?
  "KS_EnableQuakeSounds": false,

  //If KS_EnableQuakeSounds Enabled Do You Like To Disable Quake Sounds On WarmUp?
  "KS_DisableQuakeSoundsOnWarmUp": true,

  //If KS_EnableQuakeSounds Do You Like To Reset Kill Streaks On Every Round?
  "KS_ResetKillStreakOnEveryRound": true,

  //Enable MySql MySql_Settings.json?
  "KS_UseMySql": false,
//-----------------------------------------------------------------------------------

  //Do You Like To Add Freeze On Open Menu Option In The Menu?
  "KS_AddMenu_FreezeOnOpenMenu": true,

  //Do You Like To Add Sound HeadShot Kill Option In The Menu? (To Disable Make It Empty Like This "")
  "KS_AddMenu_HeadShotKillSoundPath": "sounds/GoldKingZ/Training/bell_normal.vsnd_c",

  //Do You Like To Add Sound BodyShot Kill Option In The Menu? (To Disable Make It Empty Like This "")
  "KS_AddMenu_BodyKillSoundPath": "sounds/GoldKingZ/Training/timer_bell.vsnd_c",

  //Do You Like To Add Sound HeadShot Hit Option In The Menu? (To Disable Make It Empty Like This "")
  "KS_AddMenu_HeadShotHitSoundPath": "sounds/GoldKingZ/Training/bell_impact.vsnd_c",

  //Do You Like To Add Sound BodyShot Hit Option In The Menu? (To Disable Make It Empty Like This "")
  "KS_AddMenu_BodyHitSoundPath": "sounds/GoldKingZ/Training/timer_bell.vsnd_c",

  //Do You Like To Add Quake Sounds Toggle Option In The Menu?
  "KS_AddMenu_QuakeSoundsToggle": true,

  //Do You Like To Add Quake Center Message Toggle Option In The Menu?
  "KS_AddMenu_QuakeCenterMessageToggle": true,

  //Do You Like To Add Quake Chat Message Toggle Option In The Menu?
  "KS_AddMenu_QuakeChatMessageToggle": true,

//-----------------------------------------------------------------------------------
  //Default Value Of FreezeOnOpenMenu
  "KS_DefaultValue_FreezeOnOpenMenu": true,

  //Default Value Of HeadShotKillSound
  "KS_DefaultValue_HeadShotKillSound": true,

  //Default Value Of BodyKillSound
  "KS_DefaultValue_BodyKillSound": false,

  //Default Value Of HeadShotHitSound
  "KS_DefaultValue_HeadShotHitSound": false,

  //Default Value Of BodyHitSound
  "KS_DefaultValue_BodyHitSound": false,

  //Commands In Game To Open Sound Menu
  "KS_InGameMenu": "!soundmenu,!soundsmenu,!menusound,!menusounds",

  //Only Allow These Groups To Have Access To KS_InGameMenu (Making Empty "" Means Everyone Has Access) [ex of groups: "@css/root,@css/admin,#css/admin"]
  "KS_OnlyAllowTheseGroupsToToggle": "",

  //Auto Delete Inactive Players Cookies Older Than X Days plugins/Kill-Sound-GoldKingZ/Cookies/Kill_Sound_Cookies.json
  "KS_AutoRemovePlayerCookieOlderThanXDays": 7,
}
```


## .:[ Configuration Quake ]:.

> [!CAUTION]
> Config Located In ..\addons\counterstrikesharp\plugins\Kill-Sound-GoldKingZ\config\Kill_Settings.json                                           
>

> [!NOTE]
> To Use These You Need To Enable KS_EnableQuakeSounds First In config.json                                                                                                                               
> Then Download https://github.com/Source2ZE/MultiAddonManager  With Gold KingZ WorkShop                                                                                                                              
> https://steamcommunity.com/sharedfiles/filedetails/?id=3230015783                                                                                                                             
> mm_extra_addons 3230015783                                                                                                                        
> You Can Find WorkShop Path Sound In   https://github.com/oqyh/cs2-Kill-Sound-GoldKingZ/blob/main/sounds/Gold%20KingZ%20WorkShop%20Sounds.txt                                                                                                                          
                                                                                                                       
```
	Available Sounds [ "HeadShot" , "Kill" , "KnifeKill" , "TaserKill" , "GrenadeKill" , "MollyKill" , "SelfKill" , "TeamKill" , "FirstBlood" , "RoundPrepare" , "RoundStart" ]
	
	HeadShot Can Be Used 
	HeadShot = Will Start Sound Loop On Every HeadShot Kill
	HeadShot_X = Will Start Sound Depend Kill X HeadShot Kill

	Kill Can Be Used 
	Kill = Will Start Sound Loop On Every Normal Kill
	Kill_X = Will Start Sound Depend Kill X Normal Kill

	KnifeKill Can Be Used 
	KnifeKill = Will Start Sound Loop On Every Knife Kill
	KnifeKill_X = Will Start Sound Depend Kill X Knife Kill

	TaserKill Can Be Used 
	TaserKill = Will Start Sound Loop On Every Taser Kill
	TaserKill_X = Will Start Sound Depend Kill X Taser Kill

	GrenadeKill Can Be Used 
	GrenadeKill = Will Start Sound Loop On Every Grenade Kill
	GrenadeKill_X = Will Start Sound Depend Kill X Grenade Kill

	MollyKill Can Be Used 
	MollyKill = Will Start Sound Loop On Every Molotov Kill
	MollyKill_X = Will Start Sound Depend Kill X Molotov Kill

"Announcement": These Only Can Be Controlled On/Off [ "HeadShot" , "Kill" , "KnifeKill" , "TaserKill" , "GrenadeKill" , "MollyKill" , "SelfKill" , "TeamKill" , "FirstBlood" ]

You Cannot Control ["RoundPrepare" , "RoundStart" ] Becasue Its Already Announce You Cant Turn It Off

```


![colors](https://github.com/oqyh/cs2-Kill-Sound/assets/48490385/6c0717b0-0a7e-45c3-ab7e-cd164ee74aae)



## .:[ Language ]:.
```json
{
    //==========================
    //        Colors
    //==========================
    //{Yellow} {Gold} {Silver} {Blue} {DarkBlue} {BlueGrey} {Magenta} {LightRed}
    //{LightBlue} {Olive} {Lime} {Red} {Purple} {Grey}
    //{Default} {White} {Darkred} {Green} {LightYellow}
    //==========================
    //        Other
    //==========================
    //<br> = Next Line On Center Hud 
    //{nextline} = Print On Next Line
    //==========================
	
	
	"player.not.allowed": "{green}Gold KingZ {grey}| {darkred}Toggle Sounds Menu Is For {lime}VIPS {darkred}Only",

	"player.toggle.freeze.on": "{green}Gold KingZ {grey}| {grey}Freeze On Menu Open Is {lime}On",
	"player.toggle.freeze.off": "{green}Gold KingZ {grey}| {grey}Freeze On Menu Open Is {darkred}Off",

	"player.toggle.bodykill.on": "{green}Gold KingZ {grey}| {grey}Body Kill Sound Is {lime}On",
	"player.toggle.bodykill.off": "{green}Gold KingZ {grey}| {grey}Body Kill Sound Is {darkred}Off",

	"player.toggle.bodyhit.on": "{green}Gold KingZ {grey}| {grey}Body Hit Sound Is {lime}On",
	"player.toggle.bodyhit.off": "{green}Gold KingZ {grey}| {grey}Body Hit Sound Is {darkred}Off",

	"player.toggle.headshotkill.on": "{green}Gold KingZ {grey}| {grey}HeadShot Kill Sound Is {lime}On",
	"player.toggle.headshotkill.off": "{green}Gold KingZ {grey}| {grey}HeadShot Kill Sound Is {darkred}Off",

	"player.toggle.headshothit.on": "{green}Gold KingZ {grey}| {grey}HeadShot Hit Sound Is {lime}On",
	"player.toggle.headshothit.off": "{green}Gold KingZ {grey}| {grey}HeadShot Hit Sound Is {darkred}Off",

	"player.toggle.quake.sounds.on": "{green}Gold KingZ {grey}| {grey}Quake Sounds Is {lime}On",
	"player.toggle.quake.sounds.off": "{green}Gold KingZ {grey}| {grey}Quake Sounds Is {darkred}Off",

	"player.toggle.quake.center.message.on": "{green}Gold KingZ {grey}| {grey}Quake Center Messages Is {lime}On",
	"player.toggle.quake.center.message.off": "{green}Gold KingZ {grey}| {grey}Quake Center Messages Is {darkred}Off",

	"player.toggle.quake.chat.message.on": "{green}Gold KingZ {grey}| {grey}Quake Chat Messages Is {lime}On",
	"player.toggle.quake.chat.message.off": "{green}Gold KingZ {grey}| {grey}Quake Chat Messages Is {darkred}Off",

//--------------------------------------------------------------------------------------------------------------------------------------------------------------------------//

	"chat.announce.quake.headshot.streak.5": "{green}Gold KingZ {grey}| {purple}{0} {grey}IS HEAD HUNTER!!! Got {yellow}{1} {grey}HeadShot Streak!",
	"center.announce.quake.headshot.streak.5": "<font color='purple'>{0} <font color='white'>IS HEAD HUNTER!!! Got <font color='yellow'>{1} <font color='white'>HeadShot Streak! </font>",
	
	"chat.announce.quake.kill.streak.4": "{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.4": "<font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.6": "{green}Gold KingZ {grey}| {red}Rampage  {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.6": "<font color='red'>Rampage <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.8": "{green}Gold KingZ {grey}| {red}Killing Spree {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.8": "<font color='red'>Killing Spree <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.10": "{green}Gold KingZ {grey}| {red}Monster Kill {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.10": "<font color='red'>Monster Kill <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.14": "{green}Gold KingZ {grey}| {red}Unstoppable ! {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.14": "<font color='red'>Unstoppable! <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.16": "{green}Gold KingZ {grey}| {red}Ultrakill ! {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.16": "<font color='red'>Ultrakill! <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.18": "{green}Gold KingZ {grey}| {red}Godlike !!! {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.18": "<font color='red'>Godlike!!! <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.20": "{green}Gold KingZ {grey}| {red}WickedSick !!! {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.20": "<font color='red'>WickedSick !!! <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.24": "{green}Gold KingZ {grey}| {red}Ludicrous Kill !!! {nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}",
	"center.announce.quake.kill.streak.24": "<font color='red'>Ludicrous Kill !!! <br><font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.kill.streak.26": "{green}Gold KingZ {grey}| {red}-------------------------------{nextline}{green}Gold KingZ {grey}| {blue}H {red}O {yellow}L {purple}Y {lime}S {darkred}H {darkblue}I {gold}T {blue}!!!!!!!!!!{nextline}{green}Gold KingZ {grey}| {purple}{0} {grey}On Kill Streak {yellow}{1}{nextline}{green}Gold KingZ {grey}| {red}-------------------------------",
	"center.announce.quake.kill.streak.26": "<font color='red'>-------------------------------<br><font color='blue'>H <font color='red'>O <font color='yellow'>L <font color='pink'>Y <font color='lime'>S <font color='darkred'>H <font color='darkblue'>I <font color='gold'>T <font color='blue'>!!!!!!!!!!<br>{green} <font color='purple'>{0} <font color='white'>On Kill Streak <font color='yellow'>{1}<br><font color='red'>------------------------------- </font>",
	
	
	"chat.announce.quake.knife": "{green}Gold KingZ {grey}| HAHAHA {purple}{0} {grey} Knifed {yellow}{1}",
	"center.announce.quake.knife": "<font color='white'> H A H A H A <br> <font color='purple'>{0} <font color='white'>Knifed  <font color='yellow'>{1} </font>",
	
	"chat.announce.quake.taser": "{green}Gold KingZ {grey}| HAHAHA {purple}{0} {grey} Zeused {yellow}{1}",
	"center.announce.quake.taser": "<font color='white'> H A H A H A <br> <font color='purple'>{0} <font color='white'>Zeused  <font color='yellow'>{1} </font>",
	
	
	"chat.quake.grenade": "{green}Gold KingZ {grey}| Nice! Grenade Kill, You Killed {yellow}{0}",
	
	"chat.quake.molly": "{green}Gold KingZ {grey}| Nice! molotov Kill, You Killed {yellow}{0}",
	
	"chat.announce.quake.selfkill": "{green}Gold KingZ {grey}| {purple}{0} {grey}Killed Himself",
	
	"chat.announce.quake.teamkill": "{green}Gold KingZ {grey}| {purple}{0} {darkred}TeamKill {yellow}{1}",
	
	"chat.announce.quake.firstblood": "{green}Gold KingZ {grey}| {BlueGrey}FirstBlood !!!  {purple}{0} {purple} Killed {yellow}{1}",
	
	
	"chat.announce.quake.roundprepare": "{green}Gold KingZ {grey}| {grey}Prepare To Fight...",
	"center.announce.quake.roundprepare": "<font color='yellow'>Prepare To Fight <font color='darkred'>... </font>",

	"chat.announce.quake.roundstart": "{green}Gold KingZ {grey}| {lime}Round Start !",
	"center.announce.quake.roundstart": "<font color='green'>Round Start <font color='lime'>!!! </font>",
	
//--------------------------------------------------------------------------------------------------------------------------------------------------------------------------//

	"menu.item.freeze": "Freeze Open Menu",
	"menu.item.bodyhit": "Body Hit Sound",
	"menu.item.bodykill": "Body Kill Sound",
	"menu.item.headshothit": "HeadShot Hit Sound",
	"menu.item.headshotkill": "HeadShot Kill Sound",
	"menu.item.quake.sounds": "Quake Sounds",
	"menu.item.quake.center.messages": "Quake Center Message",
	"menu.item.quake.chat.messages": "Quake Chat Message",
	"menu.left.image": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/left.gif' class=''>",
	"menu.right.image": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/right.gif' class=''>",
	"menu.more.down": "<img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/arrow.gif' class=''> <img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/arrow.gif' class=''>",
	"menu.bottom": "           <font color='cyan'>[ WASD - To Native ]</font> <br><font color='purple'>[ <img src='https://raw.githubusercontent.com/oqyh/cs2-Kill-Sound-GoldKingZ/main/Resources/tab.gif' class=''> - To Exit ]<br>"
}
```


## .:[ Change Log ]:.
```
(1.1.1)
-Support FFA DM 

(1.1.0)
-Fix Toggle Crossing Each Attackers
-Changing Config.json Names DefaultValue To KS_DefaultValue_
-Added Mysql KS_UseMySql

(1.0.9)
-Fix Toggle On Cookies


(1.0.8)
-Added KS_AutoRemovePlayerCookieOlderThanXDays
Auto Delete Inactive Players Cookies Older Than X Days plugins/Kill-Sound-GoldKingZ/Cookies/Kill_Sound_Cookies.json

(1.0.7)
-Fix Some Bugs
-Rework Menu Expose Toggle On / Off Without Hover Over
-Fixed Fly Bug (Turn On Freeze While Jump)  
-Added KS_ResetKillStreakOnEveryRound
-Added KS_AddMenu_FreezeOnOpenMenu 
-Added KS_AddMenu_QuakeSoundsToggle 
-Added KS_AddMenu_QuakeCenterMessageToggle 
-Added KS_AddMenu_QuakeChatMessageToggle 
-Added Quake In Menu
 -"ShowChat"
 -"ShowCenter"


(1.0.6)
-Upgrade Net.7 To Net.8
-Fix RoundPrepare, RoundStart Bug
-Added Menu For Hit Sounds "KS_InGameMenu"
-Added Flag For KS_InGameMenu "KS_OnlyAllowTheseGroupsToToggle"
-Added Quake [ "TaserKill" ]
-Added Better Control On Text in "Kill_Settings.json"
 -"ShowChat"
 -"ShowCenter"
 -"ShowCenter_InSecs"

(1.0.5)
-Rework Kill Sound Plugin
-Disable Menu (Temp)
-Disable Toggle (Temp)
-Added Quake [ "HeadShot" , "Kill" , "KnifeKill" , "GrenadeKill" , "MollyKill" , "SelfKill" , "TeamKill" , "FirstBlood" , "RoundPrepare" , "RoundStart" ]

(1.0.4)
-Rework Menu (SoundDisableCommandsMenu)

(1.0.3)
-Fix Null

(1.0.2)
-Fix Sounds On Teammate

(1.0.1)
-Added HeadShotKillSoundPath
-Added BodyKillSoundPath
-Added HeadShotHitSoundPath
-Added BodyHitSoundPath
-Added SoundDisableCommandsMenu
-Added SoundDisableCommands
-Added RemovePlayerCookieOlderThanXDays

(1.0.0)
-Initial Release
```

## .:[ Donation ]:.

If this project help you reduce time to develop, you can give me a cup of coffee :)

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://paypal.me/oQYh)
