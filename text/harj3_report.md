# Harjoitus 3
Tämän harjoituksen tarkoituksena on tutustuttaa itseni Gittiin, sekä GitHubiin ja niiden käyttöön. Harjoitusta varten olen rakentanut uuden 64-bittisen Xubuntu orja-koneen virtuaaliympäristöön, asentanut siihen saltin, sekä yhdistänyt koneen herrakoneeseen.

Ajoin aluksi perinteisen **'whoami'** -komennon herra-koneelta testatakseni yhteyden. Ajan salt-komennot suoraan orja-koneen ID:tä käyttäen.

	master $ sudo salt 'e005' cmd.run 'whoami'

![whoami screenshot](../images/harj3_001_whoamiprint.png)

Yhteys toimii!

## "Näytä omalla git-varastollasi esimerkit komennoista 'git log', 'git diff' ja 'git blame'"
Olin tähän mennessä tehnyt GitHubiin itselleni uuden repon ja ladannut sinne tämän raportin, sekä aikaisemman screenshotin 'whoami':n tulosteesta. Tämä oli vaatinut useamman commitin, joten päätin tarkastella lokitulostetta ja printata sen uuteen tiedostoon.

	elmo $ git log > ./text/gitlogprint.txt

Seuraavaksi työnsin lokiraportin GitHubiin ja linkitin sen tähän raporttiin.
	
	elmo $ git add . && git commit

	elmo $ git pull && git push

[Linkki lokiraporttiin.](./gitlogprint.txt)

Lokiraportti näyttää kulloisenkin commitin hashin, ajan, commitin suorittajan, sekä kommentin. Ajoin edellisen lauseen kirjoitettuani komennon

	elmo $ git diff

joka näyttää lisäykset tai poistot committien välillä. Komento tulisti [seuraavanlaisen raportin](./runninggitdiff.txt)


