---
'0':
  type: string
  name: layout
  label: Layout
  const: ProjectLayout
  hidden: true
'1':
  type: string
  name: metaTitle
  label: Title meta tag (overrides title)
  description: >-
    By default, the <title> tag for this page is determined by the title field
    (in the Content group). You can override the tag value here.
  default: null
  group: seo
'2':
  type: string
  name: metaDescription
  label: Description meta tag
  description: >-
    The description tag is used by search engines and for social sharing. By
    default, the tag is not set.
  default: null
  group: seo
'3':
  type: boolean
  name: addTitleSuffix
  label: Add title suffix
  description: >-
    If enabled, the title suffix defined in the site configuration is appended
    to the title tag of this page.
  default: true
  group: seo
'4':
  type: image
  name: socialImage
  label: Image for social sharing
  description: >-
    Set the image used when sharing this page on social networks (e.g. Facebook,
    Twitter). If not set, the default social image defined in the site
    configuration is used.
  default: null
  group: seo
'5':
  type: list
  name: metaTags
  label: Additional meta tags
  description: >-
    To add or override any meta tag for this page, add entries to this list.
    Entries defined here take precedence over any other defaults.
  group: seo
  items:
    type: model
    models:
      - MetaTag
'6':
  type: string
  name: title
  label: Title
  default: This is a project title
  required: true
'7':
  type: enum
  name: colors
  label: Colors
  description: The color theme of the page
  group: styles
  controlType: palette
  options:
    - label: Colors A
      value: colors-a
      textColor: $onDark
      backgroundColor: $dark
      borderColor: '#ececec'
    - label: Colors B
      value: colors-b
      textColor: $onLight
      backgroundColor: $light
      borderColor: '#ececec'
    - label: Colors C
      value: colors-c
      textColor: $onPrimary
      backgroundColor: $primary
      borderColor: '#ececec'
    - label: Colors D
      value: colors-d
      textColor: $onSecondary
      backgroundColor: $secondary
      borderColor: '#ececec'
    - label: Colors E
      value: colors-e
      textColor: $onComplementary
      backgroundColor: $complementary
      borderColor: '#ececec'
  default: colors-a
'8':
  type: model
  name: backgroundImage
  group: styles
  label: Project background image
  models:
    - BackgroundImage
  default:
    type: BackgroundImage
    url: /images/bg2.jpg
'9':
  type: date
  name: date
  label: Date
  required: true
'10':
  type: string
  name: client
  label: Client
  default: Awesome client
'11':
  type: string
  name: description
  label: Description
  default: >-
    Nunc rutrum felis dui, ut consequat sapien scelerisque vel. Integer
    condimentum dignissim justo vel faucibus.
'12':
  type: model
  name: featuredImage
  label: Featured image
  models:
    - ImageBlock
  default:
    type: ImageBlock
    url: 'https://assets.stackbit.com/components/images/default/post-4.jpeg'
    altText: Project thumbnail image
    caption: ''
'13':
  type: model
  name: media
  label: Media
  models:
    - ImageBlock
    - VideoBlock
  default:
    type: ImageBlock
    url: 'https://assets.stackbit.com/components/images/default/post-4.jpeg'
    altText: Project image
'14':
  type: list
  name: bottomSections
  label: Sections
  items:
    type: model
    models:
      - ContactSection
      - CtaSection
      - DividerSection
      - FeaturedItemsSection
      - FeaturedPostsSection
      - FeaturedProjectsSection
      - HeroSection
      - LabelsSection
      - MediaGallerySection
      - QuoteSection
      - RecentPostsSection
      - RecentProjectsSection
      - TestimonialsSection
      - TextSection
'15':
  type: markdown
  name: markdown_content
  label: Content
  description: Page content
layout: ProjectLayout
metaTitle: null
metaDescription: null
addTitleSuffix: true
socialImage: null
metaTags: []
title: "\U0001F9F0 kSC #33: Sai vedere le informazioni"
colors: colors-a
date: '2023-04-09'
description: Su notion?
featuredImage:
  type: ImageBlock
  altText: Project thumbnail image
  caption: ''
  url: /images/Frame 14.webp
media:
  type: ImageBlock
  url: /images/Frame 14.webp
