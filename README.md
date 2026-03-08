
!!! Figyelem !!!

	Ez a verzió kizárólag az esp32-s3-devkitc1-n16r8 44 lábú modulhoz és

	- ILI9341 320x240 felbontású SPI (LCD)

	kijelzőhöz készült és csak az audioI2S DAC eszközzel működik megfelelően, [PCM5102A](PCM5102A) -val tesztelve!

	- Nem támogatja az ESP32-t PSRAM memória nélkül.

Ez a konfiguráció néhány további könyvtártól függ. Kérlek, telepítsd őket a könyvtárkezelővel vagy PlatformIO(AJÁNLOT!) esetén használd a mellékelt platformio.ini fájlt.
	
	adafruit/Adafruit GFX Library@^1.12.3
    adafruit/Adafruit ILI9341@^1.6.2
    ;paulstoffregen/XPT2046_Touchscreen@0.0.0-alpha+sha.26b691b2c8
    adafruit/RTClib@^2.1.4
    ;moononournation/GFX Library for Arduino@^1.4.7 ;only for Gution & GC9A01 onboard ESP
    ;adafruit/Adafruit CST8XX Library ;only for GC9A01 onboard ESP
    olikraus/U8g2 @ ^2.35.19
    ; --- DLNA browser (SoapESP32) + DLNA MediaRenderer ---
    yellobyte/SoapESP32@^1.4.1
    https://github.com/pschatzmann/arduino-dlna.git

Nyelvek, teruleti beallitasok:

	Aprogram beépített nyelveket és területi beállításokat tartalmaz HU, PL, GR, EN, RU, NL, SK, UA, DE nyelveken.   
	A myoptions.h fájlban az alábbi paranccsal állíthatod be.   
	#define L10N_LANGUAGE HU

	A program az Adafruit_GFX librarit használja, ahol egy 5x7 pixel méretű fontot skáláz fel a kért méret függvényében. Ez a font a glcdfont.c fájlban van megrajzolva.    
	A fájlok helye:     
	PlatformIO esetén a \yoRadio\\.pio\libdeps\esp32-s3-devkitc1-n16r8\Adafruit GFX Library\glcdfont.c

Ha nálad nem jelennek meg helyesen a karakterek, akkor ezt a fájlt le kell cserélni a nyelvedhez tartozó fájlra. A WiFi kijelzés és hangszóró kijelzés helytelenül jelenik meg, valamint azoknál a nyelveknél, melyek az angoltól eltérő karakterkészletet használnak (ékezetest), különböző a nyelvekhez szerkesztett fájlt kell használni és arra lecserélni az eredetit.
Ezek itt találhatóak a programban:

      yoRadio/locale/glcdfont/EN, NL, CZ/glcdfont.c
      yoRadio/locale/glcdfont/GR/glcdfont.c
      yoRadio/locale/glcdfont/HU, DE/glcdfont.c
      yoRadio/locale/glcdfont/PL, SK, DE/glcdfont.c
      yoRadio/locale/glcdfont/RU/glcdfont.c
      yoRadio/locale/glcdfont/UA/glcdfont.c

A myoptions.h fájlban beállított pin-ek ajánlottak a helyes működéshez.

A névnapok tárolása az alábbi fájlokban történik.

      local/namedays/namedays_HU.h
      local/namedays/namedays_PL.h
      local/namedays/namedays_GR.h  
      local/namedays/namedays_DE.h

Ha más nyelven szeretnéd használni vedd fel velem a kapcsolatot.

	Ha nem szeretnéd megjeleníteni, akkor kommenteld ki a sort,    
	// #define NAMEDAYS_FILE HU   
	vagy a WEB-es felületen kikapcsolható options/tools-> Namedays gombbal.

Wi-Fi web rádió

