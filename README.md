
Wifi web rádió


	A webrádió kizárólag internetes streamek lejátszására képes.

	Önnállóan, Wi-Fi és internet hiányában nem működik !

	Támogatott Wi-Fi szabvány: 2,4 GHz
  
<img width="756" height="482" alt="Render" src="https://github.com/user-attachments/assets/8f474802-53bd-4fce-999c-9da3566688f6" />


Funkciók:

	Magas bitrátájú online streamek lejátszása.
	
	320X240 pixel felbontású színes érintős TFT kijelző

	Oled óra 24 órás formátum, villogó : másodperc jelővel.

	2.1 hangrenszer külön állítható Front Mély Hangerő szabályozó potméterekkel.
	
	Analóg LED-es kivezérlésjelző.

	Erősítő és hangfelvédelem.
	
	Képernyővédő
	
	Beépített 16 GB SD kártya.
	
	DLNA lejátszó és böngésző funkció.

	DLNA++ Media Renderer funkció az on th fly file átvitelhez windows/android rendszeről. 
	- Hi-Fi cast, BubbleUpnp app segítségvel.

<img width="2432" height="1816" alt="kijelző" src="https://github.com/user-attachments/assets/fa804c5f-bae4-49a0-9fde-848a78204a54" />
<img width="1817" height="820" alt="oled" src="https://github.com/user-attachments/assets/c87a6f3f-2148-459e-939e-8cc58540ddc7" />
<img width="2384" height="1624" alt="erősítő" src="https://github.com/user-attachments/assets/a09db8cd-7735-49b6-b620-c8fe8fb3c9f2" />	
	


Kezelés az előlapi tekerő gomb segítségével:


	A rendszer alapvető kezelés a webrádióra van kitalálva. Az előlapon találhato rotary gomb (végtelenül körbefordítható kattintható tekerőgomb) segítségével.
	tudunk hangerőt növelni, csökkenteni.
	
		Egyszer röviden megnyomva az aktuális lejátszás szünetel, újbóli megnyomására indul a lejátszás.

		Hosszú gombnyomásra a lajátszási lista lesz látható(rádió adók/sd kártyán lévő fájlok, dlna szerveren található kiválasztott mappa tartalma).
	
	Navigálni a tekető forgatásával lehet fel és le irányba.
	
	Kiválasztás automatikusan 2 mp-után vagy azonnal a forgató gomb megnyomásával lehetséges.
	

		Két rövid kattintással tudunk módot váltani, sorrendben Rádió - SD palyer - DlNA player.
	
			Amennyiben nincs rádió list, akkor a webszerveren lévő firmware feltöltés ikonra kattintva ki lehet tallózni a radió rendszer alap beállított rádió listát.
			Vigyázat ha korábban működött a lista és azt már szerkeszrettük, akkor ez a lépés lehetséges, hogy felülírja a változásokat !
	
			Amennyiben az SD kártyán nincsennek zene fájlok, akkor a webszerver SD feltöltés ikonjára kattintva tudunk zenéket másolni a kártyára, melyből automatikusan lejátszási lista készül melyet már meg tud jeleníteni és lejátszani a rendszer.
		
			DLNA list ha elérhető és a szerver is elérhető abban az esetben a megfelelő lista betöltődik és lejátszhatőaok a fájlok.
			Amennyiben nem elérhető a szerver hiba üzenet jelenik meg, hogy a webes felületen hatsunk végre szerver keresést,és válasszuk ki a nekünk megfelelő mappát.
			Ezek után mát lesz DLNA listánk is, és lejátszhatjuk a szerveren tárolt zenéket.

		Navigáció ugyanúgy mint a web rádió esetében. Tekerő gomb jobbra tekerés fel, balra tekerés le kattintás kiválasztás.
	
	
Kezelés az érintőkijelzőn:


	Az érintőkijelző a mellékkelt "tollal" működtethető(. A kijelzőn lévő gombok-ra kattintva a kívánt funkció elérhető és vagy módosíthatóak.
	
	Beépített funkciók:
						alsó sor jobbra húzás hangerő fel,
						balra húzás hangerő le. 
						dupla kattintás a képernyő közepe felé lejátszás/megállítás
						felhúzás lejátszási lista
						lista görgetése fel vagy lehúzás
						kiválsztás koppintás,
						elfogadás dupla kattintás

 

Webszerver funkciói:

	A legmagasabb szintű hozzáféréshez webböngésző szükséges.
	A beépített webszerver elérése a kijlezőn látható ip cím beírásával lehetséges. Pl:http://192.168.1.191

	Rádió player a  főoldal -vezérlőkkel, lejátszási listával
		Szerkeszthető az aktuális lista
	SD player - vezérlőkkel lejátszási listával
		SD_Manager oldal a fájlok kezeléséhez - feltöltés, lista készítés, törlés
	DLNA tallózó és lejátszó
		az aktuális mappát beteszi egy aktív playlistbe és azonnal elkezdi a lejátszást.
	
	Lista szerkesztő
	SD kártya kezelő
	Firmware frissítő
	Beállítások
	Rádió kereső

<img width="495" height="823" alt="playerweb" src="https://github.com/user-attachments/assets/cb7379b2-d6b2-4a37-85ae-6724d369fbeb" />


Források: 

	https://github.com/e2002/yoradio

	https://github.com/VaraiTamas/yoRadio/

	https://github.com/yellobyte/SoapESP32

	https://chatgpt.com/

3D fájlok:

	https://www.printables.com/model/1627343-yano-radio



