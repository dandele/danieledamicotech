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
date: '2022-12-25'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nIn tanti ne hanno parlato, senza dire qualcosa di davvero utile.\n\n​[Questa invece è la dimostrazione più pratica dell’impatto che l’AI può avere sulla produzione di contenuti](https://twitter.com/levelsio/status/1606352344404328449).\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nNon importa se sei un creator o chissà cosa.\n\nDi sicuro sarai abbonato a servizi vari.\n\n​[E questo potrebbe essere il modo migliore per non prenderne il controllo.](https://mysubscribe.app/)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nMonetizzare i contenuti.\n\nÈ la sfida più grande di un creator.\n\n​[E questa è una delle strategie che puoi utilizzare per raggiungerla](https://twitter.com/thatroblennon/status/1601646513142235136).\n"
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
13 a 1.

È il numero di persone che ha scommesso sulla vittoria di Notion contro Tana.

Qualche giorno fa ho pubblicato un sondaggio sul mio profilo Linkedin.

Uno che chiedeva alle persone quale tool avrebbe vinto in un confronto tra Notion e Tana.

E la risposta è stata palese.

Sembra che tutti siano convinti che Notion vincerebbe un confronto con Tana.

Ma è proprio così?

***

**TL;DR**

*   Ha senso confrontare Notion con Tana?

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 40.

***

Ehi ciao 👋,

questo è il numero 222 del Kit di Sopravvivenza per Creator.

Ed oggi ti racconterò quale tool vince tra Notion e Tana.

​

Il second brain.

È stata la prima cosa che ho cercato di costruire su Tana.

Ed è anche la cosa cui torno più spesso su Notion.

Perché col Second Brain riesci a dare struttura al tuo sistema di note: sai dov’è quello di cui hai bisogno, a cosa è collegato ecc.

E visto che volevo fare un confronto tra Notion e Tana, aveva senso paragonarli in un campo comune.

Fin dall’inizio però, ho notato una cosa.

​

## HA SENSO CONFRONTARE NOTION CON TANA?

È una cosa che noti fin dal primo momenti in cui accedi a Tana.

La sua esperienza di utilizzo, la UI e tutto il resto, ti ricordano tool come come Obisidian o Roam Research.

E ci sta.

Perché il concept alla base di Tana è proprio quello di trovare un punto di incontro tra Notion e Obsidian.

Si tratta dei tool che meglio rappresentano i diversi modi di gestire le note personali: quello dell’architetto e quello del botanico.

E Tana cerca di fornire agli architetti un tool botanico ed ai botanici un tool da architetti.

Insomma, cerca di andare a prendere gli utilizzatori di Notion che vorrebbero un po’ più di Obsidian e quelli di Obsidian che vorrebbero un po’ più di Notion.

Io rientro proprio in questa prima categoria: utilizzo Notion e ci vorrei un po’ più di Obisidian:

* Vorrei che Notion ti permettesse di contare i caratteri di scrittura, proprio come fa Obsidian;
* Vorrei che Notion ti permettesse di far scontrare le idee con la facilità visiva che ti garantisce Obsidian;
* Notion però è un tool diverso e spostarsi troppo verso le funzioni di Obsidian sarebbe un danno.

E lo stesso vale per Obsidian.

Per questo, Tana potrebbe avere senso.

Solo che c’è un problema.

​<br>

### IL PROBLEMA DI CONFRONTARE NOTION CON TANA
Notion è un prodotto in una fase di vita molto più avanzata rispetto a Tana.

Tana è in early access, è un bambino,

E sarebbe folle aspettarsi delle funzioni che manco Notion aveva al momento della sua uscita.

Quindi su Tana non troverai, per ora, API, integrazioni varie (come quella con Readwise) ecc.

Sono tutte cose che Notion ha implementato nel tempo e che ora Tana non ha.

Si tratta però di cose che io utilizzo tutti i giorni e che mi impediscono di concepire Tana come strumento principale.

​<br>

### IL GRANDE VANTAGGIO DI NOTION

C’è un’altra cosa che noti, fin da subito.

Almeno per me, Tana è più difficile di Notion.

Per riuscire a costruire il Second Brain su Tana ci ho messo qualche ora.

Su Notion ce ne metti al massimo una, senza ragionare troppo sul sistema in sè.

C’è da dire però che Tana, già ora e nonostante la sua tenera età, ha una community di nerd appassionati del tool che creano corsi (gratuiti) e strumenti per aiutare gli altri utenti.

Strumenti che lo stesso Tana ti fornisce fin da subito al primo accesso.

Insomma, Notion è molto più immediato, facile e veloce di Tana.

E lo era anche ai primi tempi, anche se privo delle funzioni di Tana.

Tale complessità cela però un vantaggio.

Ti permette di fare cose molto più fighe ed utili rispetto a quelle che ti permette di fare Notion.

Solo che le devi capire e per riuscirci devi studiare.

​<br>

### L’ALTRO GRANDE VANTAGGIO DI NOTION
Non so se questo sia un punto di vista personale oppure oggettivo.

C’è da considerare però che tutti quelli che ho sentito avvicinarsi a Notion mi hanno detto che il suo design è bello ed invitante.

Ed io lo confermo.

Adoro il design di Notion.

E Tana, al momento, ne è una versione più scheletrica, meno simpatica e di molto meno impatto.

​<br>​

Quindi, per concludere, questo confronto chi lo vince?

Non lo so.

Come ti ho detto, non si può mettere a confronto diretto i due tool.

Ma ti posso dire al verificarsi di quali condizioni dovresti valutare l’utilizzo di Tana:

Se ti piace l’idea di poter costruire quello che vuoi, come (e forse meglio di) Notion.
Se non hai bisogno di utilizzare integrazioni, API o altre funzioni più mature.
Se del design del tool, allo stato attuale, non ti importa per nulla.
Se vuoi mettere le mani su un tool complesso e con del potenziale fin dall’inizio.
Ed è proprio per questo che io stesso utilizzerò Tana.

80% Notion e 20% Tana.

Lo studierò, analizzerò e ci farò cose.

Ma altre cose, quelle più importanti, continuerò a farle su Notion.

Come l’ultimo template che ho creato!

Si chiama Easy Linkedin Algorithm e metterà il turbo al tuo Linkedin.

Tutti quelli che hanno acquistato Easy Content Strategy possono aggiornare il loro template e troveranno Easy Linkedin Algorithm all’interno.

Se invece non lo hai ancora acquistato, lo puoi fare con uno sconto del 50%.

Ti basta cliccare sul pulsante qui sotto.

Detto questo, per oggi è tutto, buon Natale e beccati le risorse.

Daniele