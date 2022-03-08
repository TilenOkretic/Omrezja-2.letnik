# Omrezja predavanja 
## <-Komunikacija v racunalniskih omrezjih->

#### Primer dveh filozofov:
* Dva filozofa ki zivita na dveh koncih sveta
  * npr. Francija in drugi na japonskem
* med njima je nekaj ovir
  * razdalja, casovni zamik, jezik
* Potrebujeta prevajalca
* potrebni sta tajnici
```
  FR FILOZOF                   JP FILOZOF
    |                             |
    |                             |
    v                             |
  FR PREVAJALEC               JP PREVAJALEC
    |                             |
    |                             |
    V                             |
  TAJNICA --------------------> TAJNICA
```
* **Sloji** in vmesniki (za komunikacijo med sloji)
* **Vmesniki** so lahko različni
* Vendar si med seboj morajo določiti neka komunikacijska pravila (**PROTOKOLI**)

## Lastnosti računalniških omrežjih
* Komunikacijski medij
* Multipleksiranje
* Kodiranje podatkov
* Posredovanje podatkov med ne direktno povezanimi napravami

## Referenčni modeli
* **TCP/IP** referencni model
  * TCP in IP sta dva glavna protokola na internetu
* **ISO OSI** referencni model
  * veliko bolj sistematicen
  * razdeli arhitekturo na 7 slojev

## 1. sloj: FIZIČNI SLOJ
  * **bit** je osnovna enota za posiljanje preko komunikacijskega medija
  * prisotne so motnje
  
## 2. sloj: PODATKOVNO LINIJSKI SLOJ
  * komunikaciranje z uporabo **OKVIRJEV**
  * naprava ki zeli poslati en okvir bo za to uporabila fizicni sloj
  * MAC naslovi, vsaka naprava ima svoj unikaten MAC naslov


HOST - SUBNET  END HOST
      /         /
     Router - /

## 3. sloj: Mrezni sloj 
  * IP naslovi
  * podatkovna enota mreznega sloja je **PAKET** (lahko zapisemo v en ali ga razdelimo in posljemo preko vec okvirjev)

* Zakaj je zaneslivost problem? 
  * Tezava je lahko v tem da je omrezje zasiceno (prenapolnjeno)
  * Lahko se zgodi da nekateri paketi ne pridejo od posiljatelja do prejemnika 
  * Omrezje ni zanesljivo

## 4. sloj: TRANSPORTNI SLOJ
* Tega sloja ni na usmerjevalnikih
* Zagotavlja zanesljivost, da bodo podatki prisli
* potrebujemo številčenje na paketih
* potrebujemo dodati dodatno glavo 
* **SEGMENT**

## 5. sloj: SEJNI(SESSION) SLOJ
* omogoca da razdelimo podatke glede na vec potreb
* razlicni kanali med napravami
* 

## 6. sloj: PREDSTAVITVENI SLOJ
* namenjen je predstavitvi podatkov, to pomoni reci kot so npr. kompresiranje podatkov, šifriranje podatkov, ...
* tega sloja internet v osnovi nima

## 7. sloj: APLIKACIJSKI SLOJ
* pravila komuniciranje z in med aplikacijami
* imamo tudi neke standardne protokole npr. HTTP protokol

## Razlike med ISO/OSI in TCP/IP
* V TCP/IP je:
* predstavitveni sloj je del aplikacijskega sloja
* sejni sloj je del transportnega sloja
* mrezni, podatkovno linijski in fizicni sloj so skupaj
* potrebujemo en dodaten pod-sloj za dostop do medija ~ **MEDIUM ACCESS CONTROL**

* Ko posiljamo podatke iz aplikacijskega sloja med aplikacijami potrebujemo se neke dodatne podatke 

* Ko komuniciramo med sloji potrebujemo poslati **koristne podatke** in **kontrolne podatke**, lahko dodamo se dodatne podatke

## PROTOKOLI
* HTTP - aplikacijski sloj
* TCP in UDP - transportni sloj
* IP - mrezni sloj <-kolekcija pravil za usmirjanje po internetu->

## Zaporedje bitov v fizicnem sloju
* | [     MAC1     ][     MAC2     ][IP1, IP2  ][          3000:80          ][GET ...         ] |
* | [naslovi nas in usmirjevalnika ][IP naslovi][transportni sloj doda glavo][Koristni podatki] |

## **NEPOVEZAVNA** omrežja in **POVEZANA** omrežja
* **QOS** - kakovost storitev
* UDP je manj zanesljiv



























