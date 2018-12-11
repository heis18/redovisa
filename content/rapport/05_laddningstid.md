---

views:
    byline:
        region: main
        template: anax/v2/block/default
        sort: 2
        data:
            class: byline
            meta:
                type: single
                route: block/byline

---
Laddningstid kmom05
=========================

Jag har i denna uppgift jämfört tre olika hemsidor, där jag undersökt sidornas laddningstid. Denna undersökning görs både i förhållande till mobil enhet och till en dator.


Urval
-----------------------

Jag har valt sidorna <a href="https://www.funasfjallen.se">Funäsfjällen</a>, <a href="http://www.skanesdjurpark.se">Skånesdjurpark</a> och <a href="https://www.liseberg.se/">Liseberg</a>

Jag gjorde mitt urval efter att ha bestämt mig för att välja tre sidor med liknande upplägg och tema, dvs någon form av turistattraktion. Jag startade mitt urval även denna gång till viss del efter minan intressen. Samtliga sidor är ganska bildtunga, vilket jag även tyckte kunde vara intressant att analysera.


Metod
-----------------------
Jag har arbetat med Google Pagespeed och devtools för att mäta laddningstiden på de olika sidorna. Jag har på Google Pagespeed tittat på hastighets poängen, och ett tiden för några olika inladdningsdelar. I devtools har jag tittat på antal förfrågningar på sidan, sidans totala storlek och tiden till slutförd laddning. Jag har även arbetat med gimp för mina screenshots och google sheets för dokumentationen.


Resultat
-----------------------

<a href="https://www.funasfjallen.se">Funäsfjällen</a>

[FIGURE src="image/funasfjall.png?w=700" class="center" alt="Funäsfjällen"]
<br>

Funäsdalens sida fick i mätningen mot mobil en poäng från Google Pagespeed på 22 och en tid till första meningsfulla skärmuppritning på 4.2 sek. Mot en dator var poängen betydligt högre, ca 92 och tiden för en första meningsfulla skärmuppritning låg på 1,2 sek.

Enligt devtools hade sidan ca 94 förfrågningar (varierade något mellan olika inladdningar), storleken på sidan var på drygt 12 mb och tog 6,23 sek att slutföra inladdningen på.
En av de främsta rekommendationerna från Google Pagespeed för att förbättra sidan, både för mobil och dator var att skicka bilderna i modernare bildformat. Även att sidan skulle kunna skjuta upp inladdningen av bilder som inte visades på skärmen. En annan bildrekommendatin var att använda bilder med rätt storlek.

<br>
<a href="http://www.skanesdjurpark.se">Skånesdjurpark</a>

[FIGURE src="image/skanesdjurpark.png?w=700" class="center" alt="Skånes djurpark"]
<br>


Skånes djurparks sida fick i mätningen mot mobil en oerhört låg poäng från Google Pagespeed på 3 och en tid till första meningsfulla skärmuppritning på 8,7 sek. Mot en dator var poängen ca 79 och för en första meningsfulla skärmuppritning låg tiden på 2,3 sek.
Enligt devtools hade sidan ca 95 förfrågningar (även här varierade det något mellan olika inladdningar), storleken på sidan var på ca 6 mb och tog 9,77 sek att slutföra inladdningen på.

Den mest tidsbesparande rekommendationen för Skånes djurparks sida på mobil var enligt Google Pagespeed att ta bort resurser som blockerar rendering. Sedan rekommenderade de att sidan skulle kunna aktivera textkomprimering, skjuta upp css som inte används och liksom Funäsfjällen använda bilder i modernare bildformat. För dator rekommenderar de i första hand att använda bilder  i rätt storlek. Sedan motsvarande rekommendationer som för mobil.

<br>
<a href="https://www.liseberg.se/">Liseberg</a>

[FIGURE src="image/liseberg.png?w=700" class="center" alt="Liseberg"]
<br>


