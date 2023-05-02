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
title: "\U0001F9F0 kSC #35: I 3 PRINCIPI…"
colors: colors-a
backgroundImage:
  type: BackgroundImage
  url: /images/bg2.jpg
date: '2023-04-23'
client: Awesome client
description: DEL NOTION BUILDER
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nE per la serie “non credo a queste guide, ma questa mi sembra sia interessante”, ecco un nuovo episodio.\n\n​[Questa volta si parla di newsletter e come farle crescere.](https://the-soulful-entrepreneur.beehiiv.com/p/8-simple-steps-grow-newsletter-50000-subscribers?utm_source=the-soulful-entrepreneur.beehiiv.com\\&utm_medium=newsletter\\&utm_campaign=8-simple-steps-to-grow-your-newsletter-to-50-000-subscribers)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nOk, Notion Builders non è una startup ma una piccola agenzia con solo due persone.\n\n​[Però sta guida sul lavoro asincrono può essere utile a noi, così come a tante altre realtà che vogliono diventare più produttive.](https://review.firstround.com/the-secret-to-an-in-sync-startup-ditch-your-meetings-and-try-an-asynchronous-culture?ref=refind)​\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nI creator producono contenuti e cercano di monetizzarli.\n\n​[E anche in questo caso, la guida è per le startup ma penso che tutti possano trovarla utile: soprattutto chi vuole imparare a convertire l’attenzione in denaro.](https://www.animalz.co/blog/bottom-of-the-funnel-thought-leadership/)​\n\n<br>\n\n"
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
    text: >+
      <Script async data-uid="a9380e8603"
      src="https://kit-sopravvivenza-creator.ck.page/a9380e8603/index.js" />


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
slug: a-scuola-di-produttivita-da-cal-newport
---
Ehi ciao 👋,

questo è il numero 35 del **Kit di Sopravvivenza per Creator**.

E oggi ti svelerò I **3 principi del Notion Builder.**

<br>

***

**TL;DR**

*   I 3 principi del Notion Builder;

*   Una risorsa per la tua audience building;

*   Una risorsa per la tua produttività;

*   Una risorsa per la tua monetization.

**Il tempo di lettura previsto è:** 4 minuti e 30.

***

Quando penso ai creatori di Notion, non so come giudicarli: **se eroi della produttività oppure truffatori.**

Hanno creato uno strumento molto potente ma che non spaventa.

Uno che attira gli utenti con la facciata di semplicità e che invece nasconde una grande dose di complessità.

Database, relazioni, rollup, formule, buttons, api ecc: il delirio.

E tutto sto **delirio è nascosto,** si mostra solo a chi vuole portare Notion al suo massimo potenziale: i builder.

Tutte quelle persone che vogliono poter costruire cose con Notion, creare sistemi con cui gestire al meglio la propria vita, azienda o che ne so.

Ed io e Beatrice siamo builder, per questo abbiamo creato [un’agenzia che porta questo nome](https://www.notionbuilders.it/).

Ma quali sono i **principi** che, secondo me, un builder dovrebbe rispettare fin dal primo momento in cui apre Notion?

<br>

## **I 3 PRINCIPI DEL NOTION BUILDER**

È un problema che sono convinto avrai incontrato anche tu: **Notion è un foglio bianco su cui puoi scrivere quello che ti pare**.

E più impari a scrivere, più ti ritrovi a scriverne di complesse oppure ti paralizzi perché non sai cosa scrivere.

Ma sono convinto che ci sia un modo per evitare questa trappola, tre principi da rispettare per diventare un grande builder fin dall’inizio.

Eccoli: 

*   svolgerai tutto il tuo lavoro lontano dal master; 

*   non tratterai il tuo workspace come un archivio; 

*   non tratterai il sistema di altri come il sistema tuo.

Continua a leggere, te li spiego in dettaglio.

<br>

### **SVOLGERAI IL TUO LAVORO LONTANO DAL MASTER**

Ok, su Notion esistono i database.

Non è la prima volta che li cito e sono sicuro che li avrai notati anche sul tuo workspace.

I database sono l’arma segreta di Notion e posso dire con certezza che **quasi tutte le pagine del tuo Notion dovrebbero essere parte di un database**.

Sti database sono importanti per tanti motivi, in particolare però ti permettono di **collegare le informazioni contenute nel tuo Notion**.

E collegandole: 

*   ti assicurerai di poterle gestire al meglio, anche in futuro; 

*   ti assicurerai la loro validità nel tempo; 

*   ti assicurerai la possibilità di spostarle al meglio (esportare pagine, inviarle ecc.).

Ma c’è una cosa che devi ricordarti quando usi i database: **non lavorare sul database originale**.

Quando crei un database, puoi crearlo sia “Inline” che in versione “Full page”.

Nel caso in cui scegli la seconda opzione, vedrai quella che sembra una **pagina classica di Notion**, solo che al suo interno c’è solo il database e non puoi creare altro.

Questa pagina è in realtà la **radice del database** ed è anche chiamata Master.

E per lavorare su questo database, non devi per forza accedere alla radice, anzi è sconsigliato.

È meglio creare delle **viste del database originale** e adattare quelle viste alle tue esigenze.

In questo modo, ti assicuri che le informazioni originali restino al sicuro e tu puoi accedere ad esse come vuoi e dove vuoi.

Il master è la fonte delle informazioni, fai di tutto per non sporcare la fonte.

​<br>

### **NON TRATTERAI IL TUO WORKSPACE COME UN ARCHIVIO!**

Ok, ora che (spero) hai capito l’importanza dei database, qual è il prossimo passo?

Quello di cominciare a **giocare con le informazioni e con i database**,comincerai a crearne tanti e dargli la struttura che preferisci.

Poi comincerai a metterli in relazione tra loro, con le loro visualizzazioni e in poco tempo ti ritroverai con tante cose sul tuo workspace.

E questo sarà il momento in cui dovrai capire una cosa: **il tuo workspace è un sistema, non un archivio.**

Che differenza c’è?

Un archivio è un raccoglitore di informazioni **statico**, un sistema invece è **dinamico**.

In un archivio puoi scaricare tutto quello che vuoi, abbandonarlo a prendere polvere e chissene.

Un sistema invece è dinamico, cresce con te e si adatta al modo in cui lo utilizzi.

Ti faccio un esempio.

Cominci ad utilizzare Notion e col tempo realizzi che vuoi una dashboard generale, nella tua home page, che mostra tutte le informazioni rilevanti giorno dopo giorno: crei le viste dei diversi database e il gioco è fatto.

Poi però passa il tempo e le tue esigenze cambiano, quindi cambi anche l’homepage, i collegamenti tra database ecc.

E è così adatti il workspace alle tue esigenze, lo tratti come un sistema, non come un archivio.

​<br>

### **NON TRATTERAI IL SISTEMA DI ALTRI, COME IL SISTEMA TUO**

Quanti template di Notion esistono?

Migliaia, anche io ne vendo alcuni.

Ma cosa sono i template e perché hanno cosí successo?

Perché sono soluzioni personali a problemi comuni.

E hanno cosi tanto successo perché ti danno la **percezione di un sistema** (di un’organizzazione strutturata delle informazioni), senza la **difficoltà di crearlo**.

Solo che ti devi ricordare il principio numero due: il tuo workspace è un sistema e dipende dalle tue esigenze, non da quelle di altri.

Utilizzare il mio workspace ti sarebbe poco utile, perché è costruito intorno alle mie esigenze non alle tue.

Ed è per questo che, quando parlo con chi ha acquistato i miei template gli dico sempre una cosa:”questo è il punto di partenza, sentiti libero di modificarlo e adattarlo alle tue esigenze”.

Stesso discorso vale per framework, filosofie di produttività ecc.

Sono tutte cose che ti possono fare da guida e scorciatoia, ma alla fine della giornata sei tu a dover utilizzare il sistema e questo deve riflettere le tue esigenze.

​

Ecco, direi che per oggi è tutto.

Buona settimana e beccati le risorse!

Daniele
