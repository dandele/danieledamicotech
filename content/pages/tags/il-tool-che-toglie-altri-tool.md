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
title: "\U0001F9F0 kSC #30: Il tool che toglie..."
colors: colors-a
date: '2023-03-19'
description: altri tool
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
  - type: CtaSection
    colors: colors-d
    elementId: ''
    backgroundSize: inset
    title: Let's do this
    text: >-
      The Stackbit theme is flexible and scalable to every need. It can manage
      any layout and any screen.
    actions:
      - label: Try it now
        altText: ''
        url: /
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-28
          - pb-28
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: col
      title:
        textAlign: center
      text:
        textAlign: center
      actions:
        justifyContent: center
  - type: DividerSection
    title: Divider
    elementId: ''
    styles:
      self:
        width: narrow
        padding:
          - pt-36
          - pb-36
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    subtitle: null
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nTutti usano ChatGPT ormai.\n\nChe sia per giocare o per pubblicare quel post in cui dicono di aver usato ChatGPT.\n\nMa se vuoi usarla per davvero, magare per creare la tua audience?\n\n[Allora dovresti leggere sta roba.](https://www.neatprompts.com/p/create-a-social-media-calendar)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nIl potere di ChatGPT ormai è noto a tutti.\n\nMa presto cambierà tutto.\n\n[Presto arriverà la sua evoluzione, prima di quanto pensi.](https://www.heise.de/news/GPT-4-is-coming-next-week-and-it-will-be-multimodal-says-Microsoft-Germany-7540972.html)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nVuoi monetizzare?\n\nAllora non dovresti considerare solo come vendere di più.\n\n[Dovresti considerare anche queste cose.](https://www.thetilt.com/business-operations/personal-finance-for-creators)\n\n"
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
slug: il-tool-che-toglie-altri-tool
---
Ehi ciao 👋,

questo è il numero 30 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò di **come gestisco i meeting notes**.

***

**TL;DR**

*   Il tool che toglie altri tool

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 30.

***

Uno dei problemi che più mi ha rovinato la psiche nel corso degli anni è la gestione delle cose da leggere.

Nel corso di una giornata normale, **leggo parecchio** e cerco di salvare alcune informazioni nella forma di highlights e note varie.

Inoltre, utilizzo spesso **LinkedIn** e **Twitter** e lì spesso incontri dei contenuti interessanti.

Io salvo quei contenuti e vorrei magari sottolinearli, farci cose.

Fino a qualche mese fa utilizzavo Instapaper per le funzioni di Read it Later e devo dire che mi trovavo bene.

Solo che poi ho notato sempre di più alcuni problemi.

<br>

## **IL TOOL CHE TOGLIE ALTRI TOOL**

L'esperienza di lettura su **Instapaper** è fantastica, non prendiamoci in giro.

Sembra di leggere un libro, anche se stai leggendo dallo schermo di un PC.

Ma col passare del tempo, Instapaper ha mostrato sempre più **carenze** e non trovavo altri tool che riuscissero a soddisfare le mie esigenze:
-   Volevo un tool integrato con Readwise;
-   Volevo un tool in cui poter leggere libri, tweet, PDF e tutti gli altri formati di contenuti che mi possono interessare;
-    Volevo un tool che mi permettesse anche di sottolineare dal web.

E per mia estrema gioia, qualche mese fa, ho trovato proprio quello di cui avevo bisogno.

Si chiama **Readwise Reader**.

<br>

### **UN TOOL INTEGRATO CON READWISE**

Diciamoci la verità, questo era il minimo indispensabile.

Se Readwise, crea un prodotto che faccia da lettore e **Read It Later**, il minimo che ti aspetti è che sia integrato con Readwise.

E infatti così è.

E questa **integrazione funziona benissimo**.

Basta salvare un contenuto, un libro, un pdf, qualsiasi cosa su Readwise Reader, cominciare a leggere, sottolineare cose e potrai vedere la magia.

In poco tempo troverai sul tuo Notion, Obsidian (o qualsiasi altro tool) i tuoi highlights e potrai farci cose.

<br>

### **UN TOOL DI LETTURA COMPLETO**

Bisogna ammettere una cosa, sul primo punto anche Instapaper era più che soddisfacente.

È questo secondo punto che ha avuto davvero impatto sulla mia scelta.

Si, perché su Instapaper c'erano alcuni **contenuti** che proprio non riuscivi a salvare.

I tweet, i video di YouTube ecc.

E questo è un problema, perché per risolverlo era necessario **salvare i contenuti all'interno della stessa app oppure su Notion**.

Con la prima opzione però non potevi comunque farci nulla, nella seconda opzione invece potevi lavorarci ma in poco tempo ti ritrovavi con una **Inbox infinita**.

Con Readwise Reader è tutto **risolto**.

Puoi importare i contenuti in diversi modi e non ci sono limiti al tipo di contenuti.

Puoi salvare i video di **YouTube**? 

Si, puoi farlo e Readwise Reader provvede addirittura a fartene una **trascrizione automatica**.

Puoi salvare i post di **LinkedIn** o **Twitter**?

Si e l'operazione è **immediata**.

Poi vai su Readwise, leggi, sottolinei e in poco tempo le tue note finiscono sul tool di knowledge management che hai scelto.

Questa cosa è una **bomba**, ora non devo utilizzare più Notion come bacino di salvataggio di cose che mi attirano ma che poi, una volta finite in Inbox, non leggerò mai.

Ora posso utilizzare **Readwise Reader come Read it Later** e **Notion** (in combinazione con Obsidian) **per gestire le informazioni**!

<br>

### **UN TOOL PER SOTTOLINEARE DAL WEB**

Questo è un punto un po' da viziati, lo riconosco.

Il fatto è che certe volte non voglio cambiare contesto, trovo un articolo interessante e lo voglio leggere lì, subito, senza posticipare.

E anche in questo caso Readwise Reader mi aiuta.

Salvo il contenuto su Readwise Reader e poi mi basta **evidenziare le parti di contenuto che mi interessano per poterle sottolineare**, proprio come fossi su Readwise, solo che sono sull'articolo stesso.

Non mi sono spostato e non ho cambiato contesto: **concentrazione fissa**.

<br>

Come potrai intuire, Readwise Reader è davvero una bomba e ne sono un grande fan.

L'unico problema è che richiede l'utilizzo di Readwise, se vuoi sfruttare la possibilità di salvataggio degli highlights sul tuo tool di knowledge management preferito.

Io lo faccio e ne sono più che soddisfatto.

Perché diciamoci la verità, viviamo in un mondo di contenuti e il **modo migliore per produrre cose di qualità è quello di consumare cose di qualità**.

Ma se le perdi per strada, non potrai mai coglierne il potenziale completo.

Ah, considera inoltre che al momento **Readwise Reader è in beta**!

Questo significa che, al netto di qualche piccolo bug, quello che ti ho detto oggi è solo l'inizio.

Se vuoi provarlo, qui trovi il link di affiliazione, così puoi provare Readwise per un mese gratis.

Magari poi li puoi utilizzare per salvare questa newsletter, oppure per salvare il mio primo tutorial su Notion, no?

Lo trovi su Youtube, ti basta cliccare il pulsante qui sotto!

E per oggi è tutto, buona settimana e beccati le risorse.

Daniele