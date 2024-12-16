Firearms Half-Life
Release Candidate 3.0 -- readme.txt
http://www.firearmsmod.com
-------------------------------------

v3.0
-----
[03.29.05]

Changes/Additions:
---------------------------------------

* Fixed treating concussion crash

* Fixed healing ammobox crash

* Fixed debug log files showing up on root C: drive
*** Fixed lag while shooting if debug logs were NOT read-only

* Fixed 'ghosting' spectator bug

* Added ability to choose voice set from command menu

* Fixed obscured death notice text when spectating
*** Was blocked by the VGUI part of the Spectating panel

* Moved scoreboard to last on the VGUI stack (means its always on top of everything else)

* Fixed parachute still being deployed after dying, spectating, then changing teams

* Fixed view bump on take damage not affecting actual accuracy

* Locked cl_sidespeed value to 400 (default)

* Locked cl_forwardspeed value to 400 (default)

* LOcked cl_backspeed value to 400 (default)

* Lowered prone view position by 2 units

* Removed first person spectating (WAY too many bugs)

* Fixed ability to reload instantly after a prone sequence is completed

* Fixed multiple ricochet sounds playing on a single bullet impact

* Installed Global FA ban for caught cheaters

* Reduced max concussion value by 5

* Lowered penetration distances on all rifles

* Turned on FA Hard Code ban list and added all FAL ban ID's and Verified Jolt ban ID's

* Reduced Sniper Rifles ability to shoot while unscoped (cannot effectively shotgun snipe anymore)
 
* Fixed UZI lighting world brushes even with surpressor

* Lowered merge magazine sound volume for players with stealth skill

* Increased accuracy of all weapons roughly by 25%

* Changed Armor back to original 2.9 values: (Absorbtion Amount-- 80% Heavy, 70% Medium, 60% Light)

* Added AK74 nomenclature reload/animations

* Added MP5a5 nomenclature reload/animations

* Added Anaconda nomenclature reload/animations

* Added new Weapon Sounds (many different types)

* Numerous Gun Balances (way to many to list) 

* Increased default max_speed to 270 (was 250)

* Added new player movement sounds

* fixed bfinfo bug (related to battlefield information)

* fixed treat reload bandage exploit

* cleaned up tons of unused code and coding errors




MAPS:

---------------------------------------

* Added new Texture Details for maps: OBJ_Vengeance, PS_Upham, SD_Durandal, SDTC_Balcome, TC_Basrah, TC_caen, TC_Iwojima. 

* Added new map OBJ_Vengeance 

* Added new version of TC_Caen




-------------------------------------
Firearms Half-Life
Release Candidate 2.9 -- readme.txt
http://www.firearmsmod.com
-------------------------------------

v2.9
-----
[04.04.04]

Changes/Additions:
------------------
- Added M14 with optional A.C.O.G scope (Marksmanship skill required).
- Added M4 Carbine with optional suppressor (Stealth skill required).
- Added map cleanup after a round ends.
- Added new bullet impact effects.
- Added new entity - trigger_noclaymores - Players cannot place claymore mines while in this area.
- Added new entity - trigger_reinforcements - Triggered when one team (or both) run out of reinforcements.
- Added new gameplay optimisations.
- Added new keyvalue to the fa_team_item entity, to let mappers disable the glow.
- Added new keyvalue to the fa_team_item entity, to let mappers specify the delay before a dropped item is returned.
- Added new keyvalue to the game_zone entity, to let mappers specify which team it can be triggered by.
- Added new night vision effects.
- Added new radio sounds.
- Added new VGUI preconfiguration screen.
- Added new weapon prediction code to comply with latest standards.
- Added noise reduction for all sounds created by players with the stealth skill (except firing).
- Added ricochet sounds to the client side.
- Added smoke grenades as artillery markers.
- Added sprite to the HUD to indicate bleeding.
- Added the option to spectate before running out of reinforcements.
- Fixed all crashes related to mortar statistics (will no longer be displayed).
- Fixed bandage and reinforcement sprites appearing in spectator mode.
- Fixed exploits involving infinite stamina.
- Fixed exploits involving third person views.
- Fixed jumpy scope sway.
- Fixed 'No Valid Targets' error.
- Fixed prone levitation.
- Fixed reinforcement penalties being applied to teams with 0 reinforcements.
- Fixed sticky bodies and prone players.
- Fixed strafe speed boost.
- Fixed telefragging.
- Fixed various other minor bugs. Too numerous to list.
- Fixed various weapon balance issues. Too numerous to list.
- Removed hundreds of lines of unused code.
- Removed unused particle systems, resources, and variables.


