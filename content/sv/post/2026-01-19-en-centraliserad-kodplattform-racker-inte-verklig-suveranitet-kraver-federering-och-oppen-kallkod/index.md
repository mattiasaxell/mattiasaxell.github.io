---
layout: post
title: En centraliserad kodplattform räcker inte – verklig suveränitet kräver federering och öppen källkod
subtitle: Det är den verkliga "no-brainern" för ett säkert Sverige
date: 2026-01-19 07:30:00
author: "Mattias Axell"
header-img: "featured.jpg"
image:
caption: 'Bildkälla: [**Andrew Moca**](https://unsplash.com/photos/text-yAGNjU4rtss)'
draft: true
summary: Att samla all offentlig kodutveckling på en enda central plattform skapar en klassisk "Single Point of Failure". I händelse av kris, krig eller riktade cyberattacker blir en sådan centraliserad instans ett attraktivt och sårbart mål. Om den slås ut stannar den gemensamma utvecklingen av digital infrastruktur upp.
---

Marcus Jerräng kallar i sin [krönika i ComputerSweden](https://computersweden.se/article/4070708/en-statlig-kodplattform-ar-en-no-brainer.html) en statlig kodplattform för en "no-brainer" och hänvisar till den nyligen publicerade rapporten [Kodsamverkansplattform för öppen programvara](/static/uploads/Digg - 2025-07189 - Arbetsgrupp kodsamverkansplattform för öppen programvara Ena - 1.0.0.pdf). Rapporten som är ett resultat från [Ena-samverkan](https://github.com/diggsweden/ena-samverkansplattform-os/tree/main?tab=readme-ov-file) handlar om att offentlig sektor, speciellt staten ska kunna samarbeta väldigt enkelt, praktiskt och säkert på bra och moderna sätt som praktiskt taget är standardiserade arbetssätt inom programvaru- och systemutveckling idag. Även om intentionen att öka samverkan och minska slöseri med skattemedel är helt rätt, förbiser förslaget om en enda central plattform för avgörande aspekter kring Sveriges säkerhet och beredskap.

Rapporten lyfter fram behovet av "digital robusthet" och "digital suveränitet" som centrala motiv. Men för att uppnå detta på riktigt räcker det inte att koden bara är synlig på en gemensam plats. Vi måste titta på hur vi bygger infrastrukturen och på vilka villkor vi äger den. Svaret ligger i kombinationen av federerad arkitektur och de fyra friheterna som kan komma med rätt krav på öppen programvara och öppen källkod.

**Centralisering skapar sårbarhet** 

Att samla all offentlig kodutveckling på en enda central plattform skapar en klassisk "Single Point of Failure". I händelse av kris, krig eller riktade cyberattacker blir en sådan centraliserad instans ett attraktivt och sårbart mål. Om den slås ut stannar den gemensamma utvecklingen av digital infrastruktur upp.

För att bygga ett verkligt motståndskraftigt Sverige bör vi istället titta på, använda och finansiera decentraliserade och federerade lösningar. Det finns idag moderna alternativ inom öppen källkod, exempelvis [Forgejo](https://forgejo.org/) (som även [nämns i rapporten](https://github.com/diggsweden/ena-samverkansplattform-os/tree/main?tab=readme-ov-file)), som möjliggör just detta. Till skillnad från en monolitisk lösning har [Forgejo](https://forgejo.org/) stöd för federering. Det innebär att varje myndighet kan drifta sin egen instans – med full kontroll över egen data och infrastruktur – samtidigt som de samarbetar sömlöst med andra i offentlig, privat eller civil sektor.

Genom federering och integration med svenska identitetsstrukturer som [Sweden Connect](https://swedenconnect.se/) (via Single Sign On), kan en utvecklare på [Skatteverket](https://www.skatteverket.se/) bidra till kod hos [Försäkringskassan](https://www.forsakringskassan.se/) utan att skapa centrala beroenden. Om en myndighets nod attackeras, påverkas inte resten av det offentliga Sveriges utvecklingsförmåga. Det är digital suveränitet i praktiken.

**De fyra friheterna – grunden för oberoende**

Arkitektur är bara halva lösningen. För att en statlig kodplattform ska vara säker på riktigt måste programvaran garantera de fyra grundläggande friheterna för staten och användarna. Utan dessa bygger vi in beroenden till leverantörer som i ett krisläge blir en säkerhetsrisk.

Frihet 0 \- Användning: Staten och skattebetalarna måste ha full rådighet när skattepengar använts. Inga användaravtal eller utländska jurisdiktioner får begränsa hur svenska myndigheter använder sin programvara. Detta skyddar oss mot sanktioner eller "kill switches" från främmande makt.

Frihet 1 \- Granskning: För nationell säkerhet krävs "Security by Transparency". Svenska säkerhetsmyndigheter måste kunna granska källkoden för att säkerställa att det inte finns bakdörrar eller spionprogram. Vi kan inte förlita oss på "svarta lådor" i kritisk infrastruktur.

Frihet 2 \- Distribution: Om en myndighet har en lösning måste den kunna delas fritt till Sveriges 290 kommuner och 21 regioner utan att licenskostnader skenar. I en krissituation måste digitala verktyg kunna rullas ut omedelbart utan juridiska hinder.

Frihet 3 \- Förbättring: Detta eliminerar "Vendor Lock-in". Om en leverantör försvinner eller agerar fientligt så måste staten kunna ta över koden och fortsätta driften. Det säkerställer att skattemedel bygger värde i det gemensamma, inte i stängda produkter vi inte äger eller har total kontroll över.

Låt oss inte bygga fast oss i en centraliserad sårbarhet. En statlig kodsamverkan är nödvändig, men den måste vila på federerade principer där varje myndighet bidrar till ett robust nätverk, byggt på programvara som garanterar de fyra friheterna.

Att välja en lösning som [Forgejo](https://forgejo.org/) är därför inte bara en teknisk preferens – det är en säkerhetspolitisk nödvändighet. Utan de fyra friheterna så hyr vi bara vår suveränitet i andras infrastruktur. Med de fyra friheterna äger vi suveräniteten och har den på riktigt. 

Det är den verkliga "no-brainern" för ett säkert Sverige.

## Länkar:
- [Krönika i ComputerSweden](https://computersweden.se/article/4070708/en-statlig-kodplattform-ar-en-no-brainer.html)
- Begäran om allmän handling på [Handlingar.se](https://handlingar.se/) gällande plattformen finns [här](https://handlingar.se/request/rapport_om_kodsamverkansplattfor#incoming-5629)
- Bild: [https://unsplash.com/photos/text-yAGNjU4rtss](https://unsplash.com/photos/text-yAGNjU4rtss)
- Rapporten "Kodsamverkansplattform för öppen programvara – 1.0.0" finns att ta del av [här](/static/uploads/Digg - 2025-07189 - Arbetsgrupp kodsamverkansplattform för öppen programvara Ena - 1.0.0.pdf)