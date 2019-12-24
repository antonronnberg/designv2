<!-- Titel på rapporten -->
Laddningstid på kommunala webbplatser
=======================

Introduktion
-----------------------

<!-- Skriv en eller två rader om vad uppgiften handlar om. -->
Med dagens teknik kan det gå snabbt att sluka datamängd. Samtidigt som för
mycket innehåll, implementerat utan tanke, kan orsaka en långsam webbplats
(Wagner 2019).

Det kan därför vara av stort intresse för användare med mobila enheter att
optimeringar på webbplatsers innehåll utförs. Mobildata är en kostnadfråga, då
de flesta idag betalar för en begränsad mängd (Wagner 2019).

Laddningstid hos en webbplats är ett sammanhängande område. Där utvecklingen
orsakat krav hos användare, en viss tid väntan kan vara acceptabel; men helst
ska interaktion kunna ske på direkten.

Så hur står sig dagens kommuner mot datamängd och laddningstid. Denna rapport
utför en granskning av tre kommuners webbplatser: Tyresö, Enköping och Karlstad.


Urval
-----------------------

<!-- Berätta vilka webbplatser du valt att undersöka och varför eller hur du gick tillväga när du gjorde ditt urval. -->
IDG.se (2019) har tagit fram &#45; "fem bästa kommunerna på nätet 2019". De tre
kommunerna som ligger i toppen kommer granskas: Tyresö, Enköping och Karlstad.  

Urvalet av granskningsområde gjordes för att webbplatser där forskaren bor har
en ouppdaterad webbplats. Hos kommuner landet över verkar det enligt
IDG.se (2019), var rätt vanligt. Vissa kommuner har dock tagit tag i sina sidor,
så att få granska de som räknas ligga i framkant kan vara av intresse.

Begränsning har gjorts till att granska tre sidor hos respektive
webbplats, sidorna som grankas är startsidan, samt varsin sida relaterad till
området skola och boende. Fokus ligger på granskning av laddningstid och
användbarhet.

Webbsidornas laddningstid har i denna rapporten fått en gräns för acceptabel
interaktionstid på under fem sekunder. Första sidrenderingen har fått en gräns
på tre sekunder för att upplevas som snabb.


Metod
-----------------------

<!-- Berätta kort om din "metod", hur du gör för att utföra undersökningen. Berätta om du använder något speciellt verktyg. -->
Undersökningen använder sig av följande verktyg för att kunna bedöma webbsidorna.

* För att granska laddningstid används:  
    - Nätverkstabben hos DevTools från Google Chrome webbläsaren &#45; via  
    inkognito-miljön (för att undvika påverkan av webbläsarens tillägg).

* För att få förslag om möjliga optimeringar:  
    - [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) &#45;
    Analyserande sammanställning av tillgängliga optimeringar via Lighthouse.

