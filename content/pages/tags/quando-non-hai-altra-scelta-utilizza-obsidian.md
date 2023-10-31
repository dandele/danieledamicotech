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
title: "\U0001F9F0 kSC #61: Quando Non HAI SCELTA..."
colors: colors-a
backgroundImage:
  type: BackgroundImage
  url: /images/bg2.jpg
date: '2023-10-22'
description: UTILIZZA OBSIDIAN!
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
    text: "## **\U0001F465 L’OBIETTIVO DI CHI SCRIVE (TANTO)**\n\nQuale dovrebbe essere l’obiettivo di chiunque crei contenuti di tipo lungo?\n\n​[Dovrebbe essere questo, non c’è alternativa.](https://joshspector.com/readers-not-subscribers/)​\n\n​\n\n## \U0001F680\_**LO STRUMENTO PIÙ SOTTOVALUTATO (MA POTENTE)**\n\nQual è lo strumento più sottovalutato ma più potente per migliorare la tua produttività, efficacia di pensiero e capacità di prendere decisioni?\n\n​[È questo e dovresti metterlo più spesso in pratica.](https://nesslabs.com/writing-thinking-tool?ref=creativerly.com)​\n\n​\n\n## **\U0001F4B8 ARRIVA IL BLACK FRIDAY**\n\nTra poco arriva il Black Friday.\n\n​[Sei alla ricerca di nuove tattiche da utilizzare per migliorare le tue vendite? Eccole qui.](https://www.thestealclub.com/blog/black-friday-special)\n\n"
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
slug: quando-non-hai-altra-scelta-utilizza-obsidian
---
Ricordo che era un pomeriggio degli ultimi giorni di luglio.

Ero su Notion, stavo pianificando i contenuti da pubblicare su LInkedin nella settimana successiva.

Poi ad un certo punto mi sono fermato.

Era appena arrivata una mail riguardo il prossimo evento Notion che Beatrice ed io avremmo organizzato a Milano e mi sono fatto una domanda.

“Ma che lo faccio a fa?”

​

**TL;DR**

*   3 mesi senza pubblicare su LinkedIn, perché l’ho fatto?

*   L’obiettivo di chi scrive (tanto);

*   Lo strumento più sottovalutato (ma potente);

*   Arriva il Black Friday.

**Il tempo di lettura previsto è**: 3 minuti e 30

​

Ora, non mi devi fraintendere.

So quanto è importante pubblicare contenuti, soprattutto per chi è un creator.

Non è la motivazione che mi era finita.

Anzi, in quel pomeriggio di luglio, mi trovavo in una serie di 3-4 mesi di pubblicazione continua su **LinkedIn**, tutti i giorni.

E quando pubblichi con tanta costanza (e disciplina), la motivazione non serve più a nulla.

Quando quella domanda è emersa, ha portato con sé tante altre domande.

Domande che non potevi più risolvere con la semplice **esecuzione**.

Quindi sono fermato dallo scrivere, per cominciare a ragionare.

E oggi scoprirai su cosa:

*   Un nuovo processo di creazione contenuti

*   Il peso delle “macerie”

*   La routine del leone

​

## **Un nuovo processo di creazione contenuti**

Quando sei perso nella creazione, spesso dimentichi di guardare le cose da lontano.

Così ti perdi un sacco di dettagli e soprattutto **non sei oggettivo**.

Uno dei motivi più importanti, per cui riuscivo a pubblicare così tanti contenuti era il fatto che avessi un **processo di creazione definito**.

Sapevo dove trovare le idee, come selezionarle, come scrivere i post, come pubblicarli e tante altre cose carine.

Era il processo migliore?

Non credo.

Funzionava?

Certo.

E lo so che in questi casi il consiglio è “se funziona, non aggiustarlo”, ma io avevo bisogno di farlo comunque.

Quindi mi sono fermato, mi sono preso il tempo per **analizzare** il mio processo di creazione contenuti e provare a **migliorarlo**.

Così ho cominciato a lavorare dietro le quinte:

*   Ho creato un mio writing hub

*   Ho dato un ruolo specifico a Notion e uno specifico a Obsidian

*   Ho capito come gestire le mie idee

*   Ho capito che tipo di sito volessi e come crearlo

*   Ho deciso di abbandonare Convertkit

Insomma, ho preso tante decisioni e ho fatto tante cose.

E non ti preoccupare, non ti parlerò di queste cose nella newsletter di oggi, c’è tempo.

Ma c’è una cosa importante da notare: ho capito in cosa migliorare, solo prendendomi del tempo per analizzare le cose.

​

## **Il peso delle “macerie”**

Questo punto è connesso al precedente.

Quando produci così tanti contenuti, hai tanti dati da dover raccogliere e da dover analizzare.

E se non hai strumenti per raccogliere con facilità, rischi di **perdere tutti questi dati**.

In fin dei conti, ogni contenuto è come una mini conversazione con chi lo legge.

E a seconda del “successo” del contenuto, puoi capire se **l’idea** alla sua base è interessante oppure no.

In pratica, dati come i commenti, i like, le interazioni e le conversazioni che nascono in DM, indicano il valore della tua idea.

Ma se sei così infognato nell’esecuzione di un processo che non hai neanche il tempo per guardarlo dall’esterno, figurati quanta attenzione puoi dare ai **risultati** di questo processo.

E così, nonostante mesi interi di post pubblicati ogni giorno, mi ritrovato senza una chiara visione dei loro **risultati**.

E senza una visione dei risultati, non puoi capire la **direzione**.

​

## **La routine del leone**

Questo è il punto forse più di impatto, quello che mi ha tranquillizzato di più.

Tranquillizzato?

Hai letto bene.

Dopo qualche settimana di pausa, **l’ansia** di perdere opportunità, connessioni e chissà cosa, cominciava a farsi sentire più forte.

Poi è arrivato il **dubbio**.

Cominciavo a pensare che questo riposo non fosse naturale, era inadatto ai tempi di oggi e ancor di più ai creator.

Ed è in questo momento che mi è tornata in mente la **routine del leone**.

Non l’ho inventata io, chiariamolo.

Non è che passo le giornate a pensare ai leoni, le passo a pensare a Notion e Obsidian.

Ma [Sahil Bloom](https://www.sahilbloom.com/newsletter/the-most-powerful-ideas) invece lo fa e l’ha spiegata in dettaglio.

In pratica, la routine dei leoni non è quella di andare a caccia ogni singolo giorno della loro vita.

Pur dovendo andare a caccia per la loro stessa sopravvivenza, si fermano, riposano e mangiano.

Anche loro hanno bisogno di recuperare le energie.

E lo stesso vale per i **creator**, dedicare il giusto tempo al riposto è tra.gli investimenti migliori che tu possa fare per continuare la tua maratona.

​

​

Ecco, direi che ti ho fatto un quadro abbastanza chiaro del perché mi sono fermato dalla pubblicazione su LinkedIn.

Per fartela breve, il riposo è un ottimo investimento.

Non importa in che modo decidi di impiegare il tempo libero che ricavi, l’importante è che ci sia lo spazio per il riposo.

Detto questo, per oggi è tutto: buona settimana e beccati le risorse.

Daniele

