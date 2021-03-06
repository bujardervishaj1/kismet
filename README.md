# Kismet

Kismet eshte nje wireless "detektor, nuhates dhe sistem detektues i nderhyrjes (detector, sniffer, and intrusion detection system)". Eshte nje nga veglat open-source me esenciale per profesionistet te sigurise se rrjetave kompjuterike. Mund te perdoret ne platforma te ndryshme duke perfshire Windows, Mac OS X, por Linux eshte nje nga te preferuarat per ekzekutimin e kesaj vegle. Ne e kemi perdorur sistemin operativ macOS BigSur.<br>
Aftesia e modit te monitorimit e karteles se rrjetit eshte qenjesore qe Kismet te funksionoj si duhet, sepse e lejon Kismetin te percjelle te gjitha paketat qe i ndegjon jo vetem te ndonje "access point" specifik. Eshte me rendesi per policine, agjencione intelegjence dhe hakerat "black hat" sepse Kismet operon ne qetesi duket degjuar paketat qe shkembehen pa lene ndonje gjurme prapa.<br>
Kismet-i eshte i dizajnuar si klient-server aplikacion, por mundet te ekzekutohet dhe si aplikacion "standalone", si server qe mbeshtet nje numer te klientave, dhe poashtu si server me "drone" Kismet qe jane te instaluar ne rrjete, dhe secili e monitoron pjesen hardwerike te wirelesit specifik dhe i dergon paketat ne server.
Dronet Kismet-et jane te "vegjel". Secili e perdore konfigurimet e veta, duke definuar burimin ku do te ndegjoje dhe ku do te i percjell paketat.

# Konfigurimet 
### Per te konfigurar Kismet ne macOS BigSur duhet konfigurimet si me poshte:
* Te klonohet kodi nga repository permes komandes: git clone https://www.kismetwireless.net/git/kismet.git<br>
* Te behet "run" konfigurimet permes komandes: ./configure<br>
* Te kompilohet: make<br>
* Te instalohet: sudo make suidinstall<br>

# Perdorimi i Kismet

#### Qe te ndezet Kismet per te degjuar duhet shkruar komanda: kismet - c en0 (ku en0 eshte emri i karteles se rrjetit qe do perdoret per te degjuar, emertimi i karteles mundet te dalloj nga sistemi operativ)
![Kismet komanda](https://github.com/bujardervishaj1/kismet/blob/master/6.png)
#### Pas startimit te Kismet navigojme te http://localhost:2501 ku shfaqet "pop up" per t'i vendosur kredencialet
![Kismet kredencialet](https://github.com/bujardervishaj1/kismet/blob/master/2.png)
#### Ne "interface" mund te konfigurohen "settings" te ndryshem si ne fotot me poshte
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/3.png)
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/4.png)
Kismet ka disa opsione kur mberrijme te prezentimi i te dhenave. Se pari mund te zgjedhim se cilat informata dojme qe te shfaqen ne interface (P.Sh. SSID, BSSID, CHANEL, Encryption, etj.), gjithashtu mund te zgjedhim nese dojme qe ta sortojme vargun e informatave qe na jep kismet, ne baze te ndonjeres nga kolonat e shfaqura ne figuren.<br>
Gjithashtu njera nder mundesite qe ofron kismet eshte paraqitja e GPS lokacioneve te paisjeve qe jane duke zhvilluar trafik.
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/5.png)

#### Pas startimit mund te percillen paketat qe shkembehen ne rrethinen ku eshte duke degjuar Kismet
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/11.gif)
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/12.png)

##### Nese percjellim nje paisje specifike mund te shohim te dhenat per te si me poshte 
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/9.png)
![Kismet](https://github.com/bujardervishaj1/kismet/blob/master/10.png)
<br>
Njera pike interesante qe vlene te ceket eshte gjetja e "Access points" te cilet SSID nuk jane duke e bere "broadcast", d.m.th. kismet mund qe ti identifikoje edhe ato "Access points" te cilet nuk kane ndonje emer si dhe mund ti monitoroje, kjo vlene te ceket pikerisht se "Access points" te cilet jane hidden jane me me interes qe te investigohen! 

## Kontribuesit

1. Bujar Dervishaj
2. Jon Klinaku
3. Urim Zymberi

# Referencat
* https://www.kismetwireless.net/docs/howto/osx/?fbclid=IwAR0Zlsa9ANCsrC87BIW-ty4U-SDGiCQvnPWX00aSBp_zqKzDnFZrcuahnfs
* https://www.kismetwireless.net/docs/readme/starting_kismet/?fbclid=IwAR3xMFBk9IZqs8_Yq4nRSknqU6GsD9tREIWoFOB9k1eiuso6J2wIhLq3M9s
* https://www.linux.com/news/introduction-kismet-packet-sniffer/?fbclid=IwAR0pGM8ib6N3LC-4QEjPYOtCjB1-E9OXNve4d6aWU_9mA6P7IJ7T1zrgeDo

