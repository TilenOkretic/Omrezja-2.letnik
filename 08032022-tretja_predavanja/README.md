# Omrezja predavanja

## Ponovitev

**Način zapisa signala** določa **fizični sloj**

Za ponovno **pošiljanje podatkov v primeru trčenja podatkov** je odgovoren **linijski sloj** 

Za usmirjanje je odgovoren **mrežni sloj**

---

# Fizični sloj

* kabel
  
  * optični
  
  * električni
    
    * parica: kabel, ki ima dve ali štiri žili, ki sta med seboj prepleteni
    
    * koaksialni kabli

* brezšično
  
  * RF ~ radijski valovi
  
  * IR
  
  * svetloba

<img src=".\2022-03-08-10-10-53-image.png">

Signali so različno dinamični

Hitrost v **baud-ih**:

* **baud** = **število sprememb signala v časovni enoti**

```
imamo 5 bit/s torej:
    NRZ-L: 5 baud
    NRZI-I: 5 baud
    MANCHESTER KODIRANJE: 10 baud
```

<img src=".\2022-03-08-10-22-58-image.png">

**Simbol** predstavlja 2 bita

<img src=".\2022-03-08-10-23-12-image.png">

---

## Fourierov transform

Kako zapistai poljuben signal z **vsoto sinusnih signalov** !!

<img src=".\2022-03-08-10-55-57-image.png">

---

## Nyquistov teorem

$f_{vz}>2*f_{max}$

$C_{max}=2*H*log_{2}V$ [$bit/s$]

* $log_{2}V$     je število $bitov / simbol$

* $V$             je število signalnih nivojev 

Na signal, ki gre po kanalu vplivajo **motnje**

$U_{out} == f_{1}*(U_{in}) + f_{2}*(motnje)$

* $f_{2}*(motnje)$  =~ T

**Rzmerje signal-šum** $S/N$

* obi;ajno ga podajamo v **dB** - decibelih

$S/N$        [dB]

   10             10

  100            20

 1000           30

     .                .

     .                .

----

## Shannonovo pravilo

$C_{max}=H*log_{2}(1 + S/N)$ [bit / s]

* S/N je razmerje => nima enote

---

## Prenos podatkov v višjih frekvenčnih pasovih

###### Aplitudna modulacija (ASK) - AM band

* **nizka amplituda**   = 0

* **visoka amplituda** = 1
  
  <img src=".\2022-03-08-11-38-00-image.png">

###### Frekvenčna modulacija (FSK) - FM band
  <img src=".\2022-03-08-11-43-00-image.png">

###### Fazna modulacija (PSK)
  <img src="./2022-03-08-11-44-00-image.png">

---

## Konstelacijski diagrami
