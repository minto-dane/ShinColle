Shin Colle
==========
Shinkeiseikan Collection

Add cute ship girls for battle and decoration.


To translator (except zh_TW):
You can edit ship/item description as you like.
I finished en_US by google translate, please correct the weird translation if you found.



Dev Video:
https://www.youtube.com/playlist?list=PLzA0TpkwD25D0Q8bwcejxokKJDVzSnk2A

Forum (Chinese)
http://forum.gamer.com.tw/C.php?bsn=18673&snA=124090&tnum=1

Mod download (Curse)
http://www.curse.com/mc-mods/minecraft/228395-shincolle

Mod source code with build.gradle (Google Doc)
1.7.10:
https://drive.google.com/file/d/0Bwod9-SE78mFbkoydnZFbmtnRDg/view?usp=sharing

Config notes
------------
- Main config file is generated at: `<minecraft config dir>/shincolle/shincolle.cfg`.
- Ship strength related settings are in category `ship setting`, especially:
  - `Attrs_Scale`
  - `Attrs_Limit`
  - `Attrs_Hostile_SmallBoss`
  - `Attrs_Hostile_LargeBoss`
  - `Attrs_Hostile_SmallMob`
  - `Attrs_Hostile_LargeMob`
- Source reference: `src/main/java/com/lulan/shincolle/handler/ConfigHandler.java`

Bug found during investigation
------------------------------
- Build may fail at dependency resolution for ForgeGradle (`net.minecraftforge.gradle:ForgeGradle:2.3-SNAPSHOT`) because it depends on the legacy host `http://files.minecraftforge.net/...`, which can be unavailable. Workaround example: in `build.gradle`, replace `maven { url = "http://files.minecraftforge.net/maven" }` with `maven { url = "https://maven.minecraftforge.net" }` (or another reachable internal mirror).
