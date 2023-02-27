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
title: "\U0001F9F0 kSC #26: Ma tu che te ne intendi di Notion..."
colors: colors-a
date: '2023-02-12'
client: Awesome client
description: DIMMI DELLE COSE
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nI\_**meme**\_sono uno strumento fantastico per creare un’audience.\n\nSolo che è un casino crearli, vero?\n\n​[Se hai risposto di sì, da oggi dovrai cambiare idea.](https://imgflip.com/memegenerator)\n\n\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nUn tempo, qualcuno mi ha detto che non puoi migliorare quello che non riesci a misurare.\n\n​[Per questo, quando ho scoperto questo tool me ne sono innamorato.](https://rize.io/)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nUtilizzi\_**Gmail**?\n\nÈ molto probabile che la risposta sia si.\n\n​[Ed è per questo che questo tool ti piacerà: possibilità di monetizzare, direttamente dal tuo account Gmail.](https://www.gmass.co/)​\n"
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
slug: notion-ai-cosa-fare
---
Tutti che parlano di AI.

È da qualche mese ormai che non c'è giorno in cui non ti capiti davanti qualche contenuto a tema AI.

Prima c'era ChatGPT.

E ora che Notion AI è aperto a tutti, la situazione peggiorerà.

Ma a parte essere figo, **Notion AI a cosa serve?**

***

**TL;DR**

*   Notion AI: che ci puoi fare?

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 40.

***

Ehi ciao 👋,

questo è il numero 27 del **Kit di Sopravvivenza per Creator**.

Ed oggi risponderò **3 modi per utilizzare Notion AI. una cosa che capita.**



Diciamoci la verità, Notion AI è stato annunciato (e poi rilasciato) in un momento particolare.

Poco dopo il rilascio di **ChatGPT**, quando il mondo ancora osservava incredulo quello che il tool di Open AI era in grado di fare.

Chi aveva tempo di pensare alla versione di AI fatta da Notion?

Solo gli ossessionati come me.

Così, mentre tutti giocavano con ChatGPT, io ho giocato sia con ChatGPT che con Notion AI.

E delle differenze ne ho parlato già qualche newsletter fa.

Oggi ti racconterò altro: ti racconterò di **tre modi in cui utilizzo Notion AI** quasi tutti i giorni.

​

## **NOTION AI: CHE CI PUOI FARE?**

Arriviamo subito al sodo, già le mie newsletter sono lunghe, meglio non esagerare.

Utilizzo Notion AI in questi modi qua:

*   Zettelkasten velocizzato;

*   Il copy efficiente;

*   Call indimenticabili.

Ora te li racconto in dettaglio.

​

### **ZETTELKASTEN VELOCIZZATO**

Conosci il [metodo Zettelkasten](https://zettelkasten.de/introduction/)?

È uno strumento che ti permette di raccogliere informazioni (prendere note), di processarle e crearne una rete.

Una rete che poi facilita la tua **creatività** e **produttività**.

Insomma, è una cosa che puoi fare con Notion, Obsidian e altri tool del genere.

Con **Notion AI** però le puoi dare una marcia in più.

Si, perché finora i miei appunti dei libri letti finivano in un database su Notion (tramite Readwise) e lì restavano, senza la giusta fase di analisi e summarization.

Con Notion AI, invece, il problema è risolto.

In pratica, per ogni libro, articolo, podcast o documento presente nella mia libreria Readwise, ci sono tutta una serie di note e appunti.

Quando finisco di leggere il libro, mi basta andare all’interno della pagina su Notion e chiedere a Notion AI di fare un summary degli appunti presi.

Qualche clic invece di qualche ora.

​

### **COPY EFFICIENTE**

Questo è l’utilizzo più ovvio, lo so.

Ma c’è così tanto potenziale.

Hai presente tutte le operazioni di scrittura ben poco creativa che bisogna fare ogni giorno?

In particolare, mi riferisco alle **e-mail**.

Ho un brutto rapporto con le e-mail ( e detto da chi scrive una newsletter sembra assurdo, lo so), perché possono essere un **buco nero di distrazione**.

Quindi, oltre a limitarne la lettura ad orari fissi, cerco anche di renderne efficiente la scrittura, tranne nei casi che meritano un tocco più umano (come la scrittura della newsletter).

E Notion AI mi aiuta proprio a gestirle al meglio.

Le e-mail adatte fanno questo **percorso**:

*   da Gmail finiscono su Notion;

*   lì chiedo al Notion AI di aiutarmi scrivendo una risposta (e magari ritoccandola io);

*   da Notion ripassano su Gmail come risposta.

Inoltre, quando mi sento pigro, il passaggio da Gmail a Notion e da Notion a Gmail, lo faccio fare a qualche automazione.

​

### **CALL INDIMENTICABILI**

Questa è la cosa che più mi piace.

Ti permette di svoltare la tua **produttività** risparmiando un sacco di tempo.

Quando Beatrice e io facciamo una call come [Notion Builders](https://www.notionbuilders.it/), nel caso in cui possiamo registrarla, accadono una serie di **cose spettacolari**:

*   la registrazione è fatta da Google Meet e finisce su Google Drive, in automatico;

*   da Google Drive passa a Notion in un database specifico (tramite automazione);

*   da Google Drive passa anche su un tool che trascrive l’audio (tramite automazione);

*   la trascrizione finisce su Notion e lì Notion AI la trasforma in meeting notes e una to-do list.

Sembrano tutte piccole azioni, lo so.

Ma ripetute decine di volte in una settimana risultavano in ore che oggi possiamo dedicare ad altro.

​

​

Cosa significa quello che ho scritto finora?

Significa che Notion AI è il tool migliore di intelligenza artificiale?

Significa che ChatGPT è meglio?

La verità è che non ne ho idea.

Qualche newsletter fa era ChatGPT a vincere il primo (impari) confronto.

Ora invece devo dire che utilizzo molto più spesso Notion AI.

E si tratta ancora di una funzione non integrata al 100%, non ci puoi costruire automazioni (per esempio).

Diciamo che la gara tra i due tool è iniziate e non ho idea di come finirà.

Nel frattempo, noi comuni mortali, possiamo solo goderci la competizione e **migliorare la nostra efficienza**.

E detto questo, per oggi è tutto, buona settimana e **beccati le risorse**.

​

Daniele