New maps:
Armory
Basrah
Sweden

Updated maps:
Crash
Marie
Oberland
Thanatos
Willow

New CVARS:
----------

"allow_spectators" (server only)
"allow_spectators" allows you to disable spectator modes on your server. When set to 0 players will not be allowed to choose to spectate from the team selection menu.
default: 1

"cl_markertype"
"cl_markertype" lets you select the type of artillery marker you wish to view. When set to 1 it will use the new smoke grenade system, and when set to 0 it will use the alternative light strobe system. Slower computers will experience a considerable performance increase around artillery markers with this set to 0.
default: 1

"mp_fpspeconly"
"mp_fpspeconly" will limit spectators to first person mode if set to 1.
default: 0

"mp_specteam" (server only)
"mp_specteam" allows you to restrict spectator modes on your server. When set to 1 players will only be able to spectate their own team, and the free roaming spectator modes will be disabled.
default: 0

"r_detailtextures" (Steam only)
"r_detailtextures" enables or disables the new detail textures system. Detail textures improve the visual quality of low resolution textures when viewed at close range. Detail textures will be displayed with this setting at 1, and disabled at 0. You will require an nVidia Geforce 4, ATI Radeon 8500, or more recent graphics card to take advantage of this feature. Slower computers will receive a significant performance increase with this feature disabled.
default: 0

"sv_endreins" (server only)
"sv_endreins" specifies the amount of reinforcements one team needs to hit before the map changes (only used if sv_playtoend is set to 1).
default: 0

"sv_playtoend" (server only)
"sv_playtoend" enables you to set your server to change maps when a team reaches a certain number of reinforcements. If set to 1, the map will change when a team's reinforcements drops to the value specified by the sv_endreins command. At 0 the game will finish when one team has no reinforcements and no players alive.
default: 0

"sv_restartround" (server only)
"sv_restartround" allows you to reset all players, entities, scores, timers, and reinforcement counts without changing map on your server. It is ideal for clan matches. When set to 1, the round will be restarted.
default: 0

-----------------------------------

v2.8
-----
[10.10.03]

Changes/Additions:
------------------
- Added ability for medics to heal before the maximum amount they can heal has been lost.
- Added ability to treat concussions to medics.
- Added ammobox hit effects.
- Added battlefield information ability to the leadership skill.
- Added concussion effect to concussion grenades.
- Added CTI items to the compass.
- Added delays to applying sulphur, suturing, and bandaging.
- Added entity optimization system (cl_optimizedraw).
- Added global banning system (sv_enforceban).
- Added mortar statistics to the HUD.
- Added Night Vision Goggles.
- Added nomenclature ability to Sterling L2A3MK4 (new model included).
- Added PKM with bipod functionality in place of the Steilhandgrenate.
- Added rain and snow weather systems.
- Added Remington M870 in place of the Benelli M3.
- Added scope sway system.
- Added secondary fire to grenades (new model included).
- Added sounds for bandaging, merging magazines and grenade fuses.
- Added VGUI based respawn menu.
- Added VGUI based end game screen.
- Added new event based shell ejection system for all view models.
- Fixed audible claymores with stealth skill.
- Fixed breathing sound playing after player's death.
- Fixed claymore setting to trip mode if bandaging while the clacker is out.
- Fixed death animation abnormalities while prone in water.
- Fixed double fog bug.
- Fixed iFeel support.
- Fixed levitation.
- Fixed server and client deploy times being out of sync.
- Fixed sv_useskills 3 bug (getting stuck in skills menu). 
- Fixed the respawn menu not displaying automatically.
- Fixed various other minor bugs. Too numerous to list.
- Fixed various view height and hull problems.
- Fixed various weapon balance issues. Too numerous to list.
- Cleaned up lots of unused code.
- Reduced chance of getting stuck on corpses.


