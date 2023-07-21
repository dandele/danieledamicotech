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
title: "\U0001F9F0 kSC #48: system thinking e notion..."
colors: colors-a
date: '2023-07-23'
description: LA (POCO) STRANA COPPIA!
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
      - label: PORTA IL SYSTEM THINKING SUL TUO NOTION!
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://zcal.co/notionbuilders/quick-talk'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nSe vuoi fare audience building devi capire una cosa, l'arrivo di un nuovo social è sempre una buona opportunità.\n\nCosì puoi approfittare della spinta di attenzione e novità che quel social ha, almeno per i primi tempi.\n\n​[Per questo, dovresti sapere di questo nuovo arrivo.](https://futuresocial.beehiiv.com/p/threads-101-strategy-guide-brands)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nIl task manager più veloce in assoluto è qui.\n\n​[E no, non è Notion.](https://godspeedapp.com/)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nUno dei concetti più interessanti elaborati da Naval Ravikant è quello del personal monopoly.\n\n​[E questo è un modo con cui puoi trovare il tuo, usando l'AI!](https://aisolopreneur.beehiiv.com/p/use-chatgpt-build-navals-personal-monopoly)​​\n"
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
slug: system-thinking-e-notion-la-(poco)-strana-coppia
---
Ehi ciao 👋,

questo è il numero 368 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò di **cos’è il system thinking e che legame ha con Notion.**

<br>

***

**TL;DR**

*   System thinking e Notion: la coppia (poco) strana

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti.

***

<br>

Nel corso dei mesi ho cambiato spesso il mio parere su Notion.

All’inizio pensavo che fosse un semplice strumento per prendere appunti, un po’ come tutti.

Poi, col passare del tempo, ho capito che Notion era in grado di fare qualcosa di più.

Ti permetteva di costruire le soluzioni più adatte alle tue esigenze, unendo database e grafica, un vero e proprio strumento no-code.

Poi però ho capito un'altra cosa.

Notion non ti permette solo di creare lo strumento più adatto alle tue esigenze.

Ti permette anche di **collegare diversi strumenti tra loro**, tutti nello stesso spazio.

In pratica, è lo strumento migliore per **mettere in pratica il system thinking**.

Ma cos’è il system thinking?

​

## **SYSTEM THINKING E NOTION: LA COPPIA (POCO) STRANA**

Lo so.

So che quando pensi a system thinking hai in mente qualcosa, qualcosa di vago e poco strutturato.

Questo valeva anche per me fino a qualche tempo fa.

Poi ho approfondito l’argomento e ora capito alcune cose.

*   Cos’è il system thinking? Senza fuffa

*   Cosa costituisce un sistema?

*   Notion e system thinking?

​

### **COS’È IL SYSTEM THINKING? SENZA FUFFA**

Questa è forse una delle cose più difficili.

Perché quando si parla di system thinking il rischio di beccarsi una spiegazione fuffa è altissimo.

Per questo, ho pensato ad un’analogia che meglio ti permettesse di comprendere la cosa.

Hai presente un **puzzle**?

Un puzzle è composto da tanti piccoli pezzetti, tutti diversi tra loro.

Che succede se guardi un singolo pezzetto?

Niente di che.

Ma che succede se invece metti tutti i pezzetti insieme?

Vedi l’**immagine complessiva** del puzzle, magari una bella riproduzione di qualche quadro famoso.

E capisci pure che il puzzle non è composto solo dai singoli pezzetti ma anche dai **modi in cui questi si collegano tra loro** e tanti altri fattori.

Fin qui ci sei? Bene.

Pensare in sistemi significa **capire come le parti di un sistema (i pezzetti del puzzle) lavorano insieme e come i cambiamenti di una di queste parti possono avere un effetto sull’intero sistema**.

E quando capisci come funziona il sistema, puoi fare scelte migliori per farlo funzionare meglio.

​

### **COSA COSTITUISCE UN SISTEMA**

Ora che siamo allineati su cos’è il system thinking possiamo passare alla **definizione di sistema**.

Anche se spero che l’analogia del puzzle ti abbia dato qualche indizio.

“Un sistema è un insieme di elementi interconnessi tra loro e che concorrono al raggiungimento di un obiettivo.”

Ok, figo, ma che significa?

Significa che tutti i sistemi sono costituiti da tre cose in particolare:

*   **Elementi**: le parti che compongono il sistema. Possono essere persone, oggetti, idee o qualsiasi altra cosa che abbia un ruolo all’interno del sistema. Nel caso del puzzle sono i pezzetti che lo compongono.

*   **Relazioni**: le relazioni tra gli elementi del sistema. Queste indicano come gli elementi interagiscono tra loro e come possono avere un impatto sulle altre parti del sistema. Nel caso del puzzle possono essere i modi in cui i pezzetti si collegano tra loro.

*   **Scopo**: è quello che il sistema cerca di raggiungere. Perché ogni sistema esiste per un motivo specifico. Nel caso del puzzle è quello di mostrare la riproduzione del quadro famoso.

​

### **NOTION E SYSTEM THINKING**

E che legame c’è tra **Notion** e System Thinking?

Beh, mettiamola così: per spiegarti il system thinking ho usato l’analogia del puzzle.

Se invece volessi spiegarti come usare Notion, potrei fare l’**analogia con i lego**.

Tanti piccoli pezzetti che metti insieme e ti permettono di costruire qualcosa.

Insomma, stiamo parlando di cose molto simili.

Su Notion hai a disposizione decine di blocchi che puoi combinare per costruire qualcosa.

Poi puoi collegare quella cosa che hai costruito ad altre cose che hai costruito.

E puoi utilizzare parti di queste cose diverse per costruire altro.

In pratica, è un **puzzle digitale**.

Figurati che c’è un tipo di operazioni che puoi fare sui database che si chiama Relations, proprio come uno dei costituenti dei sistemi!

In pratica, Notion è uno strumento che porta in sé gli elementi stessi di un sistema e quindi ti permette di costruirli al meglio.

Solo che manca una cosa per renderlo lo strumento ideale di messa in pratica del system thinking.

**Lo scopo.**

E quello è compito tuo sceglierlo.

Tu o di chi costruisce il sistema per te.

Deve essere quella persona che monta il puzzle per te, seguendo lo scopo che le dai e conoscendo tutte le regole che ci sono tra gli elementi.

E fidati di me, trovare una persona di questo tipo è difficile.

​

Per questo, Beatrice ed io, non ci limitiamo alla costruzione di singoli strumenti per i clienti di [Notion Builders](https://www.notionbuilders.it/).

Perché se vuoi un sistema per gestire la tua startup, non ti basterà solo un CRM, oppure solo un task manager o solo qualche altro strumento.

Avrai bisogno di **più strumenti**, messi in relazione tra loro, costruiti con un approccio di system thinking.

Vuoi che lo facciamo anche per te?

**Clicca sul pulsante qui sotto** e prenota una call.

Detto questo, buona settimana e **beccati le risorse**!

Daniele
