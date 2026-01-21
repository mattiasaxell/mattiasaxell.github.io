---
layout: post
title: Workshop om integritetsbevarande metoder
subtitle: Medskick till Regeringskansliets utredning om Privacy Enhancing Techniques
date: 2026-01-26 07:30:00
author: "Mattias Axell"
header-img: "featured.jpg"
image:
caption: 'Bildkälla: [**AbsolutVision**](https://unsplash.com/photos/classified-page-5-newspaper-selective-focus-photography-bSlHKWxxXak)'
draft: false
summary: Den 16:e januari deltog jag i workshop hos Regeringskansliet om utredningen för integritetsbevarande metoder. Här är mina medskick jag delade med utredningen efter workshopen.
---

Syftet med workshoppen var att få en tydligare bild av förutsättningarna för användningen av teknikerna och utredningen var därför tacksamma för att vi deltagare ville bidra med våra erfarenheter och perspektiv. Resultatet från workshoppen kommer utredarna att använda som underlag i deras fortsatta arbete i utredningen.

***De såg även gärna att vi reflekterade över några frågor kopplat till integritetsfrämjande teknik och datadelning innan workshopen, till exempel:***

## · 1\. Behövs fler tekniska standarder?

Ja, men fokus bör ligga på **interoperabilitet** snarare än bara isolerade säkerhetsprotokoll. För att integritetsfrämjande teknik (PET) ska fungera i stor skala inom offentlig sektor krävs:

**Semantiska standarder (Länkade data):** PET förlorar sitt värde om data inte kan tolkas maskinellt mellan myndigheter. Vi behöver gemensamma ontologier för att beskriva vad för data som skyddas, så att exempelvis en krypterad sökning (Searchable Encryption) vet vad den letar efter.

