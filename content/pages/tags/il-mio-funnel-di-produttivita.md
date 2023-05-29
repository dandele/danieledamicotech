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
title: "\U0001F9F0 kSC #40: IL MIO FUNNEL DI..."
colors: colors-a
date: '2023-05-28'
description: PRODUTTIVITÀ
featuredImage:
  type: ImageBlock
  altText: Project thumbnail image
  caption: ''
  url: /images/Frame 14.webp
media:
  type: ImageBlock
  url: /images/Frame 14.webp
bottomSections:
  - type: CtaSection
    colors: colors-f
    elementId: ''
    backgroundSize: full
    actions:
      - label: CHE NE PENSI?
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://www.linkedin.com/in/daniele-damico/'
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-0
          - pb-28
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: col
      title:
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nPer creare un'audience devi essere in grado di gestire l'attenzione delle persone (cosa che spero di aver fatto al meglio nella newsletter di oggi).\n\n​[Ecco 7 modi con cui puoi riuscirci quando scrivi.](https://collabfund.com/blog/attention/?utm_source=ForTheInterestedNewsletter)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nDopo una newsletter come quella di oggi, un altro link sulla produttività potrebbe essere eccessivo, no?\n\n​[Ma se proprio non ti bastano, ora sarai felice.](https://nesslabs.com/illusion-of-productivity)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nPer riuscire a monetizzare devi imparare a utilizzare il prezzo di quello che offri.\n\n​[E questa è una delle tecniche più importanti per riuscirci.](https://customercamp.co/price-anchoring/)​\n"
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
slug: il-mio-funnel-di-produttivita
---
Ehi ciao 👋,

questo è il numero 40 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò del **ti parlerò del mio funnel di produttività**.

<br>

***

**TL;DR**

*   Come ho costruito il mio funnel di produttività;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti.

***

<br>

Per quanto Notion sia l’hub centrale in cui tante cose della mia vita avvengono, non è il solo tool che utilizzo per essere produttivo.

Anzi, ti dirò che **identificare un tool come intero sistema di produttività è un tantino esagerato**.

I tool sono strumenti che si collocano in determinate fasi/aree del tuo **funnel di produttività**.

E nel mio funnel, Notion ha un posto al fianco di altri tool.

E ora ti dico quali sono.

<br />

## **IL DEMONE NASCOSTO DIETRO LA PRODUTTIVITÀ TOSSICA**

Ora, prima serve capire che cosa intendo quando parlo di funnel della produttività?

Cosa intendo per funnel di produttività?

Intendo il percorso con cui parti dalle infinite cose che puoi fare ed arrivi a fare effettivamente delle cose.

In pratica è il **percorso che ti porta dal caos alla produttività.**

È fatto da alcune fasi, e proprio come in un classico funnel, in ogni fase succedono cose.

E oggi ti svelerò quale tool utilizzo in ognuna di queste fasi.

*   Il regno di Notion: la fase di selezione

*   Il regno di Akiflow: la fase di organizzazione

*   La terra di Mezzo: la fase di esecuzione

Lo so, come in tutte le mie newsletter, i punti che ho citato sono criptici/fantasiosi.

Ma continua a leggere e vedrai che mi spiegherò meglio.



### **IL REGNO DI NOTION: LA FASE DI SELEZIONE!**

La fase di selezione è la prima fase del funnel, il momento in cui analizzi tutte le cose che hai da fare, scegli quelle su cui vuoi concentrarti e da far passare alle fasi successive.

In pratica è la **fase delle priorità**, il momento in cui più il tuo sguardo riesce ad essere olistico e meglio è.

Per questo, hai bisogno di un tool che centralizzi tutte le informazioni riguardo progetti, processi, risorse necessarie ecc.

E io utilizzo Notion.

Lo utilizzo perché è per me il tool che meglio funziona in quest’ottica.

Grazie a Notion riesco a gestire i progetti, i task, le risorse e tutto quello di cui ho bisogno per raggiungere un punto di vista olistico.

E in funzione di tutte queste informazioni, posso fare la mia selezione al meglio

C’è una **condizione fondamentale** però, devi essere disciplinato in questa fase e devi scegliere un solo tool: nel mio caso, Notion deve essere **l’unica sorgente di verità che ho sulle mie attività**.

E se ci sono altri tool di mezzo e quindi ci sono dubbi, allora le cose si complicano.

<br>

### **IL REGNO DI AKIFLOW: LA FASE DI ORGANIZZAZIONE**

Ok, una volta che hai deciso cosa devi fare è il momento di organizzarsi.

Questa è la seconda fase del funnel e in questo caso hai bisogno di tool che ti permettano di capire **cosa devi fare, quando devi farlo e come devi farlo**.

Per questo utilizzo [**Akiflow**](https://akiflow.com/).

Grazie ad Akiflow, e alla sua integrazione con Notion, posso prendere i task gestiti su Notion e utilizzarli per fare **time blocking** su Akiflow.

Chiariamoci, potevo fare time blocking anche utilizzando Notion e Make, solo che ho preferito utilizzare uno strumento verticale (e che mi evitasse qualche casino) per gestire questa fase così delicata del funnel.

In pratica, ho messo da parte il piacere di ottimizzare per fare effettivamente cose.



### **LA TERRA DI MEZZO: LA FASE DI ESECUZIONE**

Qui succede il casino.

Questa è la fase in cui, dopo aver deciso cosa fare, come farlo e quando farlo, **devi effettivamente fare le cose**.

Quindi non c’è un tool che domina sugli altri, dipende da quello che fai e quello di cui hai bisogno.

Ovviamente, nel mio caso, gran parte del lavoro per [Notion Builders](https://www.notionbuilders.it/) è fatta su Notion.

Ma ci sono tanti altri tool che utilizzo, in funzione della situazione e del task da fare.

Tra gli altri tool che utilizzo di più ci sono:

*   Figma

*   Google Drive

*   Figjam

*   Linkedin

*   Convertkit

*   Obsidian

*   Zcal

Insomma, questa è la fase in cui tutto dipende da te.

​

Essere produttivi non significa solo fare cose, ci sono tante altre variabili (e fasi) che devi considerare.

**E per ogni fase, c’è un tool più adatto.**

Non so se te hai mai visto il tuo lavoro in questi termini, ma prova a mappare la tua produttività in queste fasi.

E per le prime due, scegli un solo un tool da utilizzare.

Per la fase di esecuzione, invece, puoi essere più flessibile.

Poi, se hai domande su quale tool utilizzare in quale fase, **puoi rispondere a questa email** o **mandarmi un DM su Linkedin**, sono sempre disponibile ad aiutarti!

E ho giusto un po’ di esperienza con questi argomenti.

Buona settimana e beccati le risorse.

Daniele
