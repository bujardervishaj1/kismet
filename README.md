# Kismet

Kismet eshte nje wireless "detektor, nuhates dhe sistem detektues i nderhyrjes (detector, sniffer, and intrusion detection system)". Eshte nje nga veglat open-source me esenciale per profesionistet te sigurise se rrjetave kompjuterike. Mund te perdoret ne platforma te ndryshme duke perfshire Windows, Mac OS X, por Linux eshte nje nga te preferuarat per ekzekutimin e kesaj. Ne e kemi perdorur sistemin operativ macOS BigSur.<br>
Aftesia e modit te monitorimit eshte qenjesore qe Kismet te funksionoj si duhet, sepse e lejon Kismetin te percjelle te gjitha paketat qe i ndegjon jo vetem te ndonje "access point" specifik. Eshte me rendesi per policine, agjencione intelegjence dhe hakerat "black hat" sepse Kismet operon ne qehtesi duket ndegjuar paketat qe shkembehen pa lene ndonje gjurme prapa.<br>
Kismet-i eshte i dizajnuar si klient-server aplikacion, por edhe mund te ekzekutohet si aplikacion "standalone", si server qe mbeshtet nje numer te klientave, dhe poashtu si server me "drone" Kismet qe jane te instaluar ne rrjete, dhe secili e monitoron pjesen hardwerike te wirelesit specifik dhe i dergon paketat ne server.
Dronet Kismet-et jane te "vegjel". Secili e perdore konfigurimet e veta, duke definuar burimin ku do te ndegjoje dhe ku do te i percjell paketat.

# Konfigurimet 
### Per te konfigurar Kismet ne macOS BigSur duhet konfigurimet si me poshte:
Te klonohet kodi nga repository permes komandes: git clone https://www.kismetwireless.net/git/kismet.git<br>
Te behet "run" konfigurimet permes komandes: ./configure<br>
Te kompilohet: make<br>
Te instalohet: sudo make suidinstall<br>

# Perdorimi i Kismet

#### Qe te ndezet Kismet per te ndegjuar duhet shkruar komanda: kismet - c en0 (ku en0 eshte emri i karteles se rrjetit qe do perdoret per te ndegjuar)
![Kismet komanda](https://github.com/bujardervishaj1/kismet/blob/master/6.png)
#### Pas startimit te Kismet navigojmi te http://localhost:2501 ku shfaqet "pop up" per te i vendosur kredencialet
![Kismet komanda](https://github.com/bujardervishaj1/kismet/blob/master/2.png)
