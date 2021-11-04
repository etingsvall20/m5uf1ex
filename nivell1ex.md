# Spring framework
## Salta a la navegacióSalta a la cerca
[L'Spring framework](https://ca.wikipedia.org/wiki/Spring_framework) (abreviant, Spring), és un marc de treball de codi obert per la plataforma Java. La primera versió va ser escrita per Rod Johnson, que inicialment va llençar el producte juntament amb el llibre One-on-One [Java EE](https://ca.wikipedia.org/wiki/Java_EE) Design and Development.[1] També hi ha un port disponible per la plataforma .NET, Spring.NET.

El marc de treball va ser inicialment llençat al juny de 2003 sota la llicència Apache 2.0. La primera versió major 1.0 va ser distribuïda el març de 2004, amb llançaments addicionals el setembre de 2004 i març de 2005. Encara que Spring Framework no força cap model de programació, ha esdevingut amplament popular dintre de la comunitat Java primerament com una alternativa que desplaçaria el model [Enterprise JavaBean](https://ca.wikipedia.org/wiki/Enterprise_JavaBean). Per disseny aquest entorn ofereix una gran llibertat als desenvolupadors de Java i a més proveeix solucions fàcils i ben documentades per pràctiques habituals en la indústria.

Mentre les funcionalitats del nucli de l'entorn són usables en una aplicació Java hi ha diferents extensions i millores per construir aplicacions web damunt d'una plataforma Java EE. Gràcies a això, Spring ha aconseguit una gran popularitat i és reconegut pels fabricants com un entorn estratègicament important.


### Contingut
* Història de Spring Framework
    * Funcionalitats clau
    * Introducció a Spring Framework
    * Mòduls de l'Spring Framework
* Contenidor d'Inversió de Control
    * Entorn de programació orientada a aspectes
    * Entorn d'accés a les dades
    * Entorn de gestió de transaccions
* Entorn model-vista-controlador
    * Entorn d'accés remot
    * Referències
    * Enllaços externs
### Història de Spring Framework
Les primeres parts del que ha esdevingut Spring Framework van ser escrites per Rod Johnson el 2000, mentre treballava com a consultor independent per clients de la indústria financera a Londres. Mentre escrivia el seu llibre Expert One-on-one J2EE Design And Development (Programmer to programmer) (2002), va anar més enllà del seu codi per expressar la seva perspectiva de com les aplicacions amb diferents parts de la plataforma J2EE hauria d'esdevenir més simple i més consistent del que els desenvolupadors i les empreses ho estaven fent en aquell moment.

Tornant a 2001 els models dominants per aplicacions basades en web eren oferts per l'API de Java Servlet i Enterprise JavaBeans. Ambdues eren especificacions creades per **Sun Microsystems** en col·laboració amb altres fabricants i parts interessades i gaudeixen de gran popularitat entre la comunitat Java.

A Rod Johnson se li atribueix la creació d'un marc de treball que estava basada en les acceptades com a millors pràctiques i vàlid per tots els tipus d'aplicacions, no només aplicacions web. Aquestes idees també són estan expressades al seu llibre i posteriorment els lectors de la publicació van demanar millores poder usar el codi encartat amb el llibre sota una llicència de codi obert.

Es va formar un petit equip de desenvolupadors desitjant de treballar a ampliar l'entorn i van crear un lloc web a Sourceforge, el febrer de 2003. Després de treballar en l'entorn durant més d'un any, van llençar la versió 1.0 el març de 2004. Després d'aquest llançament va ser quan va guanyar popularitat, degut en part al Javadoc i la documentació de referència, superiors a la mitjana en un projecte de codi obert.

Tanmateix, Spring Framework va rebre dures crítiques el 2004 i continua sent tema d'agres discussions. Al moment del llançament de la primera versió major, molts desenvolupadors i **líders d'opinió** van veure Spring Framework com una manera de moure la manera de programar respecte del model tradicional, cosa realment certa, pel que __feia__ als Enterprise JavaBeans. Un dels objectius de disseny és el d'integrar-se fàcilment amb estàndards J2EE existents i eines de fabricants ja fetes. En gran manera, això elimina la necessitat de definir les seves funcionalitats en un __document d'especificació__ i controlat per un comitè oficial, cosa que també ha estat criticada.

Aquest marc de treball ha convertit tècniques antigament poc familiars en populars en un curt període, la més notable és la d'Inversió de Control. El 2004 Spring Framework va gaudir de grans índexs d'acceptació amb l'oferiment del seu propi marc de Programació orientada a aspectes (AOP), cosa que va fer esdevenir aquest paradigma més popular arreu de la comunitat Java.

2005 va veure fins i tot millors índexs d'acceptació que l'any anterior, gràcies als nous llançaments que acomplien noves fites importants i aportaven noves funcionalitats. El Fòrum de Spring que va ser llençat al final del 2004 també va ajudar a augmentar la popularitat del marc de treball i ha crescut fins a esdevenir la més important font d'informació i suport pels seus usuaris.

El mateix any els desenvolupadors de Spring van engegar la seva pròpia empresa per oferir suport comercial i es van associar amb BEA Systems. Al desembre de 2005 la primera conferència sobre Spring va ser feta a Miami atraient 300 desenvolupadors durant els tres dies de durada, seguida d'una altra a Anvers el juny del 2006, seguida per 400 persones.

### Funcionalitats clau
Gestió de la configuració basada en JavaBeans, aplicant-hi principis d'Inversió de Control, més específicament usant la tècnica d'Injecció de Dependència. Això ajuda a reduir les dependències de components, en implementacions específiques, sobre altres components.
Una factoria de Beans central, que és usada globalment.
Capa genèrica d'abstracció per la gestió de transaccions de la base de dades.
Estratègies preincorporades per la JTA i un sol DataSource de JDBC. Això elimina la dependència en un entorn Java EE pel suport a les transaccions
Integració amb entorns de persistència com Hibernate, JDO, iBatis i db4o.
Entorn d'aplicació web MVC, construït al nucli de la funcionalitat de Spring. suportant moltes tecnologies per generar vistes, incloent-hi JSP, FreeMaker, Velocity, Tiles, iText i POI.
Entorn extensiu de programació orientada a aspectes per proveir serveis, com ara gestió de les transaccions. Amb això es millora la modularitat dels sistemes.
Introducció a Spring Framework
Aquest entorn proveeix solucions per diversos reptes tècnics encarats per desenvolupadors Java i organitzacions que volen crear aplicacions basades en la Plataforma ![Java](https://i.blogs.es/53044d/java/1366_521.jpg). Donada la clara amplitud de la funcionalitat que s'hi ofereix, pot fer-se complicat distingir entre els blocs principals que componen el marc de treball. Spring Framework no està lligat exclusivament a Java EE, encara que la seva prou aconseguida integració en aquesta àrea és una raó important per la seva popularitat.

>Spring Framework és probablement més conegut per oferir funcionalitats requerides per crear efectivament aplicacions de negoci complexes a part dels models de programació que històricament han estat dominant a la indústria. A més té la fama d'introduir funcionalitats que eren poc familiars en pràctiques de programació que avui en dia són bàsiques, fins i tot més enllà de la Plataforma Java.

>Això revaloritza un entorn que ofereix un model consistent i el fa aplicable a la majoria de tipus d'aplicacions que es creen avui dia sobre la plataforma Java. Hom considera que Spring Framework implementa una manera de treballar basada en les millors pràctiques i estàndards de la indústria, fent-lo vàlid per molt dominis Java.

```javascript
if (isAwesome){
  return true
}
```