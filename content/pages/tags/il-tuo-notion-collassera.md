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
      - label: "SALVA IL TUO NOTION! \U0001F680"
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://zcal.co/notionbuilders/cust-notion-builders'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nAlla base di ogni tua iniziativa ci sono le idee.\n\nE ci sono tanti modi per generarne.\n\n​[Ecco alcuni modi insoliti per fare brainstorming.](https://longform.asmartbear.com/extreme-questions/?utm_source=ForTheInterestedNewsletter)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nHai a disposizione 4000 settimane nella tua vita, più o meno.\n\n​[Perché passarle a cercare la produttività?](https://invertedpassion.com/the-anti-productivity-manifesto/?ref=refind)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nHai creato qualcosa e ora la vuoi mettere in vendita su Product Hunt? Ottima scelta!\n\nMa pubblicare su Product Hunt e raggiungere il primo posto non è tanto semplice.\n\n​[Avrai bisogno di questi consigli per riuscirci.](https://kp.substack.com/p/3-simple-but-non-obvious-tips-to?utm_medium=email)​\n"
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
Ehi ciao 👋,

questo è il numero 37 del **Kit di Sopravvivenza per Creator**.

E oggi ti rivelerò **3 domande per capire il destino del tuo workspace su Notion**.

<br>

***

**TL;DR**

*   Il tuo Notion collasserà? 3 domande per evitare il disastro;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 24.

***

<br>

Non esiste farmaco, senza diagnosi.

È per questo che la prima cosa che io e Beatrice facciamo quando guardiamo lo spazio Notion di un cliente o prospect di [Notion Builders](https://www.notionbuilders.it/) è l’**audit**.

In pratica, facciamo un’analisi in cui cerchiamo di capire qual è lo stato attuale del workspace.

Se è messo bene o se è messo male e se rischia di **collassare**.

Ma come facciamo a capire certe cose?

Facciamo alcune domande a chi utilizza il workspace e a seconda della risposta ci facciamo un’idea.

Un’idea che di solito diventa un **numero**, ma questo è un altro discorso.

Ad ogni modo, di tutte le domande che facciamo, oggi ti svelerò le **3 più importanti**.

<br />

## **Il TUO NOTION COLLASSERÀ? 3 DOMANDE PER EVITARE IL DISASTRO**

Arriviamo subito al sodo, quali sono ste domande?

*   Sai dove finiscono le informazioni che catturi?

*   Riesci a dirci su quale progetto ti concentrerai questo mese/trimestre/anno?

*   Hai mai la sensazione che le informazioni ti sfuggano dalle mani per qualche problema?

Continua a leggere, così potrai fartele tu stesso e capire se c’è qualcosa che non va.

​

### **SAI DOVE FINISCONO LE INFORMAZIONI CHE CATTURI?**

Ok, che succede quando **salvi delle informazioni** sul tuo workspace Notion?

Sai dove finiscono?

E sai dove finiscono le informazioni che inseriscono le **persone con cui collabori**?

Perché se lo sai, bene, è una cosa positiva.

Se invece non lo sai, allora c’è qualche **problema**.

Significa che **manca un punto di raccolta unico**, nessuno sa dove inserire le informazioni e dove trovarle.

Quindi ci sono dappertutto **duplicati**, caos, stress, errori.

Che non sono proprio le cose che vorresti sulla piattaforma dove gestisci **informazioni vitali per il tuo business**, no?

​

### **RIESCI A DIRCI SU QUALE PROGETTO TI CONCENTRERAI QUESTO MESE/TRIMESTRE/ANNO?**

Ora, se la domanda precedente riguarda il modo in cui entrano le informazioni sul tuo Notion, questa invece riguarda il modo in cui le gestisci.

Le informazioni che non applichi **non sono informazioni utili**.

E quindi dovresti sempre sapere a quale **progetto** o attività possono collegarsi le informazioni che catturi.

E di conseguenza, dovresti essere in grado di capire tra tutte le attività e progetti che gestisci sul tuo Notion quali sono quelli più importanti e che ruolo hanno nella tua strategia.

Se non sei in grado di fare queste cose, allora c’è qualche problema.

Perché significa che tu e i tuoi collaboratori utilizzate lo spazio Notion **senza avere un quadro generale** e questo porta **stress e pocaconsapevolezza**.

Magari vi ritrovate a lavorare a progetti o task che non sono prioritari, magari associate informazioni ai progetti sbagliati e cose del genere.

Insomma, fate casino.

​

### **HAI MAI LA SENSAZIONE CHE LE INFORMAZIONI TI SFUGGANO DALLE MANI PER QUALCHE PROBLEMA?**

Poi c’è questa domanda, quella che qualifica l’**ansia** generata dal tuo spazio Notion.

E diciamoci la verità, l’obiettivo stesso di uno strumento come Notion è quello di darti il controllo del tuo business e quindi **ridurre l’ansia**, non aumentarla.

Se quando fai cose su Notion, ti sembra essere un bombarolo e pensi di dover fare attenzione a quello che fai perché se no **si scassa tutto**, allora c’è qualche problema.

E diciamo che questo è lo stato finale.

Di solito, quando le persone si ritrovano in questo stato hanno a disposizione una di queste opzioni: 

*   **ricominciano da capo** (ricominciando il ciclo); 

*   **cambiano strumento** (scegliendo qualcosa di più costoso);

*   chiamano me e Beatrice e **risolvono il problema**.

​

Ora, non sono te come hai risposto a queste domande.

Come ti dicevo, sono solo 3 domande di molte altre che facciamo (in modo esplicito oppure no) alle persone che fanno la prima call (gratis) con noi.

E alla fine del quiz ci sono poi dei numeri che guidano la nostra azione, ma non voglio farti spoiler sui prossimi sviluppi di Notion Builders.

L’obiettivo di questa newsletter era darti qualche strumento per **valutare la tua situazione** e mettere in atto delle **risoluzioni**.

Insomma, **prevenire prima che curare**.

Magari noti che le tue risposte alle domande che ti ho elencato non ti piacciono e decidi di risolvere, benissimo.

Se poi pensi di avere bisogno di supporto e vuoi il nostro aiuto nel capire meglio la situazione, **clicca il pulsante qui sotto**: offriamo noi.

E detto questo, per oggi è tutto: buona settimana e beccati le risorse.

Daniele
