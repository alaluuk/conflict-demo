# conflict-demo

## Git merge paikallisesti

Jos sinulla on oma branch (esim. hotfix1) kesken ja toiset opiskelijat ovat päivittäneet GitHubin mainin, tee näin
<ol>
<li>Kommitoi branch hotfix1</li>
<li>Siirry mainiin = git checkout main</li>
<li>Vedä uusin main GitHubista = git pull origin main</li>
<li>Siirry hotfix1 branchiin = git checkout hotfix1</li>
<li>Anna komento = git merge main</li>
</ol>

Edellä siis yhdistät uudet mainin ominaisuudet hotfix1:een ja voit jatkaa työskentelyä.

## Git konflikti voi syntyä:

<ol>
<li>PAIKALLISESTI: main on päivitetty GitHubiin ja haet sen pull komennolla. Sen jälkeen mergellä yhdistät mainin omaan branchiisi, mutta jossakin tiedostossa on jollakin rivillä eroa verrattuna sinun branchin tiedostoon.</li>

<li>GITHUBISSA: main on päivitetty jonkin PullRequestin jälkeen. Nyt joku toinen puskee oman branchin, mutta hänellä ei ollut uusin versio mainista. Kun nyt yritetään tehdä "merge" mainiin, tulee mahdollisesti konflikti.</li>
</ol>

## Konflictin ratkaisu

Konflikti on helpoin ratkaista VsCodella tai QtCreatorilla, koska ne näyttävät selkeästi kongliktirivit.