Lisebergs sida fick i mätningen mot mobil en poäng från Google Pagespeed på 36 och en tid till första meningsfulla skärmuppritning på 5,4 sek. Mot en dator var poängen ca 98 och för en första meningsfulla skärmuppritning låg tiden på 1,3 sek.
Enligt devtools hade sidan ca 64 förfrågningar (även här varierade det något mellan olika inladdningar), storleken på sidan var på ca 3 mb och tog 5,38 sek att slutföra inladdningen på.

Där Lisebergs mobilsida skulle kunna spara mest tid enligt Google Pagespeed är att skicka bilderna i ett modernare bildformat och även använda bilder i rätt storlek. De rekommenderar även att sidan skulle kunna skjuta upp inläsning av css som inte används samt att ta bort resurser som blockerar rendering. För datorsidan rekommenderar de i första hand att använda bilder i rätt storlek men även att skicka bilderna i ett modernare bildformat.

<br>

All data i undersökning finns att finna i följande dokument: <a href="https://docs.google.com/spreadsheets/d/1CSpOaE8TVdAP6MTvpjbM6mMOViLS7R3mX2fiSvCy8uc/edit?usp=sharing">Laddningstid Kmom05</a>



Analys
-----------------------
Det märks kan jag tycka på inläsningstiderna att sidorna innehåller mycket bilder och information. Lisebergs sida har nog lyckats begränsa mängden bilder/information på sin första sida mest i jämförelse mot de andra två, då den läser in en fjärdedel så mycket information jämfört med Funäsfjällens sida. Skånes djurparks sida har dubbelt så mycket information jämfört med Liseberg men hälften så mycket som Funäsfjällen. Tiden på de olika sidorna följer dock inte mängden data vilket jag tycker är intressant. Som man nästan kunde gissat på förhand, hade samtliga tre sidorna hade rekommendationer på hur de kunde förbättra inladdningstiden genom att arbeta mer med bilderna. Dessa bestod till stor del av att arbeta med bilder i rätt storlek, vilket jag kan förstå när jag tittar i devtools och kan hitta flertalet bilder upp emot och över 1000kb. En annan förbättring kring bilderna som rekommenderas för alla tre sidorna är att de skulle kunna arbeta med modernare bildformat, men även att sidan inte behöver läsa in information som inte visas på bilden. Den sistnämnda kan jag tänka mig är en orsak till att Funäsfjällens sida läser in så mycket mer information än de andra två. Andra rekommendationer Pagespeed ger är att ta bort resurser som blockerar renderingen av sidan. Överlag känns det som att det finns ganska mycket man skulle kunna göra på sidorna för att få dem att arbeta snabbare.

<br>

Min vinnare skulle jag nog utse Lisebergs sida till. Den har absolut högst betyg av sidorna jag jämfört i Google Pagespeed, både för dator och mobil och den gick märkbart snabbast att ladda in. Den har enligt devtools minst data att läsa in och borde vara den snabbaste vilken den bevisligen även var. Två kommer Funäsfjällens sida och sist kommer Skånes djurpark. Skånes djurparks sida märkte man under inladdningstiden att den tog lång tid, den har hälften så mycket data att läsa in som Funäsfjällens sida, och borde därför inte ta 50% längre tid att läsa in.

<br>

Jag skulle bedöma laddningstiden av Skånes djurparks sida som alldeles för långsam, även på en dator så hinner man börja tröttna innan sidan är helt färdig. Ett resultat på 3 på mobil känns katastrofalt lågt. Lisebergs sida känns ok när man laddar in den på mobilen medans Funäsfjällens sidan upplevs något långsam, så jag kan tänka mig att en poäng på åtminstone 30 på mobil borde vara att rekommendera. På datorn känns både Lisebergs och Funäsfjällens sidor helt ok i inladdningstid, så jag kan tänka mig att en sida med ett betyg på i alla fall 85-90 poäng borde vara att föredra. Ett resultat på 79 poäng som Skånes djurpark fick, duger inte.

Referenser
-----------------------

Beaird, Jason, The Principles of Beautiful Web Design, 2014

<a href="https://developers.google.com/speed/pagespeed/insights/">Google Pagespeed</a>

Devtools


Övrigt
-----------------------

Helena Isåfjäll