New maps:
Caen
Splinter

Updated maps:
Bocage
Coldwar
Force
Golan
Marie
Oberland
River
Thanatos
Willow

New CVARS:
----------

"cl_optimizedraw"
"cl_optimizedraw" allows you to enable entity based optimizations which may result in a performance increase on slower machines. However, this may also cause extreme visual abnormalities in certain situations.
default: 0

"cl_weather"
"cl_weather" allows you to enable or disable Firearms' particle based weather systems. Slower computers will experience a slight performance increase with this set to 0.
default: 1

"cl_weathereffects"
"cl_weathereffects" enables or disables weather based effects, such as water splashes. Slower computers will experience a slight performance increase with this set to 0.
default: 1


-----------------------------------

v2.7
-----
[04.04.03]

Changes/Additions:
------------------
- Added 45 second delay before CTI object is returned to its original location if dropped.
- Added basic HLTV functionality.
- Added battlefield agility causing all stamina burns to be decreased by one third.
- Added dynamic lighting to sparks.
- Added dynamic lighting to the claymore explosion.
- Added friend/enemy display in team ID bar.
- Added full use of bipods for the M82, M60 and M249.
- Added key value to func_friction to choose to affect all entities or just players.
- Added key value to info_firearms_detect, choose whether or not a player's breath is visible (cold weather or warm weather).
- Added key value to trigger_gravity to choose to affect all entities or just players.
- Added M249 light machinegun in place of PKM. PKM will return in a future version of Firearms.
- Added map fogging (OpenGL only).
- Added 'Most Cowardly' award to end game screen.
- Added moving mouths when voice communication is in use.
- Added muzzleflash sprite to the mortar.
- Added randomness to shell ejection velocities
- Added reinforcement bonuses for capturing a push point.
- Added reinforcement bonuses for continued possession of a push point.
- Added server name to the scoreboard.
- Added speech icons above players' heads (displayed when radio is being used).
- Added use of TFC-like status bar for screen tips and player ID
- Added voice icon above players' heads (displayed when voice comm. is being used).
- Added word filter system ability (for players that are offended by racial slurs, swearing, etc).
- Fixed best player calculation to be more accurate.
- Fixed black screen of death (map change lag).
- Fixed mortar damage going through walls.
- Fixed 'no helmet' exploit.
- Fixed prone flying exploit.
- Fixed "Sprite: No Such Frame..." error.
- Fixed 'sticky corpses'.
- Fixed team change retaining the same armour.
- Fixed various other minor bugs. Too numerous to list.
- Fixed various weapon balance issues. Too numerous to list.
- Fixed vote_llama server crash bug.
- Players with stealth skill don't trigger sounds when capturing areas or placing claymore mines.
- Reverted the HULLs and views back to default (to prevent 'helmet cam' exploits).
- Status icons for broken legs and parachutes are now colour coded.


New maps:
Force
Golan
Oberland
Thanatos

Updated maps:
Bocage
Marie
Paradise
River
Upham
Willow

New CVARS:
----------

"cl_censor"
"cl_censor" allows you to filter out certain words from the game. If set to 0, no censorship occurs. At 1, racist remarks are censored. At 2, swearing is censored. At 3, both racism and swearing are censored.
default: 0

"cl_dlights"
When "cl_dlights" is set to 0, all non-map dynamic lights are disabled (muzzleflashes, explosions, etc), giving an increase in performance on some systems.
default: 1