bottomSections:
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    title: ARRIVANO I BUTTONS!
    text: >+
      <iframe width="100%" height="600"
      src="https://www.youtube.com/embed/6-oHPy3RMao" title="YouTube video
      player" frameborder="0" allow="accelerometer; autoplay; clipboard-write;
      encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen></iframe>

    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-28
          - pb-28
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
  - type: DividerSection
    title: Divider
    elementId: ''
    styles:
      self:
        width: narrow
        padding:
          - pt-0
          - pb-0
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    subtitle: null
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nPer costruire un'audience hai bisogno di catturare l'attenzione delle persone.\n\nE uno dei primi strumenti che hai a disposizione per riuscirci è il titolo di quello che scrivi.\n\n[Ecco alcune lezioni che ti saranno utili a riguardo.](https://twitter.com/VeryGoodCopy/status/1641069776649830400)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nFin dalla sua uscita, Cron Calendar ha ricevuto un sacco di attenzioni positive.\n\nCosì tante che persino Notion l'ha acquisito.\n\n[E sono convinto di una cosa: ora che è accessibile dal web, avrà ancora più successo!](https://cron.com/changelog?ref=creativerly.com)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nNon importa come fai monetization.\n\nScegliere il giusto princing è fondamentale e per questo devi conoscere alcune strategie.\n\n[Queste sono le più utili che ho trovato.](https://thefutur.com/content/3-ways-to-approach-pricing-for-creative-work)\n\n<br>\n"
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-28
          - pb-28
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
  - type: DividerSection
    title: Divider
    elementId: ''
    styles:
      self:
        width: narrow
        padding:
          - pt-0
          - pb-0
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    text: "## **\U0001F680 E QUANDO VORRAI, ECCO COME TI POSSO AIUTARE**\n\n1.  Puoi scaricare\_**Easy Second Brain**\_e rendere il tuo Notion meno caotico.\n    ​[**Lo trovi qui.**](https://danieledamico.gumroad.com/l/easy-second-brain)​\n\n2.  Puoi scaricare\_**Easy Content Strategy**\_ed usare il mio sistema per creare contenuti.\n    ​[Lo trovi qui.](https://bit.ly/ecs-kit-creator)​\n\n3.  Possiamo fare una\_**call sul tuo spazio Notion**.\n    ​[Prenotala qui.](https://danieledamico.gumroad.com/l/easy-notion-workspace)\n\n"
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-28
          - pb-28
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    text: >
      <Script async data-uid="5d6a847b43"
      src="https://kit-sopravvivenza-creator.ck.page/5d6a847b43/index.js" />


      <Script async data-uid="71fb018372"
      src="https://kit-sopravvivenza-creator.ck.page/71fb018372/index.js" />
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-0
          - pb-0
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: center
      subtitle:
        textAlign: center
      text:
        textAlign: center
slug: sai-vedere-le-informazioni-su-notion
---
Ehi ciao 👋,

questo è il numero 33 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò **3 modi per avere i grafici su Notion**.

***

**TL;DR**

*   3 modi per avere i grafici su Notion

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti.

​

Una delle cose che più mi attira di Notion è la possibilità di utilizzarlo per **raccogliere tutte le informazioni** riguardo la tua vita digitale e non solo.

Puoi costruire il tuo Notion e renderlo il punto in cui ritrovare tutte le informazioni di cui hai bisogno.

Sia quelle di tipo **testuale** che quelle di tipo **visivo**.

E, a dire il vero, c’è una cosa che in molti non sanno: su Notion puoi anche “**vedere le informazioni**”.

E non sapere una cosa del genere, significa utilizzare Notion ad un livello inferiore delle sue potenzialità.

Oppure, utilizzare decine di strumenti diversi.

​

# **3 MODI PER AVERE I GRAFICI SU NOTION**

E arriviamo subito al sodo, oggi ti parlerò di 3 modi in cui puoi vedere i grafici su Notion.

*   Li puoi inserire:
*   Li puoi trasportare;
*   Li puoi creare.

Continua a leggere e vedrai (capita la battuta?).
​

## **SU NOTION PUOI INSERIRE I GRAFICI**

Questo è di sicuro il metodo più semplice.

Tutto quello di cui hai bisogno per metterlo in pratica è il **link di un grafico** che vorresti su Notion.

E poi dovrai utilizzare la funzione “**embed**” su Notion.

Mettiamo il caso che hai un grafico su qualche foglio Excel, Google Sheet, oppure preso di qualche pagina web e vuoi utilizzarlo in un **documento sul tuo Notion.**

Tutto quello che devi fare è copiare il link del grafico e spostarti su Notion, nel punto in cui vuoi vedere il grafico.

Incolli il link e poi clicchi sulla voce “embed” nel piccolo menù che si apre.

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/mt4mhGMNsxAvSZZRdfz95h/email)

Una volta che lo avrai fatto, avverrà la magia.

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/6uxu2tLHStMLD3ihqVHfqh/email)

Inoltre, considera che puoi utilizzare la funzione “embed” per inserire anche tanti tipi di contenuti presi dal web.

Per fartela semplice, se hai un link e vuoi che sia su Notion, copia il link e incollalo su Notion: vedrai che succederanno cose.

È importante da sottolineare che questi grafici sono **interattivi** e quindi puoi passare con il mouse sopra le informazioni e poter vedere ulteriori dettagli.

Insomma, una cosa parecchio utile.

​

## **SU NOTION PUOI TRASPORTARE I GRAFICI**

Anche questa opzione è abbastanza semplice da implementare.

Il meccanismo, infatti, è molto simile a quello del punto precedente, solo che devi fare qualcosa in più.

Ci sono diversi strumenti sul web che ti permettono di ottenere il massimo **dall’integrazione tra Notion e Google Sheet**.

In particolare, c’è [questo servizio](https://uno.notion.vip/charts/) che ti permette di prendere i dati dalle tabelle presenti su Google Sheet e creare dei grafici, interattivi e dinamici da poter inserire su Notion.

In pratica, dopo aver inserito i dettagli del foglio Google e dopo aver personalizzato lo stile del grafico, potrai inserirlo dove vuoi su Notion, sempre tramite la funzione “embed”.

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/7Fnv2wCfEU2zKSSmUHjzxJ/email)

​

## **SU NOTION PUOI CREARE I GRAFICI**

Questo è forse il metodo più difficile da mettere in pratica, ma è anche quello che ti darà più soddisfazioni.

O almeno, è quello che vale per me.

In pratica, su Notion puoi utilizzare un particolare linguaggio per poter creare dei **grafici/diagrammi** di flusso che rappresentino visivamente i tuoi database.

Sembra una stregoneria vero?

Devo ammettere una cosa, la faccia che fanno i clienti di [Notion Builders](https://www.notionbuilders.it/) quando vedono la flowchart del sistema che stiamo progettando per loro su Notion (fatta proprio in questo modo) è senza prezzo.

È la faccia che fai quando ti colpisce un’epifania e scommetto che è la stessa faccia che stai facendo anche tu ora.

Ma al netto di questo, come si fanno ste **flowchart**?

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/7g7dfGDBDpDNVNYUNiELKs/email)

In realtà, basta poco per preparare la situazione.

Tutto quello che devi fare è digitare “/” e poi scrivere “code”, tra le opzioni che vedrai comparire nel menù ci sarà anche “code - mermaid”, cliccaci e dovrai solo metterti a scrivere codice.

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/gtXuSF2kAFdM8hUyrSV7FX/email)

Nel nuovo elemento che apparirà, infatti, dovrai cominciare a scrivere in codice mermaid le cose che vuoi vedere.

Così arriverai al risultato desiderato.

​![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/oEqkpAswvGS2m6sgE7pEnd/email)

Ok, riconosco però che una newsletter non è il formato ideale per spiegare in dettaglio come creare una cosa del genere, quindi **continua a leggere** e vedrai.

Ho cercato di mostrarti più in dettaglio possibile come creare grafici su Notion, cosi da poterlo utilizzare al massimo del suo potenziale.

Se i primi due modi sono semplici, il terzo è un po’ più complesso.

Ed è proprio per questo che ho creato un **canale YouTube** apposito: è il canale dove inserirò **tutorial dettagliati** (e non solo) su come costruire cose con Notion e tanti altri tool.

Proprio qualche giorno fa ho pubblicato un video sulla nuova funzione dei buttons, lo puoi trovare al pulsante qui sotto.

Facciamo che se ti iscrivi al canale da questa newsletter, lo interpreterò come segnale di dover registrare un video sul codice mermaid?

Dai su, vediamo che succede!

Detto questo, per oggi è tutto, buona settimana e **beccati le risorse**.

Daniele
