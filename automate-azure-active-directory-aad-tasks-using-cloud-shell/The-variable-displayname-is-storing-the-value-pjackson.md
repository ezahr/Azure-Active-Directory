

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

