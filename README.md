# linux-palvelimet
linux palvelimet kurssin palautukset (Albert Rashica)

# h1 Oma Linux
Tässä kirjoitin tiivistelmän, missä kävin läpi teorian
## x) Raportin kirjoittaminen ja FSF:Free Software Definition muistiinpanot
- Täsmällinen teksti
- virheen uudelleen luominen
- Freedom to run(F0),Freedom to modify(F1), Freedom to copy(F2), Freedom to distribute(F3)

## a) Linuxin asentaminen
Koska minulla oli jo virtualbox ja Debian 12 live ISO valmiiksi ladattuna, tein uuden VM-koneen omalle raudalle.
Oman raudan specsit ovat CPU 6 ytimen-prosessori, 16GB ram, sekä tarpeeksi tallennustilaa.

### Ensin avasin virtualboxin seuraavasti
![Add file: Upload](virtualbox-avaus.png)
### VM-alkuasetukset
Tässä kohtaa valitsin new ja tein alkuasetukset VM-koneelle. Annoin nimeksi 'linux-palvelimet' VM-koneelle. Versioksi Valitsin Debian (64-bit). Varmistin myös, että "Skip unattended installation" on päällä. Disk Image:n jätin VDI:ksi.
![Add file: Upload](virtualbox-alkuasetukset.png)
### Vram-muistin alustava sijoitus
Laitoin että VM saa tarpeeksi näyttömuistia. Laitoin myös grafiikkakontrolleriksi VBoxSVGA.
![Add file: Upload](virtualbox-nayttomuisti.png)
### ISO-levystä asennus
Tässä sitten suoritin VM-koneen installerin, jotta sain Debian 12 live asennettua.
![Add file: Upload](virtualbox-iso-installer.png)
### Asennuksen viimeistely
Tässä sitten viimeistelin asennuksen ja annoin Guest-hostille nimeksi 'linux-palvelimet'. Annoin root-salasanat ja käyttäjätunnukset käytettäväksi. Käytin Guided disk, eli koko virtuaalinen levy käytettäväksi.
![Add file: Upload](virtualbox-viimeistely.png)
#### Huomio!
Varmistin myös että käytettiin Network Mirroria, jotta saa apt-paketit käyttäytymään oikein. On kokemusta kun olen ennen tehnyt tätä virhettä.

## asennuksen jälkeen
Asennuksen jälkeen kirjauduin Root-käyttäjänä ja lisäsin itseni eli käyttäjän bgx106 sudo-ryhmään. Varmistin myös että kaikki paketit olivat uusimpia ja päivitin ne. Tässä ovat ne seuraavat komennot.
```usermod -aG sudo bgx106```
```sudo apt update && sudo apt upgrade -y```
![Add file: Upload](debian12-sudo-usermod.png)
Tämän jälkeen uskoin että kaikki on nyt ok ja aloitin tehtävän palauttamisen.

## Palautus
Tehtävän palautin "app.terokarvinen.com" osoitteeseen.

