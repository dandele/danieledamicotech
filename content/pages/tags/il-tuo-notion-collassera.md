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
title: "\U0001F9F0 kSC #37: IL TUO NOTION COLLASSERÀ?"
colors: colors-a
backgroundImage:
  type: BackgroundImage
  url: /images/bg2.jpg
date: '2023-05-07'
description: 3 domande per evitare il disastro
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
      - label: "FAI LA TUA ANNUAL REVIEW \U0001F680"
        altText: ''
        url: /tags/easy-annual-review
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nC’è una cosa importante da ricordare quando crei qualcosa.\n\nEd è importante per capire quanto potenziale di successo avrà.\n\n​[A chi interessa?](https://twitter.com/jspector/status/1608953455250661376)\n\n\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nSei ancora in vena di previsioni e lezioni?\n\n​[Allora beccati anche queste](https://www.justinwelsh.me/e/BAh7BjoWZW1haWxfZGVsaXZlcnlfaWRsKwi38jBundefined3D--39f460dfe6545309d8232a46a66af297b086647a?skip_click_tracking=true)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nQuali sono i prerequisiti per fare monetization?\n\n​[Eccoli qui](https://twitter.com/jonbrosio/status/1609187680302125057)​\n"
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
slug: il-tuo-notion-collassera
---
Che sensazione provi quando concludi un task e **metti quella X nella to-do list**?

Bella vero?

E cosa provi quando fai la stessa cosa, ma per il task successivo?

Sempre bella, anche se forse un po' meno, vero?

Ma ti sei mai fatto una domanda?

Che succede se l'obiettivo per cui stai eliminando così tanti punti dalla tua task list, fosse un **obiettivo che non vuoi davvero**?

***

**TL;DR**

*   Come NON diventare un robot?

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti e 24.

***

Ehi ciao 👋,

questo è il numero 20 del **Kit di Sopravvivenza per Creator**.

Ed oggi ti racconterò **come NON diventare un robot.**

<br />



La fine dell'anno è sempre un periodo di **riflessioni**.

Fatti un giro su un social a caso.

Decine di post di persone la cui vita non ti riguarda neanche un po' e che condividono il loro fantastico anno di cui non ti importa neanche un po'.

C'è da dire però che riflettere sulle vicende dell'ultimo anno è utile.

Ti permette di **ragionare su quanto fatto e ti permette di impostare una direzione per il futuro**.

Ma anche più di questo: **ti evita di diventare un robot**.

Ti evita di diventare una macchina da task, che li esegue ed elimina dalla sua lista personale, senza sapere l'obiettivo per cui lo fa.

E se si chiede "Perché l'ho fatto?", si rompe.

Parlo per esperienza, mi ci sono trovato anni fa in questa situazione.

Ed è così che ne sono uscito.

​

## COME NON DIVENTARE UN ROBOT?

La soluzione è semplice: **devi essere consapevole**.

Devi solo chiederti perché fai quello che fai, a cosa punti ecc.

Ma sapere la soluzione non basta, quello che serve è **l'esecuzione**.

Perché non ero in grado di rendere la mia esecuzione più consapevole?

*   perché non sapevo cosa chiedermi;

*   non sapevo dove chiedermelo;

*   non sapevo come chiedermelo.

E nel tentativo di risolvere questi dubbi ho scoperto l’esistenza dei **Review Cycles**.

Che in questo periodo di fine dell’anno ed inizio dell’anno prossimo, prendono la forma di **Annual Review**.

Ed ecco come strutturare la tua Annual Review per il 2023.

​

### COSA CHIEDERSI NELL'ANNUAL REVIEW?

Diciamoci la verità, la ciccia dell’Annual review è proprio in questo punto.

Quello che ti chiedi (e cosa rispondi) è ciò che ha più **impatto** nel definire una direzione per i tuoi prossimi 12 mesi.

Per questo è importante definire una **struttura** e capire quali domande ha senso porsi.

Sull’argomento ci hanno ragionato tante persone: da **Ali Abdaal**, ad **August Bradley** fino a **Sahil Bloom**.

Ed è proprio la struttura di Sahil che seguo.

Analizza gli ultimi 12 mesi e pianifica i prossimi da questi punti di vista:

*   **Big Goals**: verso quali obiettivi grandi ed a lungo termina hai lavorato?
    Quali hai raggiunto?
    Quali non sono più validi? Quali nuovi Big Goals sono emersi e vorresti raggiungere?
    ​
    ​*Esempio: raggiungere i 1000 iscritti a questa newsletter nel 2023
    ​*

*   **Checkpoint Goals**: ora che hai definito i Big Goals, analizzali e rendili più semplici.
    Scomponi i Big Goals in obiettivi più piccoli, definiti e raggiungibili.
    ​
    ​*Esempio: raggiungere 500 iscritti entro giugno 2023
    ​*

*   **Daily Systems**: queste sono le azioni che, fatte di giorno in giorno, ti permettono di raggiungere prima i Checkpoint Goals e poi i Big Goals.
    ​
    ​*Esempio: scrittura newsletter quotidiana e newsletter settimanale
    ​*

*   **Anti-Goals**: cosa NON vuoi che accada nel tuo percorso per raggiungere i Big Goals?
    È importante farsi questa domanda, perché arriverai al punto in cui dovrai darti delle priorità e così non andrai in tilt.
    ​
    ​*Esempio: non permettere alle mie altre attività di farmi trascurare la newsletter*

*​*

### DOVE FARE L'ANNUAL REVIEW?

La risposta a questa domanda è semplice: **utilizza lo strumento con cui gestisci le tue attività quotidiane**.

Visto che io gestisco la maggior parte delle mie attività su Notion, è su **Notion** che faccio l’Annual Review.

Ma questo non significa che tu debba fare lo stesso: è più importante fare l’Annual Review che farla su Notion.

Ecco **altri tool** che potresti utilizzare:

*   Obsidian;

*   Roam Research;

*   Tana;

*   Evernote;

*   Todoist.

Se posso darti un consiglio però, ti direi di scegliere un tool che ti permette di **costruire sistemi**.

Solo in questo modo potrai cogliere al 100% i vantaggi e l’impatto positivo che l’Annual Review avrà sulla tua vita.

​

### COME FARE L'ANNUAL REVIEW?

Anche in questo caso, **fatto è meglio che perfetto**.

E l'importante è fare la tua annual review entro le **prime settimane di gennaio**, altrimenti perdi la motivazione.

Su Evernote puoi anche creare una semplice lista.

Mentre su Notion puoi creare un **sistema più complesso**, come quello che nel corso degli anni ho creato io.

​![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/ojq8c7koUxUegCyztzb5V9/email)

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/54YL7YwwdceezkUjJTHBtA/email)​

Poi, ci sono tante altre **regole** che potresti seguire per fare la tua Annual Review.

Ci sono tante domande che ti potresti fare.

Ma la cosa più importante, fidati che ci sono passato, è proprio quella di farla.

Tra **complessità e semplicità scegli la seconda**: non deve essere nulla di figo, complesso o perfetto, deve essere qualcosa di utile!

​

Ora, non ti posso dire che facendo l'Annual Review il tuo anno sarà fantastico e raggiungerai i tuoi obiettivi.

Te lo auguro, ma non te lo posso promettere.

Posso dirti però che con un Annual Review in tuo supporto, sarai in grado di affrontare qualsiasi progetto del 2023 con la consapevolezza necessaria per trarne il meglio.

In più, dato che voglio aiutarti a raggiungere i tuoi obiettivi ho pensato una cosa.

Ho pensato di prendere la struttura della mia **Annual Review** e renderla un **template**.

Così non avrai scuse o problemi a farla, li avrò già risolti io per te!

**Clicca il pulsante** qui sotto e vedrai.

Detto questo, per oggi è tutto, buon 2023 e beccati le **risorse**.

Daniele
