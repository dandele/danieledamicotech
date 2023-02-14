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
title: "\U0001F9F0 kSC #26: Ma tu che te ne intendi di Notion..."
colors: colors-a
date: '2023-02-12'
description: DIMMI DELLE COSE
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
      - label: "FACCIAMO 4 CHIACCHIERE \U0001F680"
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nI\_**meme**\_sono uno strumento fantastico per creare un’audience.\n\nSolo che è un casino crearli, vero?\n\n​[Se hai risposto di sì, da oggi dovrai cambiare idea.](https://imgflip.com/memegenerator)\n\n\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nUn tempo, qualcuno mi ha detto che non puoi migliorare quello che non riesci a misurare.\n\n​[Per questo, quando ho scoperto questo tool me ne sono innamorato.](https://rize.io/)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nUtilizzi\_**Gmail**?\n\nÈ molto probabile che la risposta sia si.\n\n​[Ed è per questo che questo tool ti piacerà: possibilità di monetizzare, direttamente dal tuo account Gmail.](https://www.gmass.co/)​\n"
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
slug: te-ne-intendi-di-notion
---
Non faccio il **commerciale di Notion**.

Ho fatto application per diventare **ambassador**, ma mi devono ancora far sapere.

Però devo essere sincero, spesso mi capita di consigliare l’utilizzo di Notion alle persone.

E se leggi questa newsletter, è probabile che l’abbia consigliato anche a te.

Forse pure più di una volta.

***

**TL;DR**

*   Ma tu che te ne intendi di Notion...

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti.

***

Ehi ciao 👋,

questo è il numero 26 del **Kit di Sopravvivenza per Creator**.

Ed oggi risponderò **alle** **tre domande che mi fanno più spesso riguardo Notion.**



È una cosa che capita.

Quando hai un’agenzia che si chiama [**Notion Builders**](https://www.notionbuilders.it/), capita spesso che le persone ti chiedano cose su **Notion**.

Non sono sempre cose tecniche e divertentI, eh.

Non è che tutti ti chiedano, per esempio, di creare automazioni per l’invio di e-mail e la creazione di cartelle su Google Drive dopo una determinata azione su Notion.

Quando capitano certe domande, capisci che è una giornata buona e ti divertirai.

Poi ci sono altri giorni in cui ti chiedono altro.

E non accade solo con prospect o clienti, accade anche con persone che leggono quello che scrivo e quindi chiedono.

Ci sta.

​

## **MA TU CHE TE NE INTENDI DI NOTION…**

La cosa interessante però è che **alcune domande sono fisse**, si ripetono.

Io, così come la mia socia Beatrice, ce le sentiamo fare almeno una volta a settimana.

Ecco le 3 più gettonate.

*   Ma Notion come gestisce la sicurezza dati?

*   Il mio team utilizza già tool X, possiamo utilizzarlo insieme a Notion?

*   Possiamo usare Notion come un Crm/Task manager/Knowledge base/Sito web ?

E visto che sono così frequenti, ho deciso di non considerarle come delle domande ovvie.

Ho deciso di dartene la **risposta**.

​

### **MA NOTION COME GESTISCE LA SICUREZZA DEI DATI?**

Ok, questa sembra essere una grossa **preoccupazione** per tante persone.

In tanti ci chiediamo **cosa faccia Notion dei nostri dati**.

Ed è un dubbio lecito, eh.

Quando stai pensando di utilizzare Notion per gestire tutto il tuo business, ci sta che tu abbia dubbi del genere.

Anche io, qualche tempo fa, mi feci la stessa domanda.

Poi però ho fatto qualche ricerca online e non mi sono preoccupato più.

Si, perché quelli di Notion la **fissa per la sicurezza dei dati** ce l’hanno da un bel po’.

E quindi hanno raccolto un bel po’ di certificazioni, [la più recente è la ISO 27001](https://www.notion.so/blog/were-iso-27001-compliant-heres-what-that-means-for-you).

Attesta che i **sistemi informativi utilizzati da Notion siano sicuri e riservati**.

In pratica, i tuoi dati sono al sicuro e restano segreti: sia che si tratti della tua lista della spesa che degli indirizzi e-mail dei tuoi clienti.

​

### **IL MIO TEAM USA GIÀ QUESTO TOOL, POSSIAMO USARLO INSIEME A NOTION?**

Quando ci fanno una domanda del genere io mi **emoziono**.

Perché nasconde **esigenze particolari**, quel tipo di esigenze che mi piace risolvere.

La risposta è facile.

Notion è integrabile con **qualsiasi strumento tu stia utilizzando**.

Tra integrazioni già presenti su Notion, giochetti vari con Zapier/Make e utilizzo dell’API aperta è sicuro che qualche soluzione ci sia.

Per esempio, molti ci dicono di utilizzare **Trello** e noi gli diciamo che quello che ti permette di fare Trello, lo puoi fare anche su Notion.

Certo, **Trello è più semplice da utilizzare**, su questo non c’è dubbio.

Ma su Notion, oltre che poter giocare con le kanban board, puoi giocare con tante altre cose.

Il solo problema è la capacità di costruzione, [ma per quello ci siamo noi](https://zcal.co/notionbuilders/quick-talk).

​

### **MA SI PUÒ USARE NOTION COME CRM/TASK MANAGER/KNOWLEDGE BASE/SITO WEB?**

Questa domanda è l’estensione naturale della precedente.

La notizia che Notion è così flessibile colpisce le persone come una **folgorazione**.

Vedi la loro espressione mutare, come se fossero sulla strada di Damasco e avessero appena ricevuto un altro tipo di rivelazione.

E quindi subito vogliono scendere nei **dettagli**.

“Ma si può usare come task manager?”.

“Io ci vorrei fare un CRM”.

“Mi piacerebbe utilizzarlo come sito web”.

Hai capito la storia, dai.

E indovina la riposta?

**Si**, a tutte queste domande e tutte le altre che puoi immaginare.

I **limiti tecnici dello strumento sono pochi** e spesso si possono aggirare grazie a determinate competenze.

Il grande vantaggio di Notion è che puoi utilizzarlo per **cucire il tool più adatto alle tue esigenze.**

Non dovrai più utilizzare una soluzione standardizzata e fatta senza tenere conto delle tue esigenze più particolari.

Tutti preferiscono un **vestito cucito su misura**, no?

​

​

Bene, direi che oggi ho fatto una cosa molto utile.

Ora avrò qualcosa da girare a tutte le persone che mi faranno questa domanda in futuro.

Sono convinto che ce ne saranno sempre più.

Ma a parte questa **strategica pigrizia**, spero di aver chiarito dei dubbi anche in te che con tanta pazienza hai letto fin qui.

Ma se hai altre domande sulla questione, non esitare a rispondere a questa e-mail.

Oppure **facciamo una call**, senza impegno, ti lascio il **pulsante qui sotto**.

E direi che per oggi è tutto, buona settimana e **beccati le risorse**.

