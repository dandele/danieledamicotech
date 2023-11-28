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
title: "\U0001F9F0 kSC #65: Il successo dei tuoi progetti..."
colors: colors-a
date: '2023-11-26'
description: PARTE DAL LORO FALLIMENTO!
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
    text: "## **\U0001F465 Tutti abbiamo bisogno di scrivere meglio**\n\nLa scrittura è forse lo strumento più importante da padroneggiare per creare una tua audience.\n\nE tutti abbiamo bisogno di scrivere meglio.\n\n​[Per questo, anche tu dovresti leggere questa cosa qui.](https://joshspector.com/how-to-become-a-better-writer/)​\n\n​\n\n## **\U0001F680 Rapidità e struttura per le tue note**\n\nSono convinto che l'efficacia di uno strumento di personal knowledge management sia collegata alla velocità con cui possiamo creare delle note.\n\nNotion e Obsidian ti permettono di farlo, ma non sono gli strumenti più rapidi.\n\nAltri strumenti, invece, sono rapidi ma non hanno struttura.\n\n​[E se fosse appena uscito lo strumento che unisce rapidità a struttura?](https://lazy.so/)​\n\n​\n\n## **\U0001F4B8 Come monetizzare i tuoi prompt?**\n\nFai cose con l'AI?\n\nHai cominciato a giocare con i tuoi prompt, i tuoi GPTs ecc?\n\n​[Allora questa è una cosa che potresti utilizzare a tuo vantaggio.](https://promptologer.com/)\n\n"
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
slug: il-successo-dei-tuoi-progetti-parte-dal-loro-fallimento
---
Alla base del Second Brain di Tiago Forte ci sono i **progetti**.

Infatti, nell'acronimo PARA, la P iniziale sta proprio per Projects.

Quindi i progetti sono roba grossa.

E per questo è importante scegliere bene **a quali progetti dedicarsi** e fare di tutto per **portarli al successo**.

Solo che quando lanciamo un nuovo progetto, dobbiamo fronteggiare la **fase di innamoramento dei progetti.**

Ed è una fase pericolosa, perché rischia di farci mandare tutto all'aria.

​



**TL;DR**

*   Vuoi rendere i tuoi progetti un successo? Allora parti dal loro fallimento!

*   Tutti abbiamo bisogno di scrivere meglio

*   Rapidità e struttura per le tue note

*   Come monetizzare i tuoi prompt?

**Il tempo di lettura previsto è**: 4 minuti e 30



​

Diciamoci la verità, quando comincia un nuovo progetto è tutto bello.

Siamo tutti ottimisti.

Tutti convinti che le cose andranno come vogliamo e che il progetto sarà un successo.

Non ci sarà neanche mezza complicazione, tutto filerà liscio come l’olio.

E questa sensazione regge, fino a quando poi non regge più.

Alcune cose ci colgono impreparati, arrivano le prime **complicazioni**.

Allora impariamo, troviamo soluzioni e ci adattiamo.

Poi però arriva un nuovo progetto e il ciclo ricomincia.

Lo so che sembra un ciclo inevitabile, ma penso di aver trovato una **soluzione** (e due tattiche per metterla in pratica):

*   devi partire dal fallimento;

*   come anticipare il fallimento;

*   come anticipare il fallimento con Notion.

E ora, come al solito, te le racconto.

​

### **Devi partire dal fallimento**

Ok, in questo punto devo cercare di non essere lugubre.

Ma hai presente l’autopsia?

Dai su, ti sarà capitato di vedere almeno una puntata di CSI.

Oppure di qualsiasi altro telefilm.

Qualche tempo fa, ho scoperto che l'autopsia la puoi fare pure ai **progetti**.

E di solito prende la forma di report, o documenti, scritti su come è andato il progetto e perché è stato un fallimento.

Solo che questa autopsia ha un piccolo problema: **non è retroattiva**.

Ci fornisce lezioni importanti sul passato, ma non ci aiuta a plasmare il futuro (non direttamente, almeno).

Mi segui fin qui?

Ok, perché ora ti invito ad usare l’**immaginazione**.

Invece di fare cose quando il progetto è finito, falle quando il progetto sta per iniziare!

Insomma, **scrivi un pre-mortem invece di un post-mortem**.

In questo modo, potrai anticipare le possibili cause di fallimento.

Non ci saranno più cose che ti colgono alla sprovvista ed avrai sempre un piano di risposta pronto.

Ma come ci puoi riuscire?

​

### **Come partire dal fallimento**

Ci sono alcune domande che ti puoi fare e che ti aiuteranno a ipotizzare il peggio.

*   Quali sono gli obiettivi principali del progetto?

*   Abbiamo sufficienti risorse (umane, finanziarie, tecnologiche) per completare il progetto?

*   La pianificazione è realistica? Ci sono possibili ritardi previsti?

*   Abbiamo un piano di risposta a eventuali problemi tecnici?

*   Come monitoreremo il progresso del progetto?

*   Qual è il peggiore scenario possibile per il progetto?

E diciamoci la verità, sono tutte domande che dovrebbero aiutarti a ipotizzare gli scenari peggiori del tuo progetto.

Hanno la stessa funzione delle domande di cui ti ho parlato [qui](https://danieledamico.tech/tags/quando-non-hai-altra-scelta-utilizza-obsidian/).

E proprio come quelle domande, il posto dove te le fai è irrilevante ma io **ti consiglio Notion**.

Ora ti mostrerò come puoi utilizzarle su Notion, perché è lì che **gestisco i miei progetti**.

​

### **Come anticipare il fallimento, su Notion**

Tutto quello che devi fare è inserire queste domande come **template di un database documenti** (o note) nel tuo spazio Notion.

Puoi chiamare il template "pre-mortem".

*​*

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/sbfjjS2p1kAntkmucY8q6m) |
| --------------------------------------------------------------------------------- |

​

Poi, devi **collegare il database in cui ospiti tutti i tuoi progetti** a quello in cui ospiti le tue note.

*​*

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/ohEvuNWyZ5uZj8mArXyLYg) |
| --------------------------------------------------------------------------------- |

​

In questo modo, dalla dashboard in cui gestisci i tuoi progetti, potrai **creare un nuovo pre-mortem** per il relativo progetto e compilarlo subito.

*​*

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/pVDJLkwDv113GNXEPrRfwv) |
| --------------------------------------------------------------------------------- |

*​*

E fidati, così partirai fin dall'inizio con le idee chiare.

​

​

Mi fermo qui con la spiegazione, anche se si possono fare tante altre cose.

Puoi creare dashboard che ti mostrano solo i progetti privi di pre-mortem, così puoi rimediare.

Puoi creare dashboard che ti aiutano a far partire un progetto solo se hai compilato il pre-mortem.

E addirittura **puoi sfruttare l'AI per aiutarti con la compilazione del pre-mortem** (l'ho già fatto, è fighissimo).

Ma sono tutte complicazioni che potrebbero essere superflue, il **minimo indispensabile è quello di prendere due database e incrociarli.**

Sembra poco, ma può avere un grande impatto sul successo dei tuoi progetti.

Detto questo, per oggi è tutto.

Buona settimana e beccati le risorse,

Daniele