**Öppna protokoll:** För att undvika inlåsningseffekter (leverantörsinlåsningar, vendor lock-in) måste implementeringar av tekniker som Federated Learning, Multi-Party Computation (MPC) eller annan teknik vila på öppna, välgranskade, tillgängliga standarder, som utvecklas på öppna och inkluderande sätt, om kompetensen finns. **Se mer i Diggs arbete med Interoperabla Specifikationer som finns hos [W3ID.org](http://w3id.org/inspec/specification) och på [GitHub](https://github.com/diggSweden/interoperable-specifications)** 

**Certifiering genom öppenhet:** Standarder bör kräva att de referensarkitekturer som används är baserade på öppen källkod. Transparens är en förutsättning för digital suveränitet och tillit \- till syvene och sist Sveriges nationella suveränitet.

Slutsats: Det behövs **öppna** tekniska standarder, och att vi använder de **öppna** tekniska standarder som finns. Om vi *måste* ta fram fler standarder så bör de vara **öppet** licensierade, publikt tillgängliga på Internet, kostnadsfria att tillgå och använda samt öppet paketerade.

## · 2\. Behövs någon lagändring för att underlätta användningen?

Snarare än helt nya lagar behövs **förtydliganden kring anonymisering och "data minimization"**:

* **Rättslig status för syntetiska data:** Det behövs ett tydligare juridiskt stöd för att syntetiska dataset (genererade via PET) ska betraktas som icke-personuppgifter, vilket skulle radikalt förenkla datadelning för innovation.
* **Harmonisering av "Public Interest":** Lagstiftningen bör uttryckligen premiera användningen av PET när data delas för forskning och statistik, så att myndigheter vågar dela data utan att frukta att de bryter mot proportionalitetsprincipen i GDPR, och att vi förbättrar intresset för öppna data och offentlighetsprincipen, inte använder GDPR som ett svepskäl för att motverka delning.
* **Krav på öppen källkod vid bearbetning:** En lagstadgad princip om att mjukvara som hanterar medborgares integritetskänsliga data ska kunna granskas (öppen källkod) skulle öka säkerheten och acceptansen.

## · 3\. Finns det någon specifik situation (användarfall) där ni anser att offentlig förvaltning borde använda integritetsfrämjande teknik?

Här ser vi störst potential i att kombinera PET med länkade data:

* **Sektorsövergripande hälsoanalys:** Att använda Federated Learning eller *Multi-Party Computation* (MPC) för att samköra data mellan regioner och Socialstyrelsen utan att faktiska patientjournaler någonsin lämnar sina källsystem. Genom länkade data kan vi säkerställa att "blodtryck" betyder samma sak i alla system, medan PET skyddar individen.
* **Bedrägeribekämpning via Federated Learning:** Myndigheter (t.ex. Skatteverket och Försäkringskassan) kan träna maskininlärningsmodeller för att upptäcka mönster i välfärdsbrottslighet utan att dela rådata om medborgarna med varandra.
* **Sömlös "Once-Only"-princip:** Genom att använda *Zero-Knowledge Proofs* (ZKP) kan en medborgare bevisa att de uppfyller ett villkor (t.ex. "är över 18 år" eller "har en inkomst under X kr") för en annan myndighet, utan att faktiska personuppgifter eller exakta siffror behöver delas eller lagras på nytt.

Läsning: Kommittédirektiv \- Integritetsbevarande metoder för en mer datadriven och samverkande förvaltning som finns hos [Regeringen.se](https://www.regeringen.se/contentassets/2dc1fc006b414e87af9853fe23668e0b/integritetsbevarande-metoder-for-en-mer-datadriven-och-samverkande-forvaltning-dir.-202564.pdf) 

# Ytterligare förslag baserat på direktivet

Förslag på ytterligare perspektiv och konkreta frågor att lyfta under workshoppen, baserat på det aktuella kommittédirektivet och din position som förespråkare för **öppen källkod**, **öppna standarder** och **länkade data**.

### **1\. Främja "Digital Suveränitet" genom Öppen Källkod**

Direktivet betonar behovet av att analysera förutsättningar för gemensamma tekniska tjänster och plattformar.

* **Förslag:** Argumentera för att all offentlig PET-infrastruktur bör byggas på öppen källkod. Detta säkerställer att algoritmerna för exempelvis anonymisering, Federated Learning eller *Multi-Party Computation* kan granskas av oberoende parter. 
* **Workshop-fråga:** "Hur kan vi säkerställa att förtroendet för PET-metoder bibehålls över tid om koden bakom dem inte är öppen för granskning?"

### **2\. Semantisk Interoperabilitet med Länkade Data**

För att PET ska fungera effektivt vid datadelning mellan myndigheter krävs att data är begriplig för maskiner.

* **Förslag:** Lyft fram **länkade data** (Linked Data) som den nödvändiga grunden för att PET-verktyg ska kunna tolka och skydda data automatiskt i olika system.
* **Workshop-fråga:** "Behövs standarder som inte bara täcker kryptering (PET), utan även datans betydelse (Länkade data), för att möjliggöra 'Privacy-by-Design' i automatiserade flöden?"

### **3\. Testbäddar och "Sandlådor" för Innovation**

Utredaren ska se över behovet av testmiljöer och plattformar.

* **Förslag:** Föreslå skapandet av nationella "PET-sandlådor" baserade på öppna standarder där myndigheter kan testa tekniker som metadata, *Federated Learning* eller *syntetiska data* utan att riskera riktig personuppgiftsexponering.
* **Workshop-fråga:** "Vilken roll kan en gemensam testbädd spela för att minska den rättsliga osäkerheten myndigheter känner idag?"

### **4\. Från "Anonymisering" till "Zero-Knowledge"**

Direktivet nämner anonymisering och generalisering som exempel.

* **Förslag:** Utmana workshoppen att titta på mer avancerade tekniker som **Zero-Knowledge Proofs (ZKP)**. Det tillåter en myndighet att verifiera ett påstående (t.ex. "personen har rätt till bidrag") utan att faktiskt ta emot eller lagra underliggande känsliga data.
* **Workshop-fråga:** "Istället för att dela data och sedan skydda den, hur kan vi använda PET för att svara på frågor *utan* att dela rådata?"

### **5\. Sammanfattande tabell över dina perspektiv mot Direktivets mål**

| Direktivets mål | Ditt förespråkade perspektiv | Nytta för offentlig sektor |
| :---- | :---- | :---- |
| **Gemensamma tekniska tjänster** | **Öppen källkod** | Undviker inlåsning och ökar transparens. |
| **Effektiv datadelning** | **Länkade data** | Skapar maskinläsbarhet och "Once-Only"-principen. |
| **Rättssäker användning** | **Öppna standarder** | Säkerställer att tekniken följer lagkrav enhetligt. |
