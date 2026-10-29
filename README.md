## LaTeX-Lauluvihkoeditori

Lauluvihkojen, sisällysluetteloiden ym. tekeminen aina uudestaan Writerilla / vast. dokumenttieditorilla on työlästä. LaTeX:lla luomalla yhden dokumenttipohjan voidaan nyt tuottaa lauluvihkosia kuin vettä vain.

# Vaatimukset

Jotta voit luoda dokumentin, tulee sinulla olla jokin LaTeX-compiler asennettuna koneellesi. Lauluvihkoeditori käyttää myös monia 'valmiita' LaTeX-paketteja, joten varmistu, että nekin on asennettuna koneellesi

Vaihtoehtoisesti voit ladata paketin .zip-muodossaan online-editoriin ([e.g. Overleaf - ](https://www.overleaf.com/)), ja muokata siellä.

Lista dokumentin käyttämistä paketeista ja käyttötarkoituksista alla:

```
graphix.sty // kuvien liittäminen
hyperref.sty // dokumentin sisäiset linkit
geometry.sty // marginaalien säätäminen
multicol.sty // 2-kolumniset sivut
babel.sty // lokalisaatio
blindtext.sty // testaus, ei vaadi tuotantoversiossa

verse.sty // runollisten tekstien säettämiseen ja kirjoittamiseen

titlesec.sty // otsikoiden formatointi
tocloft.sty // sisällysluettelon formatointi
```

# Koostumus

Dokumentti koostuu main.tex -tiedostosta, jossa on määritelty itse dokumentti. Lisänä on laulupankki.sty -pakettitiedosto, johon on kirjoitettu laulut

Lauluja tuodaan vihkoon kustomisoiduilla komennoilla. Lauluille on asetettu formatointisäännöt jo pankkitiedostossa, jolloin ne näkyvät lopullisessa dokumentissa oikein.

# Lyhyesti formatoinnista

- Lalujen otsikot on asetettu ´\section{}´ -komennolla, jolloin sisällysluettelo kasaantuu automaattisesti

- Laulujen säkeistöissä on käytetty ´\needspace{}´ -komentoa, jolloin säkeistöt ei leikkaannu kesken kaiken

- Formatoinnin helpottamiseksi on luotu omia komentoja, ´\cb´ ´\ns{}´ ja ´\poisto{}´. Nämä on selitetty tarkemmin tiedostojen omassa dokumentaatiossa.