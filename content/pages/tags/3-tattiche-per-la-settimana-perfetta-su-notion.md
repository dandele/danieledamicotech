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
title: "\U0001F9F0 kSC #44: 3 TATTICHE PER LA SETTIMANA PERFETTA…"
colors: colors-a
date: '2023-06-18'
description: su notion
featuredImage:
  type: ImageBlock
  altText: Project thumbnail image
  caption: ''
  url: /images/Frame 14.webp
media:
  type: ImageBlock
  url: /images/Frame 14.webp
bottomSections:
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nEsiste un modo per unire la\_**potenza dello storytelling con la brevità dei post social**?\n\n​[Si e questa è la guida definitiva su come metterlo in pratica.](https://www.worldbuilders.ai/p/micro-storytelling)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nHai presente quel problema?\n\nQuello dei\_**meeting**.\n\nQuello per cui ogni volta che hai una call, dovresti prendere appunti ma poi o non lo fai, oppure li prendi e poi li perdi?\n\n​[Ecco, questa potrebbe essere la soluzione migliore.](https://fireflies.ai/)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nCome capire se una\_**nicchia**\_può portarti alla monetization oppure no?\n\n​[Leggi questo e replica per la nicchia a cui stai puntando.](https://www.ramoswriter.com/rising-finance-phenomenon/)​\n"
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
slug: 3-tattiche-per-la-settimana-perfetta-su-notion
---
Ehi ciao 👋,

questo è il numero 370 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò di **3 sistemi da usare su Notion per sconvolgerti la vita.**

<br>

***

**TL;DR**

*   3 sistemi da usare su Notion per sconvolgerti la vita

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti.

***

<br>

Notion è uno strumento bello versatile, penso che ormai l'hai capito.

E uno dei modi in cui lo utilizzo di più, al di là dagli aspetti riguardo [Notion Builders](https://www.notionbuilders.it/), è per la mia **produttività personale**.

Sul mio spazio personale, infatti, mi prendo la libertà di testare decine e decine di framework, sistemi e pratiche di produttività.

È una cosa che mi diverte, costruisco quello che mi serve (così miglioro nelle mie capacità di costruzione su Notion) e poi lo metto in pratica (migliorando la mia produttività e non solo).

Per questo, ho pensato di consigliarti **3 sistemi che ho testato in questi ultimi mesi**.

Così, se vuoi, puoi provare a costruirteli sul tuo Notion.

​

## **3 SISTEMI DA USARE SU NOTION PER SCONVOLGERTI LA VITA**

Ma arriviamo subito al sodo, quali sono questi 3 sistemi di cui parlo?

Eccoli:

*   Il sistema 2-4-6;

*   Il metodo Scamper;

*   Il sistema a 43 cartelle;

E ora te ne parlo in dettaglio.

​

### **IL SISTEMA 2-4-6**

Questo è un **framework per dare priorità ai tuoi task**.

Di sicuro ne conosci altri, tipo la matrice di Eisenhower, o quello del 10K Value.

Questo però è quello che sto utilizzando sempre più spesso negli ultimi mesi.

In pratica, consiste nel **categorizzare le cose che devi fare** in:

*   2 task grossi;

*   4 task medi;

*   6 task piccoli.

E quando parlo di "grandezza", mi riferisco tanto alla durata temporale, che l'impatto che hanno quei task sul tuo progetto, che tanti altri fattori che tu stesso puoi decidere.

Insomma, se un task ti fa un po' paura è grosso.

Se ti fa paura così così, è un task medio.

Se invece sai che è una cosa da niente, allora è un task piccolo.

E niente, su Notion puoi metterlo in pratica utilizzando una **semplice proprietà "select" nel tuo task manager** e inserire "Large", "Medium" e "Small" come opzioni.

Poi, **classifichi ogni task** assicurandoti di rispettare i numeri di prima.

E di seguire l'ordine dal task più grande a quello più piccolo.

​

### **IL METODO SCAMPER**

Più che un framework di produttività, questo è un **framework di creatività**.

Lo so, sembra assurdo provare a dare una struttura a qualcosa che di struttura non dovrebbe averne.

Eppure, lo sto utilizzando e fa magie.

In cosa consiste?

Consiste nell'**attribuire ad ogni tua idea, il modo in cui vuoi utilizzarla**, tra 7 opzioni:

*   Sostituire;

*   Combinare;

*   Adattare;

*   Modificare;

*   Utilizzala in altro modo;

*   Eliminare;

*   Invertire.

È molto figo, in pratica con questo strumento aumenti di molto la tua creatività.

E anche questo, lo puoi mettere in pratica su Notion, in meno di 5 minuti.

**Crei un database che ospita tutte le tue idee** (e non solo le tue), poi crei una proprietà (anche in questo caso di tipo "select") e le fornisci le opzioni che ti ho elencato qui sopra.

Ogni volta che aggiungi un'idea al database, le assegni una di queste opzioni.

Questo è il modo più semplice, puoi anche utilizzare le formule per forzare l'assegnazione o renderla casuale.

Il punto però è che, in questo modo, potrai **generare nuove idee facendole scontrare tra loro oppure adattandole, o facendoci altre cose.**

Testalo, è una bomba!

​

### **IL SISTEMA A 43 CARTELLE**

Questo è un framework che puoi seguire per **organizzare il tuo spazio digitale su Notion, e non solo**.

In pratica, **crei 12 cartelle, una per ogni mese dell'anno**.

E all'interno di ognuna di queste cartelle, **crei una cartella per ogni giorno**.

Su Notion, puoi implementarlo con un database e 12 pagine al suo interno, poi al suo interno una pagina per ogni giorno.

Poi valuti tu quanto rendere le pagine collegate tra loro: ci sono tante opzioni.

Ad ogni modo, **il punto è che poi tutte quello che fai finisce all'interno di una specifica giornata**.

E così il tuo spazio resta organizzato, senza che te perdi nulla.

​

Eccoli qui.

3 framework tutti per te, da poter implementare su Notion o dove ti pare.

Come sai, non è importante lo strumento in sé, è importante quale strumento utilizzi di più (e da cui puoi trarre il meglio).

E 3 sistemi del genere, su uno strumento che davvero utilizzi ed è parte della tua giornata, ti **aiuteranno a fare le magie**.

E direi che per oggi è tutto, buona settimana e **beccati le risorse**.

Daniele