"cl_fog"
When "cl_fog" is set to 1, map specific fog effects are enabled. This may decrease performance, but will hide ugly occurrences when there is geometry outside of the specified draw distance. OpenGL mode only. Requires a map change or a restart of the game for changes to come into effect.
default: 1

"cl_voiceicon"
Setting this to 0 will disable the icon above players who are using voice communication (friendly players only).
default: 1

"mp_ffremoverein" (server only)
If set to 1, this command will remove one reinforcement for a team kill. At 0, there will be no penalty for the team.
default: 0

"mp_loglevel" (server only)
The amount of data which is stored in server logs. 0 will log basic events such as connects and disconnects, 1 will log connects, disconnects, objectives, triggers, and kills. 2 will log everything, resulting in enormous log files.
default: 1

"text_ignore"
"text_ignore", followed by a WONID, will block any text from certain players. To see a list of players and their WONIDs, use the "status" command.

"text_unignore"
"text_unignore, followed by a WONID, will cancel previous ignores for the matching player.


-----------------------------------

v2.65
-----
[9.17.02]

Changes/Additions:
------------------
- AK-47 accuracy decreased.
- AK-47 accuracy improvement time fixed.
- AK-47 damage decreased.
- AK-47 recoil increased.
- AK-47 value increased by one credit.
- Benelli M3 accuracy increased.
- Claymore mine damage changed to be more realistic. The majority of the damage is now done in front of the mine.
- Claymore mines are no longer usable in mid-air.
- FA-MAS value increased by one credit.
- G3A3 recoil increased.
- Grenade launcher range increased.
- Grenade launcher range has a slight randomness now.
- Grenade launcher projectiles now deactivate after coming into contact with a sky brush.
- Grenade launcher projectiles now use a more network efficient particle effect for their smoke trails.
- M16 fire mode no longer resets after holstering.
- M16 accuracy problems fixed.
- M60 recoil increased.
- M82 accuracy decreased.
- M82 firing disabled while the player is moving or in the air.
- M82 rate of fire decreased.
- M82 recoil increased.
- M82 value increased by one credit.
- MP5 accuracy problems fixed.
- Steilhandgrenate fuses no longer pause while sprinting.
- Sterling accuracy decreased.
- Sterling no longer unnecessarily reloads.
- 9mm penetration values decreased.
- Added a new entity - trigger_zone - Used for mappers placing areas where mortars, claymores, and medevacs can be offlimits.
- Added a new entity - env_spriteshooter - Similar to the env_shooter entity.
- Added a new keyvalue to the fa_team_item entity, to let mappers specify weapon restrictions applied to the player carrying the object.
- Added a debug command for use in situations where you are stuck after getting up from prone. Bind to a key via the controls menu.
- Added alternative (shorter) reload animations to the M16 for use with the Nomenclature skill (new model included).
- Added command menu functionality. Bind to a key via the controls menu.
- Added double magazines to the AK-47 for use with the Nomenclature skill (new model included).
- Added dynamic lighting effects to all explosions.
- Added dynamic lighting to muzzleflash effects. This does not effect suppressed weapons.
- Added medevac helicopter effects.
- Added particle based spark effects for metal and concrete bullet impacts.
- Added reinforcement information to the scoreboard.
- Added snow footstep sounds.
- Bullet impacts no longer effect a player's movement. Removed for many reasons.
- Changed M60/PKM/Claymore tracers to the client side.
- Disabled firing while crawling in prone.
- Disabled the use of the knife while prone. The only possible fix for the 'flying knife' bug.
- Enhanced the end of game screen with 'Best Player' (from both teams), 'Most Kills' and 'Most Deaths' information.
- Fixed all known problems with changing teams.
- Fixed all known prone bbox, hull, and hitbox issues.
- Fixed all weapons appearing to shoot higher than they do.
- Fixed bbox abnormalities with dead and wounded players.
- Fixed crouch bbox and hitbox abnormalities.
- Fixed Fatigue sound playing underwater.
- Fixed helmet removal effects for players who have no helmet.
- Fixed prone players blocking other player's paths.
- Fixed prone players not triggering certain entities.
- Fixed prone players staying prone while swimming.
- Fixed Search and Destroy object explosions occurring in the wrong place.
- Fixed the idle animations on the ammobox.
- Fixed use key movement exploit.
- Fixed various player model animation abnormalities.
- Fixed view height of prone, crouched and standing players to avoid the 'helmet cam' exploit.
- Reduced the amount of 'bad' network traffic by 90% after a map change and when players start to join.
- Removed friendly fire damage from ammobox explosions on servers with friendly fire disabled.

