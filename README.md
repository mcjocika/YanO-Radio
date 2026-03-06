# YabO-Radio
DIY webrádió projectem
YanO‑Radio  
Felhasználói kézikönyv 
2026‑03‑05   |   Pápai József
Tartalomjegyzék: 
 
 
Tartalomjegyzék: ....................................................................................................................................... 2 
Wifi web rádió felhasználói utasítás: ................................................................................................... 3 
Beüzemelés: ................................................................................................................................................ 4 
Funkciók: ...................................................................................................................................................... 5 
Kezelés: ......................................................................................................................................................... 6 
Kezelés az előlapi tekerő gomb segítségével: .................................................................................. 6 
Kezelés az érintőkijelzőn: ........................................................................................................................ 9 
Webszerver funkciói: .............................................................................................................................. 10 
Történelem: ............................................................................................................................................... 15 
Koncepció: ................................................................................................................................................. 16 
Koncepció rajz: ......................................................................................................................................... 17 
Koncepció AI segítség: .......................................................................................................................... 18 
Alkatrész lista: ........................................................................................................................................... 19 
Hiba elhárítás: ........................................................................................................................................... 20 
Források: .................................................................................................................................................... 21 
 
  
YanO-Radio Felhasználói kézikönyv
Wifi web rádió felhasználói utasítás: - A webrádió kizárólag internetes streamek lejátszására képes. - Önnállóan, wifi és internet hiányában nem működik ! - Támogatott Wifi szabvány: 2,4 GHz  
A rendszer elemei: - Webrádio - Érintő toll - Hangfalak - Tápegység(230/12V Dc 5A) 
3
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Beüzemelés: 
A rendszer a hálózathoz(230V) csatlakoztazot tápegységen keresztül kell működtetni. A 
tápegység 12 Volt 5 Amper terhelhetőségű, mely paraméterektől eltérni nem szabad, 
különben a berendezés károsodásához vezet. 
A tápegységet a rádió hátulján található 12V DC feliratú aljzathoz kell csatlakozatni. 
A főkapcsoló gomb BE állásba történő átbillentésvel kapcsoljuk be a készüléket.  
Első indításkor amennyiben nem tud ismerős hálózathoz csatlakozni amutoamtikusan 
átvált AP módba(hozzáférési pont mód). 
Ilyenkor a kijelzőn láthatő SSID-t közvetíti(YanO-Radio_AP). Az erre alkalmas wifi képes 
készülékkel csatlakozzunk hozzás a kijelzőn látható jelszó segítségével(12345987). 
Állítsuk be a saját wifi hálózatunk SSID-jét és jelszavát, ha megvagyunk SAVE-REBOOT 
gomb megnyomása után megpróbál csatlakozni a hálózathoz. 
Ha a hitelesítő adatok megfeleőek voltal akkot DHCP-n kap ÍP címet és a beállított 
lejátszási listából az első adót automatikusan elkezdi lejátszani.(vagy, ha már volt 
lejátszás akkor a legutolsót) 
Amenyiben hiba történne a hitelesítés alatt, újra AP módba vált és meg kell adni az 
adatokat újra(lehetőleg helyesen). 
4
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Funkciók: 
Magas bitrátájú online streamek lejátszása. 
320X240 pixel felbontású színes érintős TFT kijelző 
Oled óra 24 órás formátum, villogó : másodperc jelővel, datum, névnap és aktuális 
időjárási adatok megjelnítés(hőmérséklet, égbolt ikon) 
2.1-es hangrendszer külön állítható front, mély, hangerő szabályozó potméterekkel. 
Analóg LED-es kivezérlésjelző. 
Erősítő és hangfelvédelemi relék. 
Képernyővédő – stop és beállított idő eltelte után aktíválódik(weben módosítható) 
Beépített 16 GB SD kártya.(nem cserélhető) 
DLNA lejátszó és böngésző funkció. 
DLNA++ Media Renderer funkció az on th fly file átvitelhez windows/android rendszeről. 
Hi-Fi cast, BubbleUpnp app segítségvel. 
5
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Kezelés: 
Kezelés az előlapi tekerő gomb segítségével: 
A rendszer alapvető kezelés a webrádióra van kitalálva. Az előlapon található rotary 
gomb (végtelenül körbefordítható kattintható tekerőgomb) segítségével:  
A tekerőgomb - - - - - - 
tudunk hangerőt növelni, csökkenteni. 
Egyszer röviden megnyomva az aktuális lejátszás szünetel, újbóli megnyomására 
indul a lejátszás. 
Hosszú gombnyomásra a lajátszási lista lesz látható(rádió adók/sd kártyán lévő 
fájlok, dlna szerveren található kiválasztott mappa tartalma). 
Navigálni a tekető forgatásával lehet fel és le irányba. 
Kiválasztás automatikusan 2 mp-után vagy azonnal a forgató gomb  megnyomásával 
lehetséges. 
Két rövid kattintással tudunk módot váltani, sorrendben Rádió - SD palyer - DlNA 
player. 
Amennyiben nincs rádió list, akkor a webszerveren lévő firmware feltöltés ikonra  
kattintva ki lehet tallózni a radió rendszer alap beállított rádió listát. 
6
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Vigyázat ha korábban működött a lista és azt már szerkeszrettük, akkor ez a lépés 
lehetséges, hogy felülírja a változásokat ! 
Amennyiben az SD kártyán nincsennek zene fájlok, akkor a webszerver SD feltöltés 
ikonjára kattintva tudunk zenéket másolni a kártyára, melyből automatikusan lejátszási 
lista készül melyet már meg tud jeleníteni és lejátszani a rendszer. 
DLNA list ha elérhető és a szerver is elérhető abban az esetben a megfelelő lista 
betöltődik és lejátszhatőaok a fájlok. 
Amennyiben nem elérhető a szerver hiba üzenet jelenik meg, hogy a webes felületen 
hatsunk végre szerver keresést,és válasszuk ki a nekünk megfelelő mappát. 
7
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Ezek után már lesz DLNA listánk is, és lejátszhatjuk a szerveren tárolt zenéket. 
Navigáció ugyanúgy mint a web rádió esetében. Tekerő gomb jobbra tekerés fel, balra 
tekerés le kattintás kiválasztás. 
8
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Kezelés az érintőkijelzőn: 
Az érintőkijelző a mellékkelt "tollal" működtethető(. A kijelzőn lévő “gombok”-ra 
kattintva a kívánt funkció elérhető és vagy módosíthatóak. 
Beépített funkciók: 
alsó sor jobbra húzás hangerő fel, 
balra húzás hangerő le.  
dupla kattintás a képernyő közepe felé lejátszás/megállítás 
felhúzás lejátszási lista 
lista görgetése fel vagy lehúzás 
kiválsztás koppintás, 
elfogadás dupla kattintás 
9
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Webszerver funkciói: 
A legmagasabb szintű hozzáféréshez webböngésző szükséges. 
A beépített webszerver elérése a kijlezőn látható ip cím beírásával lehetséges. 
Pl.: http://192.168.1.191 
Rádió player a  főoldal -vezérlőkkel, lejátszási listával - - 
Szerkeszthető az aktuális lista 
a firmware tartalmazz egy rádióplaylistet, ami szükség esetén visszatölthető 
http://aktuálisipcím/webboard címen található vészhelyzeti modul 
segítségével 
10
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
SD player - vezérlőkkel lejátszási listával - 
SD_Manager oldal a fájlok kezeléséhez - feltöltés, lista készítés, törlés. 
Amennyiben az SD módra váltás nem valósul meg, akkor valamilyen hiba léoet 
fel a kártya felcsatolása közben. A rendszer teljes újraindítása utána hibának 
meg kell szűnnie, és a kártyán lévő fájlok újra lejátszahatóak lesznek. 
DLNA tallózó és lejátszó - - - 
az aktuális mappát beteszi egy aktív playlistbe és azonnal elkezdi a lejátszást. 
A keresés és lista készítés több időt vesz igénybe, a weboldalon addig ne 
frissíts, amíg nem végezz a rendszer.  
Amennyiben túl sok fájl van egy adott mappában (<1000) , előfordulhat 
Watchdog reset. és a playlist nem fog elkészülni. Ilyen esetben csökkenteni kell 
a mappában lévő állományok számát. 
11
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Firmware frissítő 
12
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Beállítások 
13
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Rádió kereső 
14
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Történelem: 
Az apósomnak nagyon tetszet a saját DIY webrádión ami egy sima ESP32 YoRadio, 
semmi extrával, csak működik szépen. 
Gondoltam, akkor építek neki is egyet és meglepem vele. 
Viszont az Ő kérése, hogy saját zenéket is le tudjon játszani, ne csak rádió adásokat. 
Ezért gondoltam az ESP32S3-ra, mert jól működő SD kártya kezelése van. 
Megszületett a koncepció, elkészült a 3D terv, megérkeztek az alkatészek. 
Majdnem minden úgy történt ahogy kitaláltam, kivéve: 
Az eredeileg tervezett Bluetooth funkció. Sajnos az ESP32S3 nem támogatja megfelelően 
nem fog működni, így maradt a DLNA. 
Rengeteg próbálkozás, kódolás, javítás után a rendszer működése stabil, minden 
integrált funkció működik. 
15
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Koncepció: 
Cél: 
Egy DIY web rádió építése, saját tervezésű 3d nyomtatott dobozban 
Fontos, hogy egy analóg(ledes) kivezérlésjelző mindenképpen legyen az előlapon !!! 
Funkciók: 
wifi hot spot első beállításhoz 
web szerver helyi eléréshez 
USB/SD zene lejátszási lehetőség 
Bluetooth lejátszási lehetőség 
2.1 hangrendszer(mély külön) 
Érintő kijelzős vezérlés 
Egy gombos rotary encoderes hangerőszabályozás, és vezérlés 
3D nyomtatás: 
Egy egységként kezelendő, mint egy bluetooth hangszóró 
Kijelző és a hangszórók 45 fokban döntve 
Hangszórók külön egység, külön nyomtatható de összeilleszthetően 
Elektronika kivehető tálcán ? 
16
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Koncepció rajz: 
17
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Koncepció AI segítség: 
18
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Alkatrész lista: 
1 db EM-50189 (HEKIT-189) Stereo kivezérlésjelző, 2-soros, logaritmikus 
1 db DFPlayer-16P MP3 lejátszó modul, microSD foglalattal  
1 db ESP32-S3-WROOM-1-N16R8-M ESP32 S3 fejlesztői modul, 16MB Flash, 8MB 
PSRAM, WiFi, Bluetooth 5, USB-C UART, USB-C OTG, microSD foglalat 
1 db MSP2807 2.8" SPI TFT modul, rezisztív érintőkijelző, microSD kártyafoglalattal 
1 db FRONT-ROT-OLED13 Előlapi kezelőpanel modul, 1.3inch OLED kijelzővel, rotary 
encoderrel, 2 gombbal, I2C 
1 db CJMCU-1334 UDA1334A alapú sztereó audio dekóder modul, DAC, I2S 
1 db ESP32-S3-EXP-44P ESP32-S3 kifejtő modul, táp áramkörrel, 44pin, 25.4mm 
1 db STDN-3A24-ADJ 3A állítható step-down DC-DC kapcsolóüzemű tápegység modul, 
1.8V/2.5V/3.3V/5V/9V/12V 
1 db XH-M139  TPA3116D2 sztereo erősítő modul, 2.1 csatornás, 2x50W, 12-24V DC 
2 db hangszóró(valami régi cd lejátszós de nem működő cuccból) 
1 db mélynyomó(ez sajnos oylan kicsi, hogy érdemben nem sokat tesz az élményhez, de 
azért lehet érzékelni, és így pont elég.)  
19
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Hiba elhárítás: - - - - 
A rádió kijelzőjén előfordulhat, hogy a playlist nem frissül megfelelően. Ilyen esetben 
a rotary hosszú megnyomásásra előjön a lista és tekergetés hatására meg fog jelenni 
az aktuális lista. 
Ha a kijelzőn összekavarodna a kijelzés és a playlist, akkor szintén be kell lépni a lista 
kijelzésben és várni amíg vissza tér a fő oldalra, ezzel a hibának meg kell szűnnie. 
SD módra váltás nem történik meg. 
Fájlrendszer vagy mount probléma, teljes tápelvétel, és rendszer újraindítása 
Az OLED-en nem a megfelelő időjárás ikon látszik. A beállított pozíció Békéscsaba, 
az ottani aktuálsi égképhez igazodik a kijelzés, mely eltérhet a lokális égképtől. 
20
Powered by mcjocika  |    
YanO-Radio Felhasználói kézikönyv
Források: 
https://github.com/e2002/yoradio 
https://github.com/VaraiTamas/yoRadio/ 
https://github.com/yellobyte/SoapESP32 
https://chatgpt.com/ 
21
Powered by mcjocika  |    