* Kalkylark med rådata:
    - [Google Sheets](https://docs.google.com/spreadsheets/d/1xIdnkXdeZ2bKuysuW4FxgNGkVb80XlBhDU9VfzedMRI/edit?usp=sharing)
    &#45; Inhämtad rådata för laddningstider och resurser.

Rådata har blivit inhämtad från en laptop med trådlös nätverksanslutning.
Undersökningen granskade de utvalda webbsidorna genom en "desktop" och mobil
(iPhone 5/SE) användning.


Resultat
-----------------------

<!-- Dokumentera dina resultat från din studie. Berätta vad du kom fram till, vilka resultat du hittade och observerade. -->

### Tyresö kommun ###

Ena webbsidan <https://www.tyreso.se/> som används från Tyresö kommun (2019)
illustrerars i bilden.  

![Tyresö](image/tyreso_start_atf.png "Tyresö kommun")

Övriga webbsidor som används i granskningen:  
<https://www.tyreso.se/forskola--skola.html>  
<https://www.tyreso.se/boende--miljo.html>  

| | Loading time (s) | Resources (x) | Page total size (MB) |
|---|:---:|:---:|:---:|
| Startsida | | | |
| - Desktop | 3,11 s | 77x | 4,7 MB |
| - Mobil | 3,04 s | 76x | 5,4 MB |
| Skola | | | |
| - Desktop | 2,95 s | 47x | 3,6 MB |
| - Mobil | 2,29 s | 46x | 3,6 MB |
| Boende | | | |
| - Desktop | 2,21 s | 47x | 3,6 MB |
| - Mobil | 2,22 s | 46x | 3,6 MB |

*Tabell 1: Summerad rådata från mätning av Tyresö:s webbsidor.*

##### Desktop- och Mobil-inläsning #####

Enligt analysdata från PageSpeed Insights (2019), får Tyresö på sin startsida
mätvärden 20 för mobil och 74 för desktop. Webbsidan för skola visar resultatet
20 för mobil och 81 för desktop, samt boende-sidan visar resultat 22 för mobil
och 78 för desktop.

Genomsnitt enligt PageSpeed Insights (2019) på mobilen till första uppritningen
av innehåll är 4,8 sekunder och tid till interaktivt tillstånd är 12,9 sekunder.
Medan desktop-tiden för första uppritningen av innehåll är 1,2 sekunder och tid
till interaktivt tillstånd är 2,9 sekunder.

Gemensam förbättringsmöjlighet för desktop och mobil enligt PageSpeed Insights
(2019) kan göras genom att minska resurser som läses in till första rendering
och rensa oanvänd CSS.

Potentiell förbättring finns också inom cachelagringspolicy, och erbjudande av
en fallback princip när typsnittet hämtas från webben.

* Punkter som Tyresö uppfyller vid olika resolutioner enligt PageSpeed Insights (2019):
    - Använd bilder med rätt storlek
    - Minifiera JavaScript
    - Aktivera textkomprimering
    - Föranslut till obligatoriska källor
    - Undvik upprepade omdirigeringar
    - Läs in viktiga resurser i förväg
    - Använd videoformat för animationer
    - Undviker ett onödigt stort DOM-träd
    - Tredjepartsanvändning


### Enköpings kommun ###

Ena webbsidan <https://enkoping.se/> som används från Enköpings kommun (2019)
illustrerars i bilden.  

![Enköping](image/enkoping_start_atf.png "Enköpings kommun")

Övriga webbsidor som används i granskningen:  
<https://enkoping.se/forskola-och-skola.html>  
<https://enkoping.se/bo-trafik-och-miljo.html>  

| | Loading time (s) | Resources (x) | Page total size (MB) |
|---|:---:|:---:|:---:|
| Startsida | | | |
| - Desktop | 1,43 s | 56x | 2,6 MB |
| - Mobil | 1,59 s | 57x | 2,6 MB |
| Skola | | | |
| - Desktop | 1,77 s | 56x | 2,7 MB |
| - Mobil | 2,28 s | 59x | 2,7 MB |
| Boende | | | |
| - Desktop | 1,87 s | 55x | 3 MB |
| - Mobil | 2,18 s | 58x | 3 MB |

*Tabell 2. Summerad rådata från mätning av Enköpings webbsidor.*

##### Desktop- och Mobil-inläsning #####

Enligt analysdata från PageSpeed Insights (2019), får Enköping på sin startsida
mätvärden 58 för mobil och 93 för desktop. Webbsidan för skola visar resultatet
50 för mobil och 88 för desktop, samt boende-sidan visar resultat 49 för mobil
och 87 för desktop.

Genomsnitt enligt PageSpeed Insights (2019) på mobilen till första uppritningen
av innehåll är 3,5 sekunder och tid till interaktivt tillstånd är 8,1 sekunder.
Medan desktop-tiden för första uppritningen av innehåll är 1,0 sekunder och tid
till interaktivt tillstånd är 1,7 sekunder.

Gemensam förbättringsmöjlighet för desktop och mobil enligt PageSpeed Insights
(2019) kan göras genom att tillämpa nyare bildformat (jpeg 2000/XR eller WebP)
och prioritera resurser för att skapa en tidigare rendering.

Potentiell förbättring finns också inom cachelagringspolicy, och erbjudande av
en fallback princip när typsnittet hämtas från webben. En annan förbättring som
nämns av PageSpeed Insights (2019) är förändring av antalet element i DOM-trädet.

* Punkter som Enköping uppfyller vid olika resolutioner enligt PageSpeed Insights (2019):
    - Minifiera CSS
    - Minifiera JavaScript
    - Föranslut till obligatoriska källor
    - Undvik upprepade omdirigeringar
    - Läs in viktiga resurser i förväg
    - Använd videoformat för animationer
    - Undviker enorm nätverksbelastning
    - Körningstid för JavaScript
    - Tredjepartsanvändning


### Karlstads kommun ###

Ena webbsidan <https://karlstad.se/> som används från Karlstads kommun (2019)
illustrerars i bilden.  

![Karlstad](image/karlstad_start_atf.png "Karlstads kommun")

Övriga webbsidor som används i granskningen:  
<https://karlstad.se/Utbildning-och-barnomsorg/>  
<https://karlstad.se/Bygga-och-bo/>  

| | Loading time (s) | Resources (x) | Page total size (MB) |
|---|:---:|:---:|:---:|
| Startsida | | | |
| - Desktop | 3,23 s | 90x | 6,6 MB |
| - Mobil | 3,48 s | 94x | 6,7 MB |
| Skola | | | |
| - Desktop | 1,26 s | 76x | 2,7 MB|
| - Mobil | 1,32 s | 81x | 2,8 MB |
| Boende | | | |
| - Desktop | 1,86 s | 90x | 4 MB |
| - Mobil | 1,92 s | 94x | 4,1 MB |

*Tabell 3. Summerad rådata från mätning av Karlstads webbsidor.*

##### Desktop- och Mobil-inläsning #####

Enligt analysdata från PageSpeed Insights (2019), får Karlstad på sin startsida
mätvärden 20 för mobil och 62 för desktop. Webbsidan för skola visar resultatet
42 för mobil och 91 för desktop, samt boende-sidan visar resultat 35 för mobil
och 82 för desktop.

Genomsnitt enligt PageSpeed Insights (2019) på mobilen till första uppritningen
av innehåll är 3,6 sekunder och tid till interaktivt tillstånd är 14,7 sekunder.
Medan desktop-tiden för första uppritningen av innehåll är 1,0 sekunder och tid
till interaktivt tillstånd är 2,7 sekunder.

Gemensam förbättringsmöjlighet för desktop och mobil enligt PageSpeed Insights
(2019) kan göras genom rensa oanvänd CSS samt prioritera resurser som krävs för
att skapa en första rendering.

Potentiell förbättring finns också inom cachelagringspolicy, och erbjudande av
en fallback princip när typsnittet hämtas från webben.

* Punkter som Karlstad uppfyller vid olika resolutioner enligt PageSpeed Insights (2019):
    - Minifiera JavaScript
    - Aktivera textkomprimering
    - Föranslut till obligatoriska källor
    - Undvik upprepade omdirigeringar
    - Läs in viktiga resurser i förväg
    - Använd videoformat för animationer
    - Tredjepartsanvändning


Analys
-----------------------

<!-- Diskutera och analysera de resultaten du fann. -->

Tyresö erbjuder en bättre hantering när det kommer till desktop-miljö
rendering. I den form att det inte gjorts någon förändring av inhämtad data för
mobila resolutioner. En möjlig förbättring som skulle gå att få till är att
skjuta upp rendering av JavaScript-/CSS-kod som inte behövs för första rendering.

Enköping förbättringsområden återfinns kring sin hantering av bilder, i form
av att tillämpa nyare bildformat (jpeg 2000/XR eller WebP) men även genom
optimering. I övrigt kan förbättring göras när JavaScript/CSS som inte tillhör
"above the fold" ska läsas in. En anledning att Enköping inte hamnar i liknande
kris kring mobilhantering sker till stor del av att de använder sina bilder rätt
sparsamt.

Det som definivit behöver sig en granskning som Enköping är mängden DOM-element
(2618x) som i nuläget används. Många element leder till en ond spiral, där kod
blir svår att följa/debugga som leder till tidstapp i utveckling av webbplatser
när kommande webbutvecklare ska ta över.

Karlstad är en "bildglad" webbplats och behöver framförallt kolla över sin
bildhantering. Där behöver de prioritera bilder som ska inledningsvis synas.
Bilden längst ner på sidan bör erbjudas en lat inläsning, så de minskar tiden
till interaktivitet. Bilderna som används behöver används av ett bättre format
och optimering kan utföras. I övrigt är det små saker som kan förbättras,
överlag utför de en bra hantering med tanke på den mängden resurser som används.

Gissningsvis går det att förbättra bildernas optimering genom att sänka
kvaliteten en aning utan att det påverkar synbarheten, om inte i desktop-miljön
så i ett mobilt avseende. Denna optimering verkar vara möjlig hos alla kommuner.

När det kom till granskning av gränsvärde hos de olika webbplatserna var det
enbart Enköping som klarade hålla sig under tre sekunder för första
sidrenderingen. Både Tyresö och Karlstad misslyckades uppnå gränsen hos sina
respektive startsidor.

Vad gäller tid innan interaktionstid klarade sig samtliga sidor i desktop-miljö
men under mobilanvändning klarade sig ingen. De kommunalt anställda som behöver
nyttja mobilanvändning för att utföra kommunalt arbete blir därmed hårt drabbade.

Baserat på gränsvärde i relation till laddningstider, kan samtliga
webbplatser optimeras genom att ha en kontinuerlig hantering av minifiering,
kompremering och prioritering av element. Det visar sig att tänket kring
optimering förekommer hos samtliga i någon form. Däremot kan det vara så att en
viss sida har blivit bättre tillämpad än en annan, hos samma webbplats.

Orsaken till detta tyder på att mängden av resurser skiljer sig mellan sidorna.
Det blir alltså viktigt att bestämma en gräns för antal resurser som maximalt
får användas per sida.

Prioritering av "above the fold" kod är något som undgås hos samtliga
webbplatser, samt användning av modernare bildformat. Just utnyttjandet av
bildformat handlar gissningsvis om att hänga med i webbutvecklingen. Så att ha
kännedom av analysverktyg för optimering är en viktig del vid skapande och
underhåll för webbutvecklare.

Samtliga webbplatser uppfyller en högre poäng i mätvärden, när det kommer till
desktop. Den mobila anpassningen verkar hos alla vara sekundär.

* Rangordning av webbplatserna utifrån resultatet:
    1. Enköping - 400p
    2. Karlstad - 332p
    3. Tyresö - 300p

Enköping tar hem segern i och med dess möjlighet till interaktionstid var
vinnande i såväl desktop-miljö som mobilt. Dagens användare finns både mobilt
och på desktop-enheter, viktig punkt att kunna uppfylla lämplig hantering på
samtliga enheter.

Karlstad hamnar som tvåa, men känns som hade de löst en bättre hantering av
bilder, kunde de nått första platsen. Karlstad tillämpar implementerande av en
stor mängd resurser, till skillnad från Enköping. De besegrar Tyresö tack var
en bättre mobilhantering.

Tyresö kan mycket väl ha sänkt sig själva genom att inledningsvis ladda in en
stor mängd med JavaScript. Deras mätvärden mobilt sätt är överlägset sämst av
de deltagande webbplatserna.


Referenser
-----------------------

<!-- Ange de eventuella referenser du använder dig av, om några. -->

Enköpings kommun. (2019). *Välkommen till Enköping*.  
&nbsp;&nbsp;&nbsp;&nbsp;[Elektronisk resurs] accessad 2019-12-18 från  
&nbsp;&nbsp;&nbsp;&nbsp;<https://enkoping.se/>

IDG.se. (2019). Topp100 2019: Här är de 5 bästa kommunerna på nätet.  
&nbsp;&nbsp;&nbsp;&nbsp;[Elektronisk resurs] accessad 2019-12-18 från  
&nbsp;&nbsp;&nbsp;&nbsp;<https://topp100.idg.se/2.39772/1.715015/topp100-2019-kommuner>

Wagner, J. (2019). Why Performance Matters.  
&nbsp;&nbsp;&nbsp;&nbsp;[Elektronisk resurs] accessad 2019-12-18 från  
&nbsp;&nbsp;&nbsp;&nbsp;<https://developers.google.com/web/fundamentals/performance/why-performance-matters/>

Karlstads kommun. (2019). *Karlstads kommuns webbplats*.  
&nbsp;&nbsp;&nbsp;&nbsp;[Elektronisk resurs] accessad 2019-12-18 från  
&nbsp;&nbsp;&nbsp;&nbsp;<https://karlstad.se/>

PageSpeed Insights. (2019). *PageSpeed Insights*.  
&nbsp;&nbsp;&nbsp;&nbsp;[Elektronisk resurs] accessad 2019-12-22 från  
&nbsp;&nbsp;&nbsp;&nbsp;<https://developers.google.com/speed/pagespeed/insights/>

Tyresö kommun. (2019). *Tyresö kommun*.  
&nbsp;&nbsp;&nbsp;&nbsp;[Elektronisk resurs] accessad 2019-12-18 från  
&nbsp;&nbsp;&nbsp;&nbsp;<https://www.tyreso.se/>


Övrigt
-----------------------

<!-- Skriv ditt eget namn samt vilka gruppmedlemmar som deltog i att författa rapporten. -->
Anton Rönnberg