![20260307_091635-ANIMATION (2)](https://github.com/user-attachments/assets/178ce886-e70d-478f-87d8-cc7de209b08f)


![myradio (1) (1) (1)](https://github.com/user-attachments/assets/3dcf2011-83cd-415f-97e0-0de0eaf098bf)


https://www.youtube.com/watch?v=gppzjGApgt8


<img width="800" height="600" alt="szólarádio" src="https://github.com/user-attachments/assets/853d9433-2151-4788-a318-95719ffab846" />

		
	A webrádió kizárólag vezeték nélküli hálózat megléte esetén működik!

	Támogatott Wi-Fi-szabvány: 2,4 GHz
  
Funkciók:

	Magas bitrátájú online streamek lejátszása.
	
	320 × 240 pixeles felbontású, színes, érintős TFT-kijelző.

	OLED-óra 24 órás formátumban, villogó másodpercjelzővel.

	2.1 hangrendszer, külön állítható front- és mélyhangerő-szabályzó potméterekkel.
	
	Analóg LED-es kivezérlésjelző.

	Erősítő- és hangfalvédelem.
	
	Képernyővédő.
	
	Beépített 16 GB-os SD-kártya.
	
	DLNA-lejátszó és böngészőfunkció.

	DLNA++ Media Renderer funkció az on-the-fly fájlátvitelhez Windows/Android rendszerről. 
	- Hi-Fi Cast, BubbleUPnP alkalmazások segítségével.

<img width="800" height="600" alt="kijelző" src="https://github.com/user-attachments/assets/fa804c5f-bae4-49a0-9fde-848a78204a54" />
<img width="800" height="600" alt="oled" src="https://github.com/user-attachments/assets/c87a6f3f-2148-459e-939e-8cc58540ddc7" />
<img width="800" height="600" alt="erősítő" src="https://github.com/user-attachments/assets/a09db8cd-7735-49b6-b620-c8fe8fb3c9f2" />	
	


Kezelés az előlapi tekerőgomb segítségével:


	A rendszer alapvető kezelése a webrádió használatára lett kialakítva. Az előlapon található rotary gomb (végtelenül körbefordítható, kattintható tekerőgomb) segítségével
	tudunk hangerőt növelni és csökkenteni.
	
		Egyszer röviden megnyomva az aktuális lejátszás szünetel, újbóli megnyomására újraindul a lejátszás.

		Hosszú gombnyomásra a lejátszási lista lesz látható (rádióadók, SD-kártyán lévő fájlok, DLNA-szerveren található kiválasztott mappa tartalma).
	
	Navigálni a tekerő forgatásával lehet fel és le irányba.
	
	Kiválasztás automatikusan 2 mp után, vagy azonnal a forgatógomb megnyomásával lehetséges.
	

		Két rövid kattintással módot lehet váltani, sorrendben: Rádió – SD player – DLNA player.
	
			Amennyiben nincs rádiólista, akkor a webszerveren lévő firmware-feltöltés ikonra kattintva ki lehet tallózni a rádiórendszer alapértelmezett rádiólistáját.
			Vigyázat! Ha a lista korábban már működött, és azt szerkesztettük, akkor ez a lépés felülírhatja a változtatásokat.
	
			Amennyiben az SD-kártyán nincsenek zenefájlok, akkor a webszerver SD-feltöltés ikonjára kattintva tudunk zenéket másolni a kártyára, amelyekből automatikusan lejátszási lista készül, melyet a rendszer már meg tud jeleníteni és le tud játszani.
		
			Ha a DLNA-lista elérhető, és a szerver is elérhető, akkor a megfelelő lista betöltődik, és a fájlok lejátszhatók.
			Amennyiben a szerver nem elérhető, hibaüzenet jelenik meg, hogy a webes felületen hajtsunk végre szerverkeresést, és válasszuk ki a nekünk megfelelő mappát.
			Ezek után már lesz DLNA-listánk is, és lejátszhatjuk a szerveren tárolt zenéket.

		A navigáció ugyanúgy működik, mint a webrádió esetében: a tekerőgomb jobbra forgatásával felfelé, balra forgatásával lefelé léphetünk, kattintással pedig kiválaszthatunk.
	
	
Kezelés az érintőkijelzőn:


	Az érintőkijelző a mellékelt "tollal" működtethető. A kijelzőn lévő gombokra kattintva a kívánt funkció elérhető, illetve módosítható.
	
	Beépített funkciók:
						alsó sor jobbra húzás: hangerő fel,
						balra húzás: hangerő le, 
						dupla kattintás a képernyő közepe felé: lejátszás/megállítás,
						felhúzás: lejátszási lista,
						listagörgetés fel- vagy lehúzással,
						kiválasztás: koppintás,
						elfogadás: dupla kattintás

 

Webszerver funkciói:

	A legmagasabb szintű hozzáféréshez webböngésző szükséges.
	A beépített webszerver elérése a kijelzőn látható IP-cím beírásával lehetséges. Pl.: http://192.168.1.191

	Rádió player a főoldalon, vezérlőkkel és lejátszási listával.
		Szerkeszthető az aktuális lista.
	SD player vezérlőkkel és lejátszási listával.
		SD Manager oldal a fájlok kezeléséhez – feltöltés, listakészítés, törlés.
	DLNA tallózó és lejátszó.
		Az aktuális mappát beteszi egy aktív playlistbe, és azonnal elkezdi a lejátszást.
	
	Listaszerkesztő.
	SD-kártyakezelő.
	Firmware-frissítő.
	Beállítások.
	Rádiókereső.

<img width="495" height="823" alt="playerweb" src="https://github.com/user-attachments/assets/cb7379b2-d6b2-4a37-85ae-6724d369fbeb" />


Források: 

	https://github.com/e2002/yoradio

	https://github.com/VaraiTamas/yoRadio/

	https://github.com/yellobyte/SoapESP32

	https://chatgpt.com/

3D fájlok:

	https://www.printables.com/model/1627343-yano-radio