Updated maps:
Balcome
Bocage
Coldwar
Durandal
Marie
Upham

New CVARS:
----------

"cl_hudcolour"
When "cl_hudcolour" is set to 0, the player's hud will display using the default colors. Changing this value from 0-7 will change the hud to a variety of different colors.
default: 0

"cl_particles"
When set to 1, high quality particle effects are used. Set to 2 for reduced effects, and 0 for no effects (0 recommended for software rendering mode).
default: 1

"cl_ifeel"
When set to 1, this cvar will enable Immersion Touchsense support, as long as Touchsense enabled hardware is detected.
default: 1

"cl_skin"
This cvar changes which skin is used on the player's model. See the multiplayer/customize/advanced menu for detailed descriptions.
default: 0


-----------------------------------

v2.6
----

Changes/Additions:
------------------
- Fixed countless bugs and exploits from previous versions.
- Removed weapons: Steyr AUG, H&K MC51, Akimbo M11s, PSG-1, M4, and Flashbang Grenade.
- Added weapons: Sig SSG3000, PKM, UZI, Dragunov SVD, AK-74 with GP-25, and Concussion Grenade.
- Added particle systems (cl_particles 0/1/2 | off/normal/limited). - SHOULD BE DISABLED FOR SOFTWARE MODE.
- New weapon selection menu.
- Added ability to edit all preconfigured classes.
- All new player and weapon models, skins, animations and sounds.
- Added player customization (bind key via controls menu).
- Added realistic weapon recoil.
- Added Immersion iFeel force-feedback support.
- Many tweaks to client-side weapon code.
- Added menu selection for changing teams.
- Added menu for llama vote-kick (bind key via controls menu).
- Added ability to attach silencers to UZI, MP5 and Beretta 92f with Stealth Skill.
- Added ability to use grenade launcher attachments on AK-74 and M16 with Artillery Skill.
- Added ability to use scope on Anaconda with Marksmanship Skill.
- Modified gun damage values, armour values, bullet penetration values and weapon costs.
- Added ability to sprint (bind key via controls menu).
- Added slow down when using scope.
- Removed ability to fire machinegun while in air or running.
- Added ability to change hud colour (cl_hudcolour 0 - 7).
- Added maps: obj_bocage, obj_paradise, obj_willow, ps_deadline, ps_upham, sdtc_balcome, tc_rubble.
- Updated maps: ps_coldwar, ps_crash, ps_greatoutdoors, ps_inlands, ps_marie, ps_river, ps_swamp, sd_durandal, tc_iwojima.
- Modified logging to meet Half-Life logging standards.
- Updated hud graphics.
- Added individual scopes for each weapon.
- Added individual reticules for each weapon.
- Added Valve Voice-Communication technology support.
- Added basic HLTV spectator technology.
- Added realistic and logical magazine changes (ie: extra round stays in chamber, magazine with most rounds chosen).
- Added ability to merge partially used magazines (bind key via controls menu).
- Added helmet knock-off for headshots.
- Countless other small additions and tweaks.

-----------------------------------
Overview

Firearms is a modification for Valve's award winning Half-Life.  Firearms is a multiplayer modification that introduces realistic weaponry and new exciting scenarios to the half-life engine.  The purpose of Firearms is to bring an entertaining multiplayer experience by combining real world weapons and scenarios to the Half-Life engine.

