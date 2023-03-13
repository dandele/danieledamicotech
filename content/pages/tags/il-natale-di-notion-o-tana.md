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
title: "\U0001F9F0 kSC #29: Il NATALE DI NOTION..."
colors: colors-a
backgroundImage:
  type: BackgroundImage
  url: /images/bg2.jpg
date: '2023-03-13'
client: Awesome client
description: O TANA?
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
slug: il-natale-di-notion-o-tana
---
Ehi ciao 👋,

questo è il numero 29 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò di **come gestisco i meeting notes**.

***

**TL;DR**

*   Meeting notes efficaci;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 40.

***

Tool come Notion, Obsidian e Tana mi attirano perché li puoi trasformare nel tuo secondo cervello.

Li puoi utilizzare per **salvare informazioni** e per **organizzarle** come vuoi.

Poi, se prendi la tangente come me, arriverai presto al punto di **pianificare processi** per salvare le informazioni nel tuo secondo cervello.

Ma questo è un altro discorso.

Il punto è che, una volta scoperto il loro potenziale, presto cercherai di salvare un tipo di informazioni in particolare: gli **appunti dei meeting**.

O meglio, detto con tono meno da manager: gli appunti delle c\*\*\* di call.

<br>

## **MEETING NOTES EFFICACI**

Un po' come tutti, ormai anche la mia vita è costellata da un numero di call molto più alto di quanto vorrei.

È una di quelle cose della vita che devi accettare, un po' come il fatto che Blanco deve stare lontano dai fiori.

Ma visto che nelle call ci si scambia spesso **informazioni vitali**, ho cercato di definire il **processo migliore** per non perdere queste informazioni.

Senza passare ore a trascrivere registrazioni, oppure non ascoltare chi ti sta parlando.

Ed il processo richiede solo tre cose:

*   Un database;
*   Una piccola automazione;
*   Un semplice template.

Il tool che utilizzo, come forse saprai, è Notion ma una cosa simile si può mettere in piedi anche su altri tool (con le dovute differenze).

<br>

### **UN DATABASE**

Questo è la prima cosa di cui hai bisogno: un **database dove raccogliere tutti gli appunti**.

E puoi chiamarlo "meeting notes" oppure in altri modi, decidi tu.

Una cosa importante che devi considerare però è la complessità di questo database ed il **numero di informazioni che conterrà**.

Se fai tante call e ci tieni ad avere database puliti, allora conviene che questo sia un database in cui salvi solo i meeting notes.

Se invece preferisci avere meno database sul tuo workspace, allora puoi integrare i meeting notes in altri database.

Ad esempio, per le call di [Notion Builders]([https://www.notionbuilders.it]\(https://www.notionbuilders.it/\)), Beatrice ed io salviamo i meeting notes in un database chiamato Documents.

Ed in questo database ci finiscono non solo i meeting notes ma anche altre informazioni.

Inoltre, a questo database, è collegato il **database CRM**, quello dei **progetti** e quello dei **task**: in questo modo ogni informazione è in rete con le altre, è accessibile da più punti.

Insomma, ad ogni call che facciamo corrisponde una pagina nel database Documents, taggata come Meeting Notes e con al suo interno la possibilità di assegnare clienti, progetti e task.

Una possibilità che può essere **automatica** oppure no, dipende da te.

Noi abbiamo scelto di renderla automatica.

<br>

### **UNA PICCOLA AUTOMAZIONE**

Questo è un punto interessante.

Perché non è necessario: non tutto deve per forza essere reso automatico.

Noi però abbiamo deciso di renderlo tale.

Quindi, abbiamo costruito una **piccola automazione su Make** che fa queste cose qui:

*   quando un nuovo evento viene creato sul Calendar delle call di Notion Builders parte l'automazione;
*   Make recupare le informazioni da questa call e crea una pagina all'interno del database Documents;
*   Make darà alla pagina lo stesso titolo dell'evento;
*   nel caso in cui sia presente, Make associa a quella pagina la persona del CRM con cui faremo la call;
*   nel caso In cui non sia presente, Make crea quella persona nel database CRM;
*   alla creazione di una voce nel CRM, Notion associa un progetto standard a quella voce e a sua volta determinati task.

La cosa potrebbe andare avanti ancora e ancora, ma Beatrice ed io non ne abbiamo bisogno.

E magari non ne hai bisogno neanche tu.

È tutta roba che ti fa **risparmiare un bel po' di tempo**, ma è anche **complessa**.

<br>

### **IL TEMPLATE MEETING NOTES**

Questa cosa ti serve invece.

Così come il database, è obbligatoria.

Altrimenti come li prendi appunti? Senza struttura?

Non mi sembra il caso, dai.

Il punto di questo template è poter inserire con facilità le **informazioni più importanti riguardo la call**, le cose che poi serviranno per le **prossime azioni**.

E quindi spetta a te delineare la struttura e capire cosa inserire nei tuoi appunti.

Sono gentile però e quindi ecco la struttura del nostro template:

*   **Meeting agenda**: un campo con tutte le cose che bisogna trattare nel corso della call ed il sistema su Notion fa in modo che questo campo sia già popolato;
*   **Next actions**: i prossimi passi da mettere in atto, emergono nel corso della call;
*   **Meeting precedenti**: una vista filtrata degli appunti delle call precedenti con la stessa persona ed eventuali registrazioni;

<br>

Spero di essere stato chiaro e di averti fatto capire due cose in particolare: la **facilità** di poter creare un sistema del genere e la sua **flessibilità**.

Perché penso che su quanto sia **necessario** siamo tutti d'accordo, no?

E detto questo, buona settimana e beccati le **risorse**.

Daniele
