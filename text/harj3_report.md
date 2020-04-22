# Harjoitus 3
Tämän harjoituksen tarkoituksena on tutustuttaa itseni Gittiin, sekä GitHubiin ja niiden käyttöön. Harjoitusta varten olen rakentanut uuden 64-bittisen Xubuntu orja-koneen virtuaaliympäristöön, asentanut siihen saltin, sekä yhdistänyt koneen herrakoneeseen.

Ajoin aluksi perinteisen **'whoami'** -komennon herra-koneelta testatakseni yhteyden. Ajan salt-komennot suoraan orja-koneen ID:tä käyttäen.

	master $ sudo salt 'e005' cmd.run 'whoami'

![whoami screenshot](../images/harj3_001_whoamiprint.png)