Firearms emphasizes team cooperation with unique scenarios such as Push and Capture the Intelligence.  It is also fully customizable, allowing players to contribute to their team in many different ways such as providing cover fire or taking the role of a sniper.  With Firearms, players can immerse themselves in modern warfare with realistic weapons, accessories, and environments.  

Included maps feature scenarios such as the territorial push, and the unique Capture the Intelligence (or CTI).  With Capture the Intelligence, mapmakers have the freedom to make their own scenarios rather than be restricted to simple capture the flag or team deathmatch.

A plethora of modern day weaponry is also included.  An assortment of pistols, shotguns, sub-machineguns, rifles, grenades, explosives, and accessories are at your disposal.  These weapons can be accessed through a unique credits system which gives players who have just entered the game, as good a chance as one who has been playing for an hour.

Now, with the addition of the innovative skill and ranking system, a feeling of accomplishment is added as you battle with your team.  The ability to earn valuable traits such as field medicine and leadership adds more to the firearms experience.

We believe that Firearms provides a unique experience for all players, and we sincerely hope that you will enjoy this exciting modification as you are immersed in the world of modern warfare.

-----------------------------------
Quickstart

1.  Start Half-Life by clicking on Half-Life shortcut.
2.  Access the Custom Game menu, and activate Firearms.
3.  Configure your controls by selecting configuration, then controls.
4.  Customize your online persona by selecting multiplayer, then customize.
5.  Join a game by selecting multiplayer, then internet games.

-----------------------------------
Basic Gameplay

