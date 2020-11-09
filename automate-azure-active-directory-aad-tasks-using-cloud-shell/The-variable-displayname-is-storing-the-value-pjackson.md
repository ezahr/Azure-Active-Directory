

![automate-azure-active-directory-aad-tasks-using-cloud-shell/](https://www.sqlshack.com/automate-azure-active-directory-aad-tasks-using-cloud-shell/)


## displayname=pjackson

The variable displayname is storing the value “pjackson”. You can verify the value of the variable using the echo command like this:

## Echo $displayname

We will now read user input and store in a variable named password. To do that, run the following command:

## read password

After that, you can write the password, which will be stored in the password variable.

To concatenate values, you just need to write the string together:

## userprincipalname=$displayname@dani671hotmail.onmicrosoft.com

In this example, we are concatenating the variable $dispalyname with the string “@dani671@hotmail.onmicrosoft.com”.

The following example, will use the variables to create a new user:

## az ad user create –display-name $displayname –password $password –user-principal-name $userprincipalname


## Create multiple Azure Active Directory users from a test file

In the next example, we will create a list of users and we will create AAD users from that list automatically.
We will first create a file named “listuser”. The first line will be ”jlopez”, which is an AAD user that we want to create:

echo “jlopez” > listusers
We will append two more lines to the text file:
echo “dtrump” >> listusers
echo “bobama” >> listusers

You can also specify a password:
read password

The following lines of code will read the file listuser. It will create a user for each line of the file.:

````
cat listusers | while read line
do
az ad user create –display-name $line –password $password –user-principal-name $line@dani671hotmail.onmicrosoft.com
done 
`````

|user|@bdmcc.net|
|---------------------|-----------------------------|
|Alex Smits | alex.smits@bdmcc.net|
|Alexandra Brouwershaven | as.van.brouwershaven@bdmcc.net|
|Alfred Pruim | a.pruim@bdmcc.net|
|Almar Diehl |a.diehl@bdmcc.net|
|Andre Vlaardingerbroek | a.vlaardingerbroek@bdmcc.net|
|Andy van den Biggelaar | andy.van.den.biggelaar@bdmcc.net|
|Anja Boonstra de Boer | a.boonstra-de.boer@bdmcc.net|
|Arian Geertsema | a.geertsema@bdmcc.net|
|Arthur Rijke | arthur.rijke@bdmcc.net|
|Asare Twum | a.twum@bdmcc.net|
|Barend Tempelman | b.tempelman@bdmcc.net|
|Bart Heijenk | bd.heijenk@bdmcc.net|
|Ben Beijer | b.beijer@bdmcc.net|
|Bert Harmsen | b.harmsen@bdmcc.net|
|Bianca Averink | b.averink@bdmcc.net|
|Bianca Tijssen-van Gelder | b.tijssen-van.gelder@bdmcc.net|
|Bram Duvigneau | bram@bdmcc.net|
|Brenno de Winter | brenno@bdmcc.net|
|Cameron MC Gorian | cameron@bdmcc.net|
|Caner Bektas | c.bektas@bdmcc.net|
|Cara Koesoemo | cara.koesoemo@bdmcc.net|
|Casper Meijerink | casper.meijerink@bdmcc.net|
|Chi Hon Choi | ch.choi@bdmcc.net|
|Chris Baas | c.baas@bdmcc.net|
|Chris Timmermans | cma.timmermans@bdmcc.net|
|Christiaan Veeningen | c.veeningen@bdmcc.net|
|Cindy Babis | cindy.babis@bdmcc.net|
|Clarinda Moonen | cm.moonen@bdmcc.net|
|cm de Jongh | cm.d.jongh@bdmcc.net|
|Danai van Lith | Danai.van.Lith@bdmcc.net|
|Danny Pluim | d_pluim@bdmcc.net|
|Danny van Luijpen | d.van.luijpen@bdmcc.net|
|Debby Huijsmans | d.huijsmans@bdmcc.net|
|Dennis Boehmer | d.boehmer@bdmcc.net|
|Dennis Kramer | dennis@bdmcc.net|
|Dennis Matthijsen | d.matthijsen@bdmcc.net|
|Dennis Roozemond | da.roozemond@bdmcc.net|
|Diane de Joode | diane-de.joode@bdmcc.net|
|Dick Blaauw | h.r.blaauw@bdmcc.net|
|Diego Marcon | dm.marcon@bdmcc.net|
|Dion Oude Spraakste | dtj.oude.spraakste@bdmcc.net|
|Dirk-Willem van Gulik | dirkx@bdmcc.net|
|Dominick Nijboer | d.nijboer@bdmcc.net|
|Don van Meel | don.van.meel@bdmcc.net|
|Douwe van der Galien | douwe.van.der.galien@bdmcc.net|
|Edo Plantinga | edo@bdmcc.net|
|Edwin Croes | ec.croes@bdmcc.net|
|Eghbol Sarwar | e.sarwar@bdmcc.net|
|Emiel Janson | hello@bdmcc.net|
|Eric Reijnders | eha.reijnders@bdmcc.net|
|Eric Verheul | eric.verheul@bdmcc.net|
|Eric Visser | ep_visser@bdmcc.net|
|Erica van Kempen | ej.van.kempen@bdmcc.net|
|Erik Goverde | e.goverde@bdmcc.net|
|Erik Henricks | eha.henricks@bdmcc.net|
|Erik Holkers | e.h.holkers@bdmcc.net|
|Erik te Boome | hjm.te.boome@bdmcc.net|
|Evelien Wolters | e_wolters@bdmcc.net|
|Evert Jan Elings | ej.elings@bdmcc.net|
|Ewoud Koster | e.koster@bdmcc.net|
|ezrah.ligthart.schenk | ezrah.ligthart.schenk@bdmcc.net|
|F. Sevinc | f.sevinc@bdmcc.net|
|F.L. Aries | fl.aries@bdmcc.net|
|Fatma Kilinc | fz.kilinc@bdmcc.net|
|Frans Lexis | fhm.lexis@bdmcc.net|
|Fred Both | f.both@bdmcc.net|
|Fred Bruins | fej.bruins@bdmcc.net|
|Freek Riegman | fa.riegman@bdmcc.net|
|Funs Janssen | f.janssen@bdmcc.net|
|Gemma Mooij | Gemma.mooij@bdmcc.net|
|Gerbrant van den Hengel | g.vandenhengel@bdmcc.net|
|Gerwin Veenhuizen | gwg.veenhuizen@bdmcc.net|
|Gianni Castaldi | Gianni.castaldi@bdmcc.net|
|H.J. van Haastert | hj.v.haastert@bdmcc.net|
|Hamid Ouaali | h.ouaali@bdmcc.net|
|Hans-Peter Los | jh.los@bdmcc.net|
|Hans Schaap | h.schaap@bdmcc.net|
|Hans Versteeg | Hans.Versteeg@bdmcc.net|
|HansRob Reus | HansRob.Reus@bdmcc.net|
|Harald Lammers | h.lammers@bdmcc.net|
|Hendrik Jan Schuurkamp | hj.schuurkamp@bdmcc.net|
|Henri Hoekerd | hj.hoekerd@bdmcc.net|
|Henri ter Hofte | h.ter.hofte@bdmcc.net|
|Hidde Schultze | hidde.schultze@bdmcc.net|
|Hugo Visser | hugo@bdmcc.net|
|Huib Schopman | hha.schopman@bdmcc.net|
|Ilias El Gris | i.el.gris@bdmcc.net|
|Ingrid van Buuren | ib.v.buuren@bdmcc.net|
|Iris Hekkelman | iv.hekkelman@bdmcc.net|
|Ivo Jansch | ivo@bdmcc.net|
|Ivo Kepers | ihcj.kepers@bdmcc.net|
|J. Biesboer | j.biesboer@bdmcc.net|
|J.C. Hoorenman | jc.hoorenman@bdmcc.net|
|J.E. Slot | je.slot@bdmcc.net|
|J.M. Schmitz | jm.schmitz@bdmcc.net|
|Jan Quist | jan.quist@bdmcc.net|
|Jan Tanis | j.tanis@bdmcc.net|
|Jarst Faber | jarst.faber@bdmcc.net|
|Jasper Boerkoel | j.boerkoel@bdmcc.net|
|Jasper Hausen | jasper@bdmcc.net|
|jasperhupkens@bdmcc.net | Member|
|Jasper Tangermann | j.tangermann@bdmcc.net|
|Jasper Verbeek | jg.verbeek@bdmcc.net|
|Jay Richardson | jm.richardson@bdmcc.net|
|Jay Verkouteren | ja.verkouteren@bdmcc.net|
|Jelle Prins | jelleprins@bdmcc.net|
|Jeroen Dijkgraaf | j.dijkgraaf@bdmcc.net|
|Jeroen Hogendoorn | j.hogendoorn@bdmcc.net|
|Jeroen Lamberts | j.lamberts@bdmcc.net|
|Jeroen Niesen | Jeroen.Niesen@bdmcc.net|
|Jeroen Wolters | Jeroen.Wolters@bdmcc.net|
|Jeroom van Amstel | jj.van.amstel@bdmcc.net|
|Jesse Mulder | mulder_j@bdmcc.net|
|Job Jansweijer | job.jansweijer@bdmcc.net|
|Johan Burgler | jn.burgler@bdmcc.net|
|Johan Kremer | johankremer@bdmcc.net|
|John Blokhuis | jgm.blokhuis@bdmcc.net|
|John Verburg | nj.verburg@bdmcc.net|
|Jolanda Verhoef | jolanda.verhoef@bdmcc.net|
|Joost IJskes | jm.ijskes@bdmcc.net|
|Joost van Aartsen | jt.van.aartsen@bdmcc.net|
|Jop Cobussen | jf.cobussen@bdmcc.net|
|Jop Gerritsen | jop_gerritsen@bdmcc.net|
|Joris Leker | joris@bdmcc.net|
|Jos Neuteboom Spijker | j.neuteboom.spijker@bdmcc.net|
|Jules Munsterman | j.munsterman@bdmcc.net|
|Justian Lutteke | j.lutteke@bdmcc.net|
|Karansingh Lala | rj.lala@bdmcc.net|
|Klaas Admiraal | k.admiraal@bdmcc.net|
|Klaas Troost | k.troost@bdmcc.net|
|Koen Hendriks | km.hendriks@bdmcc.net|
|Koen Zwikstra | kmz.zwikstra@bdmcc.net|
|Kyra de Vries | k.devries@bdmcc.net|
|Laura van Well | l.van.Well@bdmcc.net|
|Lc.d.reus | Lc.d.reus@bdmcc.net|
|Leejanne Hollaar-Meijboom | l.hollaar-meijboom@bdmcc.net|
|Leendert Versluijs | l.versluijs@bdmcc.net|
|Leon Boon | LBoon@bdmcc.net|
|Leon Mulder | ml.mulder@bdmcc.net|
|Lex van Tol | info@bdmcc.net|
|Lia Bardoel | lia.bardoel@bdmcc.net|
|Linda Jansen | em.jansen@bdmcc.net|
|Linne van Kan | lj.van.kan@bdmcc.net|
|Lise Jonkman | l.jonkman@bdmcc.net|
|Lisenka Impens | l.impens@bdmcc.net|
|Lisette van Gemert | j.vangemert-pijnen@bdmcc.net|
|Maarten Brugman | m.brugman@bdmcc.net|
|Maike Klip | maike.klip@bdmcc.net|
|Maite Donker-Eikelenboom | me.donker-eikelenboom@bdmcc.net|
|Maninder Singh | m.singh@bdmcc.net|
|Marc van der Loo | mj.van.der.loo@bdmcc.net|
|Marcel Ermers | mwc.ermers@bdmcc.net|
|Marcel Heitmeijer | ma.heitmeijer@bdmcc.net|
|Marco Caumon | mch.caumon@bdmcc.net|
|Marco Janssen | marco.janssen@bdmcc.net|
|Marco van Belzen | m.van.belzen@bdmcc.net|
|Marco Zalm | m.zalm@bdmcc.net|
|Margo Pulles | mcc.pulles@bdmcc.net|
|Marielle Verlouw | mh.verlouw@bdmcc.net|
|Mariska Naaktgeboren-Kerssen | m.naaktgeboren_kerssen@bdmcc.net|
|Martijn Hendriks | ma.hendriks@bdmcc.net|
|Martijn Krijgsman | ms.krijgsman@bdmcc.net|
|Martin Janssen | m.janssen@bdmcc.net|
|Martin Krouwer | Martin.Krouwer@bdmcc.net|
|Marvin Lieferink | mj.lieferink@bdmcc.net|
|Matthijs de Vries | m.devries@bdmcc.net|
|Matthijs Goense | matthijs@bdmcc.net|
|Matthijs Veldhuizen | m.veldhuizen@bdmcc.net|
|Maurice de Jong | Maurice.de.Jong@bdmcc.net|
|Maurice Rosmuller | mftm.rosmuller@bdmcc.net|
|Mel van Veen | m_van_veen@bdmcc.net|
|Menno van de Kamp | mne.van.de.kamp@bdmcc.net|
|Michael Ramlal | m.ramlal@bdmcc.net|
|Michel Vaassen | maf.vaassen@bdmcc.net|
|Michel van Seijen | mr.van.seijen@bdmcc.net|
|Michelle Cheung | mn.cheung@bdmcc.net|
|Michelle de Haan-Pitman | m.de.haan-pitman@bdmcc.net|
|Michiel (milvum) | michiel@bdmcc.net|
|Michiel Hegemans | michiel.hegemans@bdmcc.net|
|Michiel Kamminga | m_kamminga@bdmcc.net|
|Michiel Mak | Michiel.Mak@bdmcc.net|
|Mieke van Velzen | am.van.velzen@bdmcc.net|
|Mittchel van Vliet | m-van-vliet@bdmcc.net|
|MT Lambrecht | mt.lambrecht@bdmcc.net|
|Mubaraak Hassan | m.hassan@bdmcc.net|
|Mustafa Yavuz | m.yavuz@bdmcc.net|
|Nick van Luttikhuizen | aw.van.luttikhuizen@bdmcc.net|
|Niels Reinders | neg.reinders@bdmcc.net|
|Nina Wip | nm.wip@bdmcc.net|
|Norbert Laduczky | n.laduczky@bdmcc.net|
|Norman Jamias | norman.jamias@bdmcc.net|
|Olaf van den Berg | oh.van.den.berg@bdmcc.net|
|Patrick Bosz | Patrick.bosz@bdmcc.net|
|Paul Vermaak | p.vermaak@bdmcc.net|
|Paula Lexova | p.lexova@bdmcc.net|
|Pepijn Tournoij | p.tournoij@bdmcc.net|
|Perry de Wit | Perry.de.Wit@bdmcc.net|
|Perry Lambrechts | perry.lambrechts@bdmcc.net|
|Peter Bosch | p.bosch@bdmcc.net|
|Peter Buitenkamp | p.buitenkamp@bdmcc.net|
|Peter Huiskamp | p.huiskamp@bdmcc.net|
|Peter Seignette | p.seignette@bdmcc.net|
|Quincy Soerokarso | q.soerokarso@bdmcc.net|
|R.G.J. Vestjens | r.g.j.vestjens@bdmcc.net|
|Reinier Kops | r.kops@bdmcc.net|
|Remco Pihlajamaa | rm.pihlajamaa@bdmcc.net|
|Remco van Blarcum | r.van.blarcum@bdmcc.net|
|René van Beersum | r.van.beersum@bdmcc.net|
|René Wasseveld | ra.wasseveld@bdmcc.net|
|Richard Rook | r.rook@bdmcc.net|
|Rick Pastoor | me@bdmcc.net|
|Rick van der Klugt | r.vd.klugt@bdmcc.net|
|Rob Mallinckrodt | rhl.mallinckrodt@bdmcc.net|
|Rob Mulder | r.mulder5@bdmcc.net|
|Rob Pijpers | re.pijpers@bdmcc.net|
|Robert Appeldoorn | r.appeldoorn@bdmcc.net|
|Robert Bol | r_bol@bdmcc.net|
|Robin van Dijke | robinvandijke@bdmcc.net|
|Rogier Gerritsen | r.gerritsen@bdmcc.net|
|Ron Roozendaal | r.roozendaal@bdmcc.net|
|Ronald Bellert | ja.bellert@bdmcc.net|
|Ronald Heukers | w.j.r.heukers@bdmcc.net|
|Roos Schouten | a-schouten@bdmcc.net|
|Rosemary Edo Ihaza | ri.edo.ihaza@bdmcc.net|
|Roy Kaizer | r.kaizer@bdmcc.net|
|Rudi Essers | r.essers@bdmcc.net|
|Ryan Barret | Ryan@bdmcc.net|
|S. Djafari | s.djafari@bdmcc.net|
|Sabine Kos | sabinekos@bdmcc.net|
|Salar Silk | salar@bdmcc.net|
|Sander Meier | jgs.meier@bdmcc.net|
|Sander Tuurenhout | sf.tuurenhout@bdmcc.net|
|Security Ordina | security.ordina@bdmcc.net|
|Security PWC | Security.pwc@bdmcc.net|
|Security Reqon | Security.Reqon@bdmcc.net|
|Security Secura | Security.Secura@bdmcc.net|
|Sietse Ringers | sringers@bdmcc.net|
|Sjors Gerritsen | s-gerritsen@bdmcc.net|
|Stefan Hannema | s.hannema@bdmcc.net|
|Stefan Willemsen | s.willemsen@bdmcc.net|
|Stephan Marciniak | support@bdmcc.net|
|Steve Kellaway | steve.kellaway@bdmcc.net|
|Suzan Masson | sb.masson@bdmcc.net|
|Sylvia Bronmans | sylvia.bronmans@bdmcc.net|
|System Appcenter | System.Appcenter@bdmcc.net|
|System Backup | system.backup@bdmcc.net|
|System LDAP | system.ldap@bdmcc.net|
|System Nextcloud | system.nextcloud@bdmcc.net|
|System Nuget | system.nuget@bdmcc.net|
|system.devices@bdmcc.net | system.devices@bdmcc.net|
|Tanja van Dijk | tm.v.dijk@bdmcc.net|
|Tanya Klok - Kastsiuk | tr.klok-kastsiuk@bdmcc.net|
|Theo Meinster | tj.meinster@bdmcc.net|
|Thijs Fieret | ta.fieret@bdmcc.net|
|Thijs Kroesbergen | ta.kroesbergen@bdmcc.net|
|Thijs Weitkamp | twweitkamp@bdmcc.net|
|Tim de Groot | tim.de.groot@bdmcc.net|
|Tim Wijgers | tim.wijgers@bdmcc.net|
|Tino Schubert | ra.schubert@bdmcc.net|
|Tjibbe Bouma | t.bouma@bdmcc.net|
|Tobias Dekker | Tobias_Dekker@bdmcc.net|
|Tobias van der Voorn | t.vd.voorn@bdmcc.net|
|Toine Veenhuis | jla.veenhuis@bdmcc.net|
|Tom den Boer | ta.den.boer@bdmcc.net|
|Tom Westerhout | t.westerhout@bdmcc.net|
|Tomas Harreveld | t.harreveld@bdmcc.net|
|Tomas van der Kolk | ta.van.der.kolk@bdmcc.net|
|Tycho Carbaat | tycho.carbaat@bdmcc.net|
|Vidjay Prahladsingh | v.prahladsingh@bdmcc.net|
|Wilfred Willemink | jwf.willemink@bdmcc.net|
|Willem van Deel | w.van.deel@bdmcc.net|
|Wilrico Feenstra | hjw.feenstra@bdmcc.net|
|Wim Bron | wm.bron@bdmcc.net|
|WonJung Kalsbeek | WonJung.Kalsbeek@bdmcc.net|
|Wouter Hennekam | wouter.hennekam@bdmcc.net|
|Yassin Azdad | y.azdad@bdmcc.net|
|Yigit Baylan | my.baylan@bdmcc.net|
|Yola Park | je.park@bdmcc.net|
|Zsa Zsa Zonnenberg | zzm.zonnenberg@bdmcc.net|
|zTest Nextcloud (tbv 2FA testen Nextcloud) | ztest.nextcloud@bdmcc.net|

````
az ad user create --display-name "Alex Smits"  --password Mypaermy2aa3434$$  --user-principal-name  "alex.smits@ugchelen.onmicrosoft.com"
az ad user create --display-name "Alexandra Brouwershaven"  --password Mypaermy2aa3434$$  --user-principal-name  "as.van.brouwershaven@ugchelen.onmicrosoft.com"
az ad user create --display-name "Alfred Pruim"  --password Mypaermy2aa3434$$  --user-principal-name  "a.pruim@ugchelen.onmicrosoft.com"
az ad user create --display-name "Almar Diehl"  --password Mypaermy2aa3434$$ --user-principal-name a.diehl@ugchelen.onmicrosoft.com"
az ad user create --display-name "Andre Vlaardingerbroek"  --password Mypaermy2aa3434$$  --user-principal-name  "a.vlaardingerbroek@ugchelen.onmicrosoft.com"
az ad user create --display-name "Andy van den Biggelaar"  --password Mypaermy2aa3434$$  --user-principal-name  "andy.van.den.biggelaar@ugchelen.onmicrosoft.com"
az ad user create --display-name "Anja Boonstra de Boer"  --password Mypaermy2aa3434$$  --user-principal-name  "a.boonstra-de.boer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Arian Geertsema"  --password Mypaermy2aa3434$$  --user-principal-name  "a.geertsema@ugchelen.onmicrosoft.com"
az ad user create --display-name "Arthur Rijke"  --password Mypaermy2aa3434$$  --user-principal-name  "arthur.rijke@ugchelen.onmicrosoft.com"
az ad user create --display-name "Asare Twum"  --password Mypaermy2aa3434$$  --user-principal-name  "a.twum@ugchelen.onmicrosoft.com"
az ad user create --display-name "Barend Tempelman"  --password Mypaermy2aa3434$$  --user-principal-name  "b.tempelman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Bart Heijenk"  --password Mypaermy2aa3434$$  --user-principal-name  "bd.heijenk@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ben Beijer"  --password Mypaermy2aa3434$$  --user-principal-name  "b.beijer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Bert Harmsen"  --password Mypaermy2aa3434$$  --user-principal-name  "b.harmsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Bianca Averink"  --password Mypaermy2aa3434$$  --user-principal-name  "b.averink@ugchelen.onmicrosoft.com"
az ad user create --display-name "Bianca Tijssen-van Gelder"  --password Mypaermy2aa3434$$  --user-principal-name  "b.tijssen-van.gelder@ugchelen.onmicrosoft.com"
az ad user create --display-name "Bram Duvigneau"  --password Mypaermy2aa3434$$  --user-principal-name  "bram@ugchelen.onmicrosoft.com"
az ad user create --display-name "Brenno de Winter"  --password Mypaermy2aa3434$$  --user-principal-name  "brenno@ugchelen.onmicrosoft.com"
az ad user create --display-name "Cameron MC Gorian"  --password Mypaermy2aa3434$$  --user-principal-name  "cameron@ugchelen.onmicrosoft.com"
az ad user create --display-name "Caner Bektas"  --password Mypaermy2aa3434$$  --user-principal-name  "c.bektas@ugchelen.onmicrosoft.com"
az ad user create --display-name "Cara Koesoemo"  --password Mypaermy2aa3434$$  --user-principal-name  "cara.koesoemo@ugchelen.onmicrosoft.com"
az ad user create --display-name "Casper Meijerink"  --password Mypaermy2aa3434$$  --user-principal-name  "casper.meijerink@ugchelen.onmicrosoft.com"
az ad user create --display-name "Chi Hon Choi"  --password Mypaermy2aa3434$$  --user-principal-name  "ch.choi@ugchelen.onmicrosoft.com"
az ad user create --display-name "Chris Baas"  --password Mypaermy2aa3434$$  --user-principal-name  "c.baas@ugchelen.onmicrosoft.com"
az ad user create --display-name "Chris Timmermans"  --password Mypaermy2aa3434$$  --user-principal-name  "cma.timmermans@ugchelen.onmicrosoft.com"
az ad user create --display-name "Christiaan Veeningen"  --password Mypaermy2aa3434$$  --user-principal-name  "c.veeningen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Cindy Babis"  --password Mypaermy2aa3434$$  --user-principal-name  "cindy.babis@ugchelen.onmicrosoft.com"
az ad user create --display-name "Clarinda Moonen"  --password Mypaermy2aa3434$$  --user-principal-name  "cm.moonen@ugchelen.onmicrosoft.com"
az ad user create --display-name "cm de Jongh"  --password Mypaermy2aa3434$$  --user-principal-name  "cm.d.jongh@ugchelen.onmicrosoft.com"
az ad user create --display-name "Danai van Lith"  --password Mypaermy2aa3434$$  --user-principal-name  "Danai.van.Lith@ugchelen.onmicrosoft.com"
az ad user create --display-name "Danny Pluim"  --password Mypaermy2aa3434$$  --user-principal-name  "d_pluim@ugchelen.onmicrosoft.com"
az ad user create --display-name "Danny van Luijpen"  --password Mypaermy2aa3434$$  --user-principal-name  "d.van.luijpen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Debby Huijsmans"  --password Mypaermy2aa3434$$  --user-principal-name  "d.huijsmans@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dennis Boehmer"  --password Mypaermy2aa3434$$  --user-principal-name  "d.boehmer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dennis Kramer"  --password Mypaermy2aa3434$$  --user-principal-name  "dennis@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dennis Matthijsen"  --password Mypaermy2aa3434$$  --user-principal-name  "d.matthijsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dennis Roozemond"  --password Mypaermy2aa3434$$  --user-principal-name  "da.roozemond@ugchelen.onmicrosoft.com"
az ad user create --display-name "Diane de Joode"  --password Mypaermy2aa3434$$  --user-principal-name  "diane-de.joode@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dick Blaauw"  --password Mypaermy2aa3434$$  --user-principal-name  "h.r.blaauw@ugchelen.onmicrosoft.com"
az ad user create --display-name "Diego Marcon"  --password Mypaermy2aa3434$$  --user-principal-name  "dm.marcon@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dion Oude Spraakste"  --password Mypaermy2aa3434$$  --user-principal-name  "dtj.oude.spraakste@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dirk-Willem van Gulik"  --password Mypaermy2aa3434$$  --user-principal-name  "dirkx@ugchelen.onmicrosoft.com"
az ad user create --display-name "Dominick Nijboer"  --password Mypaermy2aa3434$$  --user-principal-name  "d.nijboer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Don van Meel"  --password Mypaermy2aa3434$$  --user-principal-name  "don.van.meel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Douwe van der Galien"  --password Mypaermy2aa3434$$  --user-principal-name  "douwe.van.der.galien@ugchelen.onmicrosoft.com"
az ad user create --display-name "Edo Plantinga"  --password Mypaermy2aa3434$$  --user-principal-name  "edo@ugchelen.onmicrosoft.com"
az ad user create --display-name "Edwin Croes"  --password Mypaermy2aa3434$$  --user-principal-name  "ec.croes@ugchelen.onmicrosoft.com"
az ad user create --display-name "Eghbol Sarwar"  --password Mypaermy2aa3434$$  --user-principal-name  "e.sarwar@ugchelen.onmicrosoft.com"
az ad user create --display-name "Emiel Janson"  --password Mypaermy2aa3434$$  --user-principal-name  "hello@ugchelen.onmicrosoft.com"
az ad user create --display-name "Eric Reijnders"  --password Mypaermy2aa3434$$  --user-principal-name  "eha.reijnders@ugchelen.onmicrosoft.com"
az ad user create --display-name "Eric Verheul"  --password Mypaermy2aa3434$$  --user-principal-name  "eric.verheul@ugchelen.onmicrosoft.com"
az ad user create --display-name "Eric Visser"  --password Mypaermy2aa3434$$  --user-principal-name  "ep_visser@ugchelen.onmicrosoft.com"
az ad user create --display-name "Erica van Kempen"  --password Mypaermy2aa3434$$  --user-principal-name  "ej.van.kempen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Erik Goverde"  --password Mypaermy2aa3434$$  --user-principal-name  "e.goverde@ugchelen.onmicrosoft.com"
az ad user create --display-name "Erik Henricks"  --password Mypaermy2aa3434$$  --user-principal-name  "eha.henricks@ugchelen.onmicrosoft.com"
az ad user create --display-name "Erik Holkers"  --password Mypaermy2aa3434$$  --user-principal-name  "e.h.holkers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Erik te Boome"  --password Mypaermy2aa3434$$  --user-principal-name  "hjm.te.boome@ugchelen.onmicrosoft.com"
az ad user create --display-name "Evelien Wolters"  --password Mypaermy2aa3434$$  --user-principal-name  "e_wolters@ugchelen.onmicrosoft.com"
az ad user create --display-name "Evert Jan Elings"  --password Mypaermy2aa3434$$  --user-principal-name  "ej.elings@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ewoud Koster"  --password Mypaermy2aa3434$$  --user-principal-name  "e.koster@ugchelen.onmicrosoft.com"
az ad user create --display-name "ezrah.ligthart.schenk"  --password Mypaermy2aa3434$$  --user-principal-name  "ezrah.ligthart.schenk@ugchelen.onmicrosoft.com"
az ad user create --display-name "F. Sevinc"  --password Mypaermy2aa3434$$  --user-principal-name  "f.sevinc@ugchelen.onmicrosoft.com"
az ad user create --display-name "F.L. Aries"  --password Mypaermy2aa3434$$  --user-principal-name  "fl.aries@ugchelen.onmicrosoft.com"
az ad user create --display-name "Fatma Kilinc"  --password Mypaermy2aa3434$$  --user-principal-name  "fz.kilinc@ugchelen.onmicrosoft.com"
az ad user create --display-name "Frans Lexis"  --password Mypaermy2aa3434$$  --user-principal-name  "fhm.lexis@ugchelen.onmicrosoft.com"
az ad user create --display-name "Fred Both"  --password Mypaermy2aa3434$$  --user-principal-name  "f.both@ugchelen.onmicrosoft.com"
az ad user create --display-name "Fred Bruins"  --password Mypaermy2aa3434$$  --user-principal-name  "fej.bruins@ugchelen.onmicrosoft.com"
az ad user create --display-name "Freek Riegman"  --password Mypaermy2aa3434$$  --user-principal-name  "fa.riegman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Funs Janssen"  --password Mypaermy2aa3434$$  --user-principal-name  "f.janssen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Gemma Mooij"  --password Mypaermy2aa3434$$  --user-principal-name  "Gemma.mooij@ugchelen.onmicrosoft.com"
az ad user create --display-name "Gerbrant van den Hengel"  --password Mypaermy2aa3434$$  --user-principal-name  "g.vandenhengel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Gerwin Veenhuizen"  --password Mypaermy2aa3434$$  --user-principal-name  "gwg.veenhuizen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Gianni Castaldi"  --password Mypaermy2aa3434$$  --user-principal-name  "Gianni.castaldi@ugchelen.onmicrosoft.com"
az ad user create --display-name "H.J. van Haastert"  --password Mypaermy2aa3434$$  --user-principal-name  "hj.v.haastert@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hamid Ouaali"  --password Mypaermy2aa3434$$  --user-principal-name  "h.ouaali@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hans-Peter Los"  --password Mypaermy2aa3434$$  --user-principal-name  "jh.los@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hans Schaap"  --password Mypaermy2aa3434$$  --user-principal-name  "h.schaap@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hans Versteeg"  --password Mypaermy2aa3434$$  --user-principal-name  "Hans.Versteeg@ugchelen.onmicrosoft.com"
az ad user create --display-name "HansRob Reus"  --password Mypaermy2aa3434$$  --user-principal-name  "HansRob.Reus@ugchelen.onmicrosoft.com"
az ad user create --display-name "Harald Lammers"  --password Mypaermy2aa3434$$  --user-principal-name  "h.lammers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hendrik Jan Schuurkamp"  --password Mypaermy2aa3434$$  --user-principal-name  "hj.schuurkamp@ugchelen.onmicrosoft.com"
az ad user create --display-name "Henri Hoekerd"  --password Mypaermy2aa3434$$  --user-principal-name  "hj.hoekerd@ugchelen.onmicrosoft.com"
az ad user create --display-name "Henri ter Hofte"  --password Mypaermy2aa3434$$  --user-principal-name  "h.ter.hofte@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hidde Schultze"  --password Mypaermy2aa3434$$  --user-principal-name  "hidde.schultze@ugchelen.onmicrosoft.com"
az ad user create --display-name "Hugo Visser"  --password Mypaermy2aa3434$$  --user-principal-name  "hugo@ugchelen.onmicrosoft.com"
az ad user create --display-name "Huib Schopman"  --password Mypaermy2aa3434$$  --user-principal-name  "hha.schopman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ilias El Gris"  --password Mypaermy2aa3434$$  --user-principal-name  "i.el.gris@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ingrid van Buuren"  --password Mypaermy2aa3434$$  --user-principal-name  "ib.v.buuren@ugchelen.onmicrosoft.com"
az ad user create --display-name "Iris Hekkelman"  --password Mypaermy2aa3434$$  --user-principal-name  "iv.hekkelman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ivo Jansch"  --password Mypaermy2aa3434$$  --user-principal-name  "ivo@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ivo Kepers"  --password Mypaermy2aa3434$$  --user-principal-name  "ihcj.kepers@ugchelen.onmicrosoft.com"
az ad user create --display-name "J. Biesboer"  --password Mypaermy2aa3434$$  --user-principal-name  "j.biesboer@ugchelen.onmicrosoft.com"
az ad user create --display-name "J.C. Hoorenman"  --password Mypaermy2aa3434$$  --user-principal-name  "jc.hoorenman@ugchelen.onmicrosoft.com"
az ad user create --display-name "J.E. Slot"  --password Mypaermy2aa3434$$  --user-principal-name  "je.slot@ugchelen.onmicrosoft.com"
az ad user create --display-name "J.M. Schmitz"  --password Mypaermy2aa3434$$  --user-principal-name  "jm.schmitz@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jan Quist"  --password Mypaermy2aa3434$$  --user-principal-name  "jan.quist@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jan Tanis"  --password Mypaermy2aa3434$$  --user-principal-name  "j.tanis@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jarst Faber"  --password Mypaermy2aa3434$$  --user-principal-name  "jarst.faber@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jasper Boerkoel"  --password Mypaermy2aa3434$$  --user-principal-name  "j.boerkoel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jasper Hausen"  --password Mypaermy2aa3434$$  --user-principal-name  "jasper@ugchelen.onmicrosoft.com"
az ad user create --display-name "jasperhupkens@ugchelen.onmicrosoft.com""  --password Mypaermy2aa3434$$  --user-principal-name  "Member
az ad user create --display-name "Jasper Tangermann"  --password Mypaermy2aa3434$$  --user-principal-name  "j.tangermann@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jasper Verbeek"  --password Mypaermy2aa3434$$  --user-principal-name  "jg.verbeek@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jay Richardson"  --password Mypaermy2aa3434$$  --user-principal-name  "jm.richardson@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jay Verkouteren"  --password Mypaermy2aa3434$$  --user-principal-name  "ja.verkouteren@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jelle Prins"  --password Mypaermy2aa3434$$  --user-principal-name  "jelleprins@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jeroen Dijkgraaf"  --password Mypaermy2aa3434$$  --user-principal-name  "j.dijkgraaf@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jeroen Hogendoorn"  --password Mypaermy2aa3434$$  --user-principal-name  "j.hogendoorn@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jeroen Lamberts"  --password Mypaermy2aa3434$$  --user-principal-name  "j.lamberts@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jeroen Niesen"  --password Mypaermy2aa3434$$  --user-principal-name  "Jeroen.Niesen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jeroen Wolters"  --password Mypaermy2aa3434$$  --user-principal-name  "Jeroen.Wolters@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jeroom van Amstel"  --password Mypaermy2aa3434$$  --user-principal-name  "jj.van.amstel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jesse Mulder"  --password Mypaermy2aa3434$$  --user-principal-name  "mulder_j@ugchelen.onmicrosoft.com"
az ad user create --display-name "Job Jansweijer"  --password Mypaermy2aa3434$$  --user-principal-name  "job.jansweijer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Johan Burgler"  --password Mypaermy2aa3434$$  --user-principal-name  "jn.burgler@ugchelen.onmicrosoft.com"
az ad user create --display-name "Johan Kremer"  --password Mypaermy2aa3434$$  --user-principal-name  "johankremer@ugchelen.onmicrosoft.com"
az ad user create --display-name "John Blokhuis"  --password Mypaermy2aa3434$$  --user-principal-name  "jgm.blokhuis@ugchelen.onmicrosoft.com"
az ad user create --display-name "John Verburg"  --password Mypaermy2aa3434$$  --user-principal-name  "nj.verburg@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jolanda Verhoef"  --password Mypaermy2aa3434$$  --user-principal-name  "jolanda.verhoef@ugchelen.onmicrosoft.com"
az ad user create --display-name "Joost IJskes"  --password Mypaermy2aa3434$$  --user-principal-name  "jm.ijskes@ugchelen.onmicrosoft.com"
az ad user create --display-name "Joost van Aartsen"  --password Mypaermy2aa3434$$  --user-principal-name  "jt.van.aartsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jop Cobussen"  --password Mypaermy2aa3434$$  --user-principal-name  "jf.cobussen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jop Gerritsen"  --password Mypaermy2aa3434$$  --user-principal-name  "jop_gerritsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Joris Leker"  --password Mypaermy2aa3434$$  --user-principal-name  "joris@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jos Neuteboom Spijker"  --password Mypaermy2aa3434$$  --user-principal-name  "j.neuteboom.spijker@ugchelen.onmicrosoft.com"
az ad user create --display-name "Jules Munsterman"  --password Mypaermy2aa3434$$  --user-principal-name  "j.munsterman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Justian Lutteke"  --password Mypaermy2aa3434$$  --user-principal-name  "j.lutteke@ugchelen.onmicrosoft.com"
az ad user create --display-name "Karansingh Lala"  --password Mypaermy2aa3434$$  --user-principal-name  "rj.lala@ugchelen.onmicrosoft.com"
az ad user create --display-name "Klaas Admiraal"  --password Mypaermy2aa3434$$  --user-principal-name  "k.admiraal@ugchelen.onmicrosoft.com"
az ad user create --display-name "Klaas Troost"  --password Mypaermy2aa3434$$  --user-principal-name  "k.troost@ugchelen.onmicrosoft.com"
az ad user create --display-name "Koen Hendriks"  --password Mypaermy2aa3434$$  --user-principal-name  "km.hendriks@ugchelen.onmicrosoft.com"
az ad user create --display-name "Koen Zwikstra"  --password Mypaermy2aa3434$$  --user-principal-name  "kmz.zwikstra@ugchelen.onmicrosoft.com"
az ad user create --display-name "Kyra de Vries"  --password Mypaermy2aa3434$$  --user-principal-name  "k.devries@ugchelen.onmicrosoft.com"
az ad user create --display-name "Laura van Well"  --password Mypaermy2aa3434$$  --user-principal-name  "l.van.Well@ugchelen.onmicrosoft.com"
az ad user create --display-name "Lc.d.reus"  --password Mypaermy2aa3434$$  --user-principal-name  "Lc.d.reus@ugchelen.onmicrosoft.com"
az ad user create --display-name "Leejanne Hollaar-Meijboom"  --password Mypaermy2aa3434$$  --user-principal-name  "l.hollaar-meijboom@ugchelen.onmicrosoft.com"
az ad user create --display-name "Leendert Versluijs"  --password Mypaermy2aa3434$$  --user-principal-name  "l.versluijs@ugchelen.onmicrosoft.com"
az ad user create --display-name "Leon Boon"  --password Mypaermy2aa3434$$  --user-principal-name  "LBoon@ugchelen.onmicrosoft.com"
az ad user create --display-name "Leon Mulder"  --password Mypaermy2aa3434$$  --user-principal-name  "ml.mulder@ugchelen.onmicrosoft.com"
az ad user create --display-name "Lex van Tol"  --password Mypaermy2aa3434$$  --user-principal-name  "info@ugchelen.onmicrosoft.com"
az ad user create --display-name "Lia Bardoel"  --password Mypaermy2aa3434$$  --user-principal-name  "lia.bardoel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Linda Jansen"  --password Mypaermy2aa3434$$  --user-principal-name  "em.jansen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Linne van Kan"  --password Mypaermy2aa3434$$  --user-principal-name  "lj.van.kan@ugchelen.onmicrosoft.com"
az ad user create --display-name "Lise Jonkman"  --password Mypaermy2aa3434$$  --user-principal-name  "l.jonkman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Lisenka Impens"  --password Mypaermy2aa3434$$  --user-principal-name  "l.impens@ugchelen.onmicrosoft.com"
az ad user create --display-name "Lisette van Gemert"  --password Mypaermy2aa3434$$  --user-principal-name  "j.vangemert-pijnen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Maarten Brugman"  --password Mypaermy2aa3434$$  --user-principal-name  "m.brugman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Maike Klip"  --password Mypaermy2aa3434$$  --user-principal-name  "maike.klip@ugchelen.onmicrosoft.com"
az ad user create --display-name "Maite Donker-Eikelenboom"  --password Mypaermy2aa3434$$  --user-principal-name  "me.donker-eikelenboom@ugchelen.onmicrosoft.com"
az ad user create --display-name "Maninder Singh"  --password Mypaermy2aa3434$$  --user-principal-name  "m.singh@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marc van der Loo"  --password Mypaermy2aa3434$$  --user-principal-name  "mj.van.der.loo@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marcel Ermers"  --password Mypaermy2aa3434$$  --user-principal-name  "mwc.ermers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marcel Heitmeijer"  --password Mypaermy2aa3434$$  --user-principal-name  "ma.heitmeijer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marco Caumon"  --password Mypaermy2aa3434$$  --user-principal-name  "mch.caumon@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marco Janssen"  --password Mypaermy2aa3434$$  --user-principal-name  "marco.janssen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marco van Belzen"  --password Mypaermy2aa3434$$  --user-principal-name  "m.van.belzen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marco Zalm"  --password Mypaermy2aa3434$$  --user-principal-name  "m.zalm@ugchelen.onmicrosoft.com"
az ad user create --display-name "Margo Pulles"  --password Mypaermy2aa3434$$  --user-principal-name  "mcc.pulles@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marielle Verlouw"  --password Mypaermy2aa3434$$  --user-principal-name  "mh.verlouw@ugchelen.onmicrosoft.com"
az ad user create --display-name "Mariska Naaktgeboren-Kerssen"  --password Mypaermy2aa3434$$  --user-principal-name  "m.naaktgeboren_kerssen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Martijn Hendriks"  --password Mypaermy2aa3434$$  --user-principal-name  "ma.hendriks@ugchelen.onmicrosoft.com"
az ad user create --display-name "Martijn Krijgsman"  --password Mypaermy2aa3434$$  --user-principal-name  "ms.krijgsman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Martin Janssen"  --password Mypaermy2aa3434$$  --user-principal-name  "m.janssen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Martin Krouwer"  --password Mypaermy2aa3434$$  --user-principal-name  "Martin.Krouwer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Marvin Lieferink"  --password Mypaermy2aa3434$$  --user-principal-name  "mj.lieferink@ugchelen.onmicrosoft.com"
az ad user create --display-name "Matthijs de Vries"  --password Mypaermy2aa3434$$  --user-principal-name  "m.devries@ugchelen.onmicrosoft.com"
az ad user create --display-name "Matthijs Goense"  --password Mypaermy2aa3434$$  --user-principal-name  "matthijs@ugchelen.onmicrosoft.com"
az ad user create --display-name "Matthijs Veldhuizen"  --password Mypaermy2aa3434$$  --user-principal-name  "m.veldhuizen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Maurice de Jong"  --password Mypaermy2aa3434$$  --user-principal-name  "Maurice.de.Jong@ugchelen.onmicrosoft.com"
az ad user create --display-name "Maurice Rosmuller"  --password Mypaermy2aa3434$$  --user-principal-name  "mftm.rosmuller@ugchelen.onmicrosoft.com"
az ad user create --display-name "Mel van Veen"  --password Mypaermy2aa3434$$  --user-principal-name  "m_van_veen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Menno van de Kamp"  --password Mypaermy2aa3434$$  --user-principal-name  "mne.van.de.kamp@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michael Ramlal"  --password Mypaermy2aa3434$$  --user-principal-name  "m.ramlal@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michel Vaassen"  --password Mypaermy2aa3434$$  --user-principal-name  "maf.vaassen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michel van Seijen"  --password Mypaermy2aa3434$$  --user-principal-name  "mr.van.seijen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michelle Cheung"  --password Mypaermy2aa3434$$  --user-principal-name  "mn.cheung@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michelle de Haan-Pitman"  --password Mypaermy2aa3434$$  --user-principal-name  "m.de.haan-pitman@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michiel (milvum)"  --password Mypaermy2aa3434$$  --user-principal-name  "michiel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michiel Hegemans"  --password Mypaermy2aa3434$$  --user-principal-name  "michiel.hegemans@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michiel Kamminga"  --password Mypaermy2aa3434$$  --user-principal-name  "m_kamminga@ugchelen.onmicrosoft.com"
az ad user create --display-name "Michiel Mak"  --password Mypaermy2aa3434$$  --user-principal-name  "Michiel.Mak@ugchelen.onmicrosoft.com"
az ad user create --display-name "Mieke van Velzen"  --password Mypaermy2aa3434$$  --user-principal-name  "am.van.velzen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Mittchel van Vliet"  --password Mypaermy2aa3434$$  --user-principal-name  "m-van-vliet@ugchelen.onmicrosoft.com"
az ad user create --display-name "MT Lambrecht"  --password Mypaermy2aa3434$$  --user-principal-name  "mt.lambrecht@ugchelen.onmicrosoft.com"
az ad user create --display-name "Mubaraak Hassan"  --password Mypaermy2aa3434$$  --user-principal-name  "m.hassan@ugchelen.onmicrosoft.com"
az ad user create --display-name "Mustafa Yavuz"  --password Mypaermy2aa3434$$  --user-principal-name  "m.yavuz@ugchelen.onmicrosoft.com"
az ad user create --display-name "Nick van Luttikhuizen"  --password Mypaermy2aa3434$$  --user-principal-name  "aw.van.luttikhuizen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Niels Reinders"  --password Mypaermy2aa3434$$  --user-principal-name  "neg.reinders@ugchelen.onmicrosoft.com"
az ad user create --display-name "Nina Wip"  --password Mypaermy2aa3434$$  --user-principal-name  "nm.wip@ugchelen.onmicrosoft.com"
az ad user create --display-name "Norbert Laduczky"  --password Mypaermy2aa3434$$  --user-principal-name  "n.laduczky@ugchelen.onmicrosoft.com"
az ad user create --display-name "Norman Jamias"  --password Mypaermy2aa3434$$  --user-principal-name  "norman.jamias@ugchelen.onmicrosoft.com"
az ad user create --display-name "Olaf van den Berg"  --password Mypaermy2aa3434$$  --user-principal-name  "oh.van.den.berg@ugchelen.onmicrosoft.com"
az ad user create --display-name "Patrick Bosz"  --password Mypaermy2aa3434$$  --user-principal-name  "Patrick.bosz@ugchelen.onmicrosoft.com"
az ad user create --display-name "Paul Vermaak"  --password Mypaermy2aa3434$$  --user-principal-name  "p.vermaak@ugchelen.onmicrosoft.com"
az ad user create --display-name "Paula Lexova"  --password Mypaermy2aa3434$$  --user-principal-name  "p.lexova@ugchelen.onmicrosoft.com"
az ad user create --display-name "Pepijn Tournoij"  --password Mypaermy2aa3434$$  --user-principal-name  "p.tournoij@ugchelen.onmicrosoft.com"
az ad user create --display-name "Perry de Wit"  --password Mypaermy2aa3434$$  --user-principal-name  "Perry.de.Wit@ugchelen.onmicrosoft.com"
az ad user create --display-name "Perry Lambrechts"  --password Mypaermy2aa3434$$  --user-principal-name  "perry.lambrechts@ugchelen.onmicrosoft.com"
az ad user create --display-name "Peter Bosch"  --password Mypaermy2aa3434$$  --user-principal-name  "p.bosch@ugchelen.onmicrosoft.com"
az ad user create --display-name "Peter Buitenkamp"  --password Mypaermy2aa3434$$  --user-principal-name  "p.buitenkamp@ugchelen.onmicrosoft.com"
az ad user create --display-name "Peter Huiskamp"  --password Mypaermy2aa3434$$  --user-principal-name  "p.huiskamp@ugchelen.onmicrosoft.com"
az ad user create --display-name "Peter Seignette"  --password Mypaermy2aa3434$$  --user-principal-name  "p.seignette@ugchelen.onmicrosoft.com"
az ad user create --display-name "Quincy Soerokarso"  --password Mypaermy2aa3434$$  --user-principal-name  "q.soerokarso@ugchelen.onmicrosoft.com"
az ad user create --display-name "R.G.J. Vestjens"  --password Mypaermy2aa3434$$  --user-principal-name  "r.g.j.vestjens@ugchelen.onmicrosoft.com"
az ad user create --display-name "Reinier Kops"  --password Mypaermy2aa3434$$  --user-principal-name  "r.kops@ugchelen.onmicrosoft.com"
az ad user create --display-name "Remco Pihlajamaa"  --password Mypaermy2aa3434$$  --user-principal-name  "rm.pihlajamaa@ugchelen.onmicrosoft.com"
az ad user create --display-name "Remco van Blarcum"  --password Mypaermy2aa3434$$  --user-principal-name  "r.van.blarcum@ugchelen.onmicrosoft.com"
az ad user create --display-name "René van Beersum"  --password Mypaermy2aa3434$$  --user-principal-name  "r.van.beersum@ugchelen.onmicrosoft.com"
az ad user create --display-name "René Wasseveld"  --password Mypaermy2aa3434$$  --user-principal-name  "ra.wasseveld@ugchelen.onmicrosoft.com"
az ad user create --display-name "Richard Rook"  --password Mypaermy2aa3434$$  --user-principal-name  "r.rook@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rick Pastoor"  --password Mypaermy2aa3434$$  --user-principal-name  "me@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rick van der Klugt"  --password Mypaermy2aa3434$$  --user-principal-name  "r.vd.klugt@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rob Mallinckrodt"  --password Mypaermy2aa3434$$  --user-principal-name  "rhl.mallinckrodt@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rob Mulder"  --password Mypaermy2aa3434$$  --user-principal-name  "r.mulder5@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rob Pijpers"  --password Mypaermy2aa3434$$  --user-principal-name  "re.pijpers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Robert Appeldoorn"  --password Mypaermy2aa3434$$  --user-principal-name  "r.appeldoorn@ugchelen.onmicrosoft.com"
az ad user create --display-name "Robert Bol"  --password Mypaermy2aa3434$$  --user-principal-name  "r_bol@ugchelen.onmicrosoft.com"
az ad user create --display-name "Robin van Dijke"  --password Mypaermy2aa3434$$  --user-principal-name  "robinvandijke@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rogier Gerritsen"  --password Mypaermy2aa3434$$  --user-principal-name  "r.gerritsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ron Roozendaal"  --password Mypaermy2aa3434$$  --user-principal-name  "r.roozendaal@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ronald Bellert"  --password Mypaermy2aa3434$$  --user-principal-name  "ja.bellert@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ronald Heukers"  --password Mypaermy2aa3434$$  --user-principal-name  "w.j.r.heukers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Roos Schouten"  --password Mypaermy2aa3434$$  --user-principal-name  "a-schouten@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rosemary Edo Ihaza"  --password Mypaermy2aa3434$$  --user-principal-name  "ri.edo.ihaza@ugchelen.onmicrosoft.com"
az ad user create --display-name "Roy Kaizer"  --password Mypaermy2aa3434$$  --user-principal-name  "r.kaizer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Rudi Essers"  --password Mypaermy2aa3434$$  --user-principal-name  "r.essers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Ryan Barret"  --password Mypaermy2aa3434$$  --user-principal-name  "Ryan@ugchelen.onmicrosoft.com"
az ad user create --display-name "S. Djafari"  --password Mypaermy2aa3434$$  --user-principal-name  "s.djafari@ugchelen.onmicrosoft.com"
az ad user create --display-name "Sabine Kos"  --password Mypaermy2aa3434$$  --user-principal-name  "sabinekos@ugchelen.onmicrosoft.com"
az ad user create --display-name "Salar Silk"  --password Mypaermy2aa3434$$  --user-principal-name  "salar@ugchelen.onmicrosoft.com"
az ad user create --display-name "Sander Meier"  --password Mypaermy2aa3434$$  --user-principal-name  "jgs.meier@ugchelen.onmicrosoft.com"
az ad user create --display-name "Sander Tuurenhout"  --password Mypaermy2aa3434$$  --user-principal-name  "sf.tuurenhout@ugchelen.onmicrosoft.com"
az ad user create --display-name "Security Ordina"  --password Mypaermy2aa3434$$  --user-principal-name  "security.ordina@ugchelen.onmicrosoft.com"
az ad user create --display-name "Security PWC"  --password Mypaermy2aa3434$$  --user-principal-name  "Security.pwc@ugchelen.onmicrosoft.com"
az ad user create --display-name "Security Reqon"  --password Mypaermy2aa3434$$  --user-principal-name  "Security.Reqon@ugchelen.onmicrosoft.com"
az ad user create --display-name "Security Secura"  --password Mypaermy2aa3434$$  --user-principal-name  "Security.Secura@ugchelen.onmicrosoft.com"
az ad user create --display-name "Sietse Ringers"  --password Mypaermy2aa3434$$  --user-principal-name  "sringers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Sjors Gerritsen"  --password Mypaermy2aa3434$$  --user-principal-name  "s-gerritsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Stefan Hannema"  --password Mypaermy2aa3434$$  --user-principal-name  "s.hannema@ugchelen.onmicrosoft.com"
az ad user create --display-name "Stefan Willemsen"  --password Mypaermy2aa3434$$  --user-principal-name  "s.willemsen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Stephan Marciniak"  --password Mypaermy2aa3434$$  --user-principal-name  "support@ugchelen.onmicrosoft.com"
az ad user create --display-name "Steve Kellaway"  --password Mypaermy2aa3434$$  --user-principal-name  "steve.kellaway@ugchelen.onmicrosoft.com"
az ad user create --display-name "Suzan Masson"  --password Mypaermy2aa3434$$  --user-principal-name  "sb.masson@ugchelen.onmicrosoft.com"
az ad user create --display-name "Sylvia Bronmans"  --password Mypaermy2aa3434$$  --user-principal-name  "sylvia.bronmans@ugchelen.onmicrosoft.com"
az ad user create --display-name "System Appcenter"  --password Mypaermy2aa3434$$  --user-principal-name  "System.Appcenter@ugchelen.onmicrosoft.com"
az ad user create --display-name "System Backup"  --password Mypaermy2aa3434$$  --user-principal-name  "system.backup@ugchelen.onmicrosoft.com"
az ad user create --display-name "System LDAP"  --password Mypaermy2aa3434$$  --user-principal-name  "system.ldap@ugchelen.onmicrosoft.com"
az ad user create --display-name "System Nextcloud"  --password Mypaermy2aa3434$$  --user-principal-name  "system.nextcloud@ugchelen.onmicrosoft.com"
az ad user create --display-name "System Nuget"  --password Mypaermy2aa3434$$  --user-principal-name  "system.nuget@ugchelen.onmicrosoft.com"
az ad user create --display-name "system.devices@ugchelen.onmicrosoft.com""  --password Mypaermy2aa3434$$  --user-principal-name  "system.devices@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tanja van Dijk"  --password Mypaermy2aa3434$$  --user-principal-name  "tm.v.dijk@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tanya Klok - Kastsiuk"  --password Mypaermy2aa3434$$  --user-principal-name  "tr.klok-kastsiuk@ugchelen.onmicrosoft.com"
az ad user create --display-name "Theo Meinster"  --password Mypaermy2aa3434$$  --user-principal-name  "tj.meinster@ugchelen.onmicrosoft.com"
az ad user create --display-name "Thijs Fieret"  --password Mypaermy2aa3434$$  --user-principal-name  "ta.fieret@ugchelen.onmicrosoft.com"
az ad user create --display-name "Thijs Kroesbergen"  --password Mypaermy2aa3434$$  --user-principal-name  "ta.kroesbergen@ugchelen.onmicrosoft.com"
az ad user create --display-name "Thijs Weitkamp"  --password Mypaermy2aa3434$$  --user-principal-name  "twweitkamp@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tim de Groot"  --password Mypaermy2aa3434$$  --user-principal-name  "tim.de.groot@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tim Wijgers"  --password Mypaermy2aa3434$$  --user-principal-name  "tim.wijgers@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tino Schubert"  --password Mypaermy2aa3434$$  --user-principal-name  "ra.schubert@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tjibbe Bouma"  --password Mypaermy2aa3434$$  --user-principal-name  "t.bouma@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tobias Dekker"  --password Mypaermy2aa3434$$  --user-principal-name  "Tobias_Dekker@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tobias van der Voorn"  --password Mypaermy2aa3434$$  --user-principal-name  "t.vd.voorn@ugchelen.onmicrosoft.com"
az ad user create --display-name "Toine Veenhuis"  --password Mypaermy2aa3434$$  --user-principal-name  "jla.veenhuis@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tom den Boer"  --password Mypaermy2aa3434$$  --user-principal-name  "ta.den.boer@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tom Westerhout"  --password Mypaermy2aa3434$$  --user-principal-name  "t.westerhout@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tomas Harreveld"  --password Mypaermy2aa3434$$  --user-principal-name  "t.harreveld@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tomas van der Kolk"  --password Mypaermy2aa3434$$  --user-principal-name  "ta.van.der.kolk@ugchelen.onmicrosoft.com"
az ad user create --display-name "Tycho Carbaat"  --password Mypaermy2aa3434$$  --user-principal-name  "tycho.carbaat@ugchelen.onmicrosoft.com"
az ad user create --display-name "Vidjay Prahladsingh"  --password Mypaermy2aa3434$$  --user-principal-name  "v.prahladsingh@ugchelen.onmicrosoft.com"
az ad user create --display-name "Wilfred Willemink"  --password Mypaermy2aa3434$$  --user-principal-name  "jwf.willemink@ugchelen.onmicrosoft.com"
az ad user create --display-name "Willem van Deel"  --password Mypaermy2aa3434$$  --user-principal-name  "w.van.deel@ugchelen.onmicrosoft.com"
az ad user create --display-name "Wilrico Feenstra"  --password Mypaermy2aa3434$$  --user-principal-name  "hjw.feenstra@ugchelen.onmicrosoft.com"
az ad user create --display-name "Wim Bron"  --password Mypaermy2aa3434$$  --user-principal-name  "wm.bron@ugchelen.onmicrosoft.com"
az ad user create --display-name "WonJung Kalsbeek"  --password Mypaermy2aa3434$$  --user-principal-name  "WonJung.Kalsbeek@ugchelen.onmicrosoft.com"
az ad user create --display-name "Wouter Hennekam"  --password Mypaermy2aa3434$$  --user-principal-name  "wouter.hennekam@ugchelen.onmicrosoft.com"
az ad user create --display-name "Yassin Azdad"  --password Mypaermy2aa3434$$  --user-principal-name  "y.azdad@ugchelen.onmicrosoft.com"
az ad user create --display-name "Yigit Baylan"  --password Mypaermy2aa3434$$  --user-principal-name  "my.baylan@ugchelen.onmicrosoft.com"
az ad user create --display-name "Yola Park"  --password Mypaermy2aa3434$$  --user-principal-name  "je.park@ugchelen.onmicrosoft.com"
az ad user create --display-name "Zsa Zsa Zonnenberg"  --password Mypaermy2aa3434$$  --user-principal-name  "zzm.zonnenberg@ugchelen.onmicrosoft.com"
az ad user create --display-name "zTest Nextcloud (tbv 2FA testen Nextcloud)"  --password Mypaermy2aa3434$$  --user-principal-name  "ztest.nextcloud@ugchelen.onmicrosoft.com"
````
