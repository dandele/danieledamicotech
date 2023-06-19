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
title: "\U0001F9F0 kSC #43: 3 SISTEMI DA USARE SU NOTION…"
colors: colors-a
date: '2023-06-18'
description: PER SCONVOLGERTI LA VITA
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nSahil Bloom fa numeri da record.\n\nIn 3 anni ha creato un'audience di 400mila persone, se non di più.\n\n​[E come ha fatto?](https://growthinreverse.com/sahil-bloom/)**​**\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nQuanto lavori?\n\nPoco o tanto?\n\nForse lavori un po' troppo e non è l'ideale.\n\n​[Ecco come puoi capirlo (e risolvere).](https://twitter.com/jspector/status/1663168391731879937)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nMonetizzare non è la parte finale del tuo percorso da creator.\n\nE solo l'inizio di un altro percorso.\n\n​[Ed è così che puoi costruire il tuo.](https://nathanbarry.com/creator-flywheels/)​\n"
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
slug: 3-sistemi-da-usare-su-notion-per-sconvolgerti-la-vita
---
Ehi ciao 👋,

questo è il numero 369 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò di **Notion Projects..**

<br>

***

**TL;DR**

*   Notion Projects: che roba è?

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti.

***

<br>

Sono sempre contento quando escono nuove feature di Notion perché significa che ho nuovi giocattoli con cui fare magie.

Il fatto è che, per ogni nuova feature di Notion, io, Beatrice e le tante altre migliaia di persone nel mondo che usano Notion, abbiamo un’arma in più per fare quello di cui c’è bisogno.

E da qualche settimana **è uscita Notion Projects**, la nuova feature di Notion, che punta a fare alcune cose carine.

​

## **NOTION PROJECTS: CHE ROBA È?**

Notion Projects nasce come un insieme di feature e ha l’obiettivo di aiutare le persone a gestire i progetti.

Chi lo avrebbe mai detto, eh?

In particolare, Notion Projects è:

*   Un mix efficace di vecchio e nuovo;

*   Un template sotto steroidi;

*   Un chiaro segnale da parte di Notion;

Tutto chiaro fino a qui?

Allora possiamo iniziare!

​

### **UN MIX DI VECCHIO E NUOVO**

Ho scoperto dell’esistenza di Notion Projects in modo particolare.

Perché quando utilizzi qualcosa tutti i giorni e d’improvviso cambia, lo noti subito.

Così qualche giorno fa, mentre lavoravo per un cliente di Notion Builders, ho notato che erano spuntate alcune nuove proprietà nei database.

E non erano delle proprietà qualsiasi, erano le proprietà che aspettavo fin dall’arrivo di ChatGPT e di Notion AI: **proprietà database potenziate dall’intelligenza artificiale!**

In pratica, ti permettono di utilizzare l’AI per fare cose con i database.

Le proprietà sono: 

*   AI Summary; 

*   AI Key Info;

*   AI Custom Autofill.

Poi ho esplorato un po’ di più e ho scoperto altre proprietà.

C’erano: 

*   Collegamento a Figma; 

*   Collegamento a Google Drive: 

*   Collegamento a GItHub.

E poi un’altra ancora, anche questa “nuova”, più o meno: **la proprietà ID**.

Solo che questa non era nuova per davvero.

La proprietà ID, infatti, genera un ID per i record di un database.

Ed è una cosa che, fino al suo arrivo, potevi creare tramite una **semplice formula ID**.

E quindi?

Continua a leggere e capirai.

​

### **UN TEMPLATE SOTTO STEROIDI**

Insomma, ho giocato un po’ con queste nuove aggiunte e ho scoperto che rientravano in **Notion Projects**.

E cos’è Notion Projects?

È una forte spinta da parte di Notion verso la **gestione di progetti**.

Una spinta che all’atto pratico puoi trovare in queste nuove proprietà e nel rilascio di un **template gratuito ottimizzato** proprio per la gestione progetti.

E basta, poi arriveranno altre cose (che sembrano fighe), ma per ora non ci sono ancora.

Insomma, per fartela breve, **Notion Projects è un nuovo template**.

Un template fatto da Notion, gratuito e ottimizzato per le nuove proprietà e quindi per la gestione progetti.

Fighissimo, per carità, ma **nulla di nuovo per davvero**.

E quindi, non capivo quale fosse la sua utilità.

​

### **UN CHIARO SEGNALE DA PARTE DI NOTION**

Poi ci ho ragionato un po’ meglio.

Ho capito che, con questo rilascio, **Notion ha preso una posizione**.

Anzi, ha proprio urlato:” We vedete che potete usare anche per me gestire i progetti, togliete di mezzo gli altri tool più costosi e complicati, ci penso io”.

E non l’ha fatto abbandonando quanto costruito finora, ha solo rimescolato le carte e fatto qualche piccola aggiunta (la parte di AI).

Così, non ha reso vana l’attività delle tante persone che hanno notato queste potenzialità nello strumento, prima ancora che fossero ufficialmente note.

In pratica, Notion ha preso le costruzioni particolari, i modi di fare cose più utilizzati dalla community di **utilizzatori avanzati** dello strumento (in particolare i consulenti), le hanno rese parte di un pacchetto e hanno dato loro risalto.

Secondo me, hanno fatto una **genialata**.

​

​

Ora, non so se sia davvero questo che hanno fatto, è tutta una mia interpretazione.

Inoltre, ho anche capito una cosa.

Ad un primo impatto, credevo che una feature del genere, permettendo di fare più cose all’utente con conoscenze più basilari, potesse creare **problemi ai consulenti**.

Invece, ho capito che mi sbagliavo.

Perché con questa nuova aggiunta, **Notion diventa uno strumento ancora più complesso da gestire**.

E questo rende realtà come [Notion Builders](https://www.notionbuilders.it/), ancora più centrali nell’ecosistema.

E niente, la cosa mi ha reso felice.

Detto questo, buona settimana e **beccati le risorse**.

Daniele