Before you begin experiencing the excitement of online warfare, make sure you've configured your controls and customized your online persona.  Make sure you assigned slots 6-9 in your controls configuration, or some menus may not function properly.  Most people don't think to highly of someone named 'Freshmeat', so make sure to make a good first impression.  Now go ahead and join a server.  If you need assistance with Gamespy (http://www.gamespy3d.com) or Half-Life's built in internet browser, consult their documentation.

Once you connect you will be suspended in mid air with a team selection menu before you.  Choose either the Red or Blue Force or let the computer choose for you.  Then either select the option to configure your weapons, or choose a predefined class.  If you choose to configure your arsenal by yourself, you will have to choose armor, an optional item, and weapons.  As you're building up your arsenal, watch your credits, the more you use up, the more weighted you will become.

Once you've finished your selections you'll be dropped into the battlefield.  The gameplay modes currently supported are Teamplay (maps preceded with tp_), Capture the Intelligence (maps preceded with cti_), Territorial Control (maps preceded with tc_), Objective Based (maps preceded with obj_), Search and Destroy (maps preceded with sd_) and Push (maps preceded with ps_). Firearms 2.6 provides several maps taking advantage of the Territorial Control, Objective Based, Search and Destroy and the Push gameplay modes, but certain servers include custom made maps, so the ability to play the remaining two types.

From here on your best bet is to experiment.  Try out all the weapons, find out what works for you and what doesn't.  Only by understanding the weapons can you master Firearms.  Good luck, and we hope that you enjoy this modification for Half-Life!

-----------------------------------
New Controls

Choose team (default: i) - If you feel the game is shifting too far to the advantage of your team, then you can press this key to display a menu allowing you to change your team.

Customize appearance (default: o) - Pressing this key will display a menu allowing you to alter your appearance to suit your personal tastes. The changes are just visual.

Sprint (default: x) - For an extra burst of speed, you can use this button. Your stamina will deplete quickly though, so sprint wisely. Also remember that while sprinting, you cannot use any weapons except the knife.

Treat (default: l) - This is simply a shortcut to the command that can be accessed through the skills menu after you have acquired a Medic skill. If there is a player directly in front of you, you will treat them. If there is no player in front of you, you will treat yourself. If you, or the player in front of you, do not need treating, then you will call out letting others know there is a medic available. You must have available medical supplies to use this key.

Set hospice (default: ;) - This is simply a shortcut to the command that can be accessed through the skills menu after you have acquired a Medic skill. You will place a hospice flag to let players know there is a medic available. Hospice flags are removed when you are killed.

Set artillery marker (default: m) - This is simply a shortcut to the command that can be accessed through the skills menu after you have acquired an Artillery skill. An artillery marker will be placed where you currently stand, as long as you are outside.

Merge partially used magazines (default: n) - This key will lower your weapon and merge any magazines which have been partially used. For instance, if you press the merge magazines key when you have two half empty magazines, they will be merged to one full magazine. If you have one magazine missing five rounds, and another missing ten, five rounds will be deducted from the magazine with ten rounds missing, to create a full magazine and a magazine with fifteen rounds missing.

Apply bandage (default f) - Press this button when you are bleeding to patch up the wounds (Only available if you have a bandage.  If you can hear yourself breathing heavily, and are periodically losing small amounts of health, then you are bleeding.

Toggle weapon fire mode (default: g) - This button switches between firing modes on your weapons.  These consist of single shot, full auto, and 3 round burst.  Keep in mind that certain guns do not have some firing modes.

Bring up Use Skills menu (default: h) - To use certain skills such as building artillery you will need to press this button and select the appropriate function.

Show Available Skills (default: j) - If you need to see what skills you currently have press this button.

Bring up Radio/Voice Menu (default: b) - When you press this button you will have the ability to use a predefined radio or voice message.  Radio messages to go everyone on your team.  Voice messages are heard by those around you.  Have fun with the war cry :)

Toggle prone position (default: z) - This switches between standing up and being prone.  Being prone makes your person lie on their stomach and allows for increased accuracy

Use item (default: e) - Use items allows you to do such functions as press buttons, use ammo crates, and fire mortars.

Drop item (default: Backspace) - Pressing this button will make you drop the Capture the Intelligence item you are currently holding (usually a case or flag). 

Command Menu (default: p) - Using this button will display an in game menu with a series of useful options, such as shortcuts to radio commands and skills.

Merge magazines (default n) - This button will merge any partially depleted magazines into a full one.

Deploy bipod (default: v) - Bipods are available on certain weapons, and give increased stability resulting in increased accuracy and decreased recoil.

Battlefield information (default: /) - Holding this button will display useful information about the battlefield. The leadership skill is required to use this ability.

Night vision goggles (default: c) - This button activates and deactivates the night vision goggles (if you possess them).

-----------------------------------
Skill and Ranking System

With the release of release candidate 2.1 came the introduction of the skill and ranking system.  Every time you earn 10 points, you will earn a rank.  Upon earning a rank you will be able to choose a skill such as nomenclature (faster reloading) or artillery (ability to use mortars).  We feel that this is a very exciting addition, as it allows you to build up the character you wish to play and adds a new dimension to Firearms.  Plus, while the skills are beneficial, they do not unbalance the game to the point where it is difficult for players just entering the game to succeed.

If you would like to read a comprehensive guide on the skills, please visit http://www.firearmsmod.com and look under the manual section for a skill guide.  It contains information on every skill, allowing you to evaluate the skills beforehand so you can make an educated choice on which you want during the game.

-----------------------------------
Fatigue System

The fatigue system was introduced with release candidate 2.1 as well, and then heavily tweaked in 2.6.  This was added to encourage more strategic play in firearms.  You can see the status of your stamina by looking at the colored bar on the left side of your screen.  Whenever you sprint or jump, you will become more fatigued.  Once the bar on the left becomes drained completely, you movement speed will become much slower, forcing you to rest.  In order to gain stamina back you must either stand still or crouch.  Crouching is the fastest way to regain stamina so keep that in mind when you are fatigued.

-----------------------------------
Compass

The compass is a bar displayed on your HUD, at either the top or bottom of your screen. It displays map objectives, the position of your squad leader, and the position of any radio commands, such as artillery requests. Console commands for the compass are: cl_compass 0/1/2 for off, top, and bottom. A flag in the compass denotes a "push" point. It will either be Red, Blue, (depending on which team controls it) or white (if no one controls it). A red or blue crate signals a "search and destroy" crate. These won't change color. A yellow star is the position of your leader, and a green radio is the position of the last radio command. Note that the compass does NOT show height, just general direction (N, S, E, W).

-----------------------------------
Other Notes

The secondary fire key will use the scope on your weapon of it has one. Other weapons may have other secondary functions, such as bayonets or mounted grenade launchers. If your weapon does not have a secondary function, the secondary fire key will toggle between the available fire modes for that particular weapon.

The use key will open up your parachute while you are in the air, and take it off when you are on the ground.  You can also detach your parachute in mid air to save a little time. Be careful though, as detaching too early can result in a broken leg, or even death.

-----------------------------------
Beta Status

Firearms is currently in release candidate stages (also known as 'beta') and as such may have unforeseen problems and glitches. If you encounter problems, please let us know posting on our forums, which are located at http://forums.firearmsmod.com

-----------------------------------
CREDITS:

Firearms team members:
Ben Irwin		- Team lead, 2D art, 3D art, Animation.
Cale Dunlap		- Programming.
Dean Gagnon		- Programming.
Graham Davis		- Additional Programming, Mapping.
Stephen Charman		- Additional Programming, iFeel effects.
Christian Øelund	- 2D art, 3D art, Animation.
Ross Thelen		- 2D art, 3D art, Animation.
Albert Edinoff		- 3D art.
Rusbin Lopez		- 2D art.
Alex Jordan		- Mapping.
Stephen Jackson		- Mapping.
Stephen Gangi		- Audio.

Former Firearms team members with contributions to 3.0:
Eric Smith		- Programming, Firearms' daddy.
Scott Rennie		- Programming.
David Reeves		- Mapping.
Tyler Munden		- Mapping.
Michael Hope		- Mapping.
Jon Monaghan		- Mapping.

External contributions:
Brian Schkerke		- Linux Port.
Alex Fenton		- Mapping.
Zach Ford		- Mapping.
Toni Hiltunen		- Mapping.
Phil Mapleback		- Mapping.
Bill Parsh		- Mapping.
Sigurd Svidal Randal	- Mapping.
James Trogdon		- Mapping.
Chuckie Wilson		- Mapping.
Samuel Cho		- Radio Sounds.
Belial			- 2D art.
Ville Kytömäki		- 2D art.
Mike St. Pierre		- Local gun nut.

Map Credits:
Armory			- James Trogdon
Balcome			- Phil Mapleback, Belial.
Basrah			- Alex Fenton.
Bocage			- Alex Jordan, Graham Davis.
Caen			- Bill Parsh.
Coldwar			- Graham Davis.
Crash			- Sigurd Svidal Randal, Phil Mapleback, Chuckie Wilson.
Durandal		- David Reeves, Phil Mapleback.
Force			- Jon Monaghan.
Golan			- Alex Jordan.
Iwojima			- Tyler Munden.
Marie			- Michael Hope, Alex Jordan.
Oberland		- Alex Jordan.
Paradise		- Ben Rosen.
River			- Graham Davis.
Splinter		- Zach Ford.
Thanatos		- Stephen Jackson.
Upham			- Toni Hiltunen.
Willow			- Graham Davis.
Vengeance		- Stephen Jackson.

Special thanks to:
All the beta testers, especially Clan Seek and Destroy [S^D].
Mr. D for doing all the nomenclature animations for 3.0.
Wesley "Crystalx" Hayes for all the coding help.
Phil Mapleback for his invaluable mapping help.
Everyone at Valve Software, for obvious reasons.
Christopher 'Ilian' MacArthur and Tony 'omega' Sergi for their help with all things programming related.
Bob Heubel and everyone at Immersion for their help with iFeel support.
Recon Gamer for their web hosting services.
Will Mackey for being incredibly generous.
And anyone else we've forgotten.