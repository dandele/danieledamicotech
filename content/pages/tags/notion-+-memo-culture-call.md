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
title: "\U0001F9F0 kSC #61: Notion + Memo culture ="
colors: colors-a
date: '2023-10-29'
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
    text: "## **\U0001F465\_CHE ORA È?**\n\nUtilizzi Linkedin?\n\nTi chiedi qual è l’ora migliore per pubblicare?\n\n​[Ecco le risposte di cui hai bisogno.](https://www.linkedin.com/posts/ankitpatel96_we-analyzed-130000-linkedin-posts-here-activity-7122223992970629120-NWjm/?ck_subscriber_id=1870002162)​\n\n​\n\n## **\U0001F680 FARE CURATION NON BASTA**\n\nCerte volte, il modo migliore per essere più produttivi è quello di lasciar andare alcune cose.\n\n​[Di quali cose parlo e perché?](https://newsletter.thejorgemedina.com/p/youre-not-lacking-creativity-youre)​\n\n​\n\n## **\U0001F4B8 IL POTERE DI ALCUNE FRASI**\n\nCi sono frasi che sono più forti di altre.\n\n​[Questa è una lista di quelle che più ti possono aiutare a ottenere risultati.](https://twitter.com/Nicolascole77/status/1714099071143587913?ck_subscriber_id=1870002162)\n\n"
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
slug: notion-+-memo-culture-call
---
”Non avevo scelta”.

È una delle frasi più utilizzate dai cattivi di film, libri ecc.

Passano l’intera storia a fare le loro cose da cattivi, poi arriva la resa dei conti.

Gli eroi vincono e il cattivo la dice, quasi fosse una scusa.

Scommetto che anche tu l’hai pensata qualche volta, vero?

In tal caso, **Obsidian** ti potrebbe aiutare.

​



**TL;DR**

*   Quando non hai altra scelta…utilizza Notion!

*   Che ora è?

*   Fare curation non basta;

*   Il potere di alcune frasi.

**Il tempo di lettura previsto è**: 3 minuti e 30



​

Anche io l’ho pensata qualche volta.

E fino a qualche tempo credevo fosse tutta questione di fortuna e volontà.

Se avevi la sfortuna di trovarti in una situazione in cui non avevi scelte, dovevi avere la forza di **volontà** per fare la scelta giusta (o inventartene una nuova).

Poi però ho letto un libro e ho capito che puoi evitare le situazioni da “non ho scelta”.

E che puoi utilizzare **Obsidian** per riuscirci.

In questi tre step:

*   La condizione necessaria

*   Non unire ciò che deve restare separato

*   Il thinking template

​

## **La condizione necessaria**

Tutta questa idea di utilizzare Obsidian per pensare meglio mi è partita dalla lettura di [questo libro](https://www.amazon.it/Clear-Thinking-Turning-Ordinary-Extraordinary/dp/1529915945).

Secondo l’autore, spesso facciamo **scelte sbagliate** perché in precedenza abbiamo fatto errori di **posizionamento**.

Non parlo del posizionamento di marketing, ma più quello degli scacchi.

Prendiamo decisioni che pensiamo prive di impatto e poi scopriamo che un impatto lo avevano eccome!

E questo condiziona le nostre scelte future.

Così finiamo in una catena di cause e effetto che poi ci porta alle situazioni “Non ho una scelta”.

Per fortuna però c’è un modo per rompere sta catena.

Basta prendersi del **tempo** e utilizzarlo per **pensare con lucidità**.

Ma che c’entra Obsidian?

Obsidian è lo strumento per **prenderti il tempo e ragionare!**

**​**

## **Non unire ciò che deve restare separato**

Che intendo?

Intendo che devi scegliere uno strumento per ragionare e basta.

Deve essere scollegato da tutto il resto: niente task, niente progetti e niente contenuti.

E vedi che è una scelta importante.

Solo se fai questa separazione potrai utilizzare lo strumento scelto per pensare con lucidità.

Poi, se proprio vuoi, puoi utilizzare lo stesso strumento per ragionare e fare cose ma basta che usi due spazi diversi (tipo due vault).

Io ho scelto **Obsidian per pensare** e **Notion per fare cose**.

​

## **Il thinking template**

Una volta che ti sei preso il tempo e hai scelto lo strumento, puoi passare alla pratica.

Ma come?

Con la scrittura!

E non parlo di scrivere racconti o contenuti.

Parlo di quella scrittura che è ragionamento, quella che è fatta di **punti elenco** e che ti aiuta a **strutturare i tuoi pensieri**.

Insomma, quella che propongono [anche in Amazon](https://thehustle.co/02162021-amazon-writing/).

Ed è qui che interviene il **thinking template**.

È un template, proprio come quelli di Notion, che comprende 5 domande.

Tutte domande prese dal libro di Parrish e che ti guidano lungo il percorso di un **ragionamento** efficace.

Eccole qui:

*   Qual è il problema?

*   Quali sono le possibili soluzioni al problema?

*   Come valuti le diverse ipotesi di soluzione al problema?

*   Qual è l’ipotesi migliore?

*   Come la metterai in atto?

​

E quindi?

Quindi, la prossima volta che devi prendere una decisione (o affrontare un problema) non pensare non avere opzioni.

Prenditi del **tempo per ragionare** e apri il tuo tool for though preferito (ti consiglio Obsidian, ma può essere anche Notion o quello che vuoi) in uno **spazio riservato solo al ragionamento**.

Fai partire il **thinking template** e **rispondi alle domande**.

Vedrai che poi succedono cose.

E fidati, non ti ritroverai più spalle al muro.

Detto questo, buona settimana e **beccati le risorse**.

Daniele
