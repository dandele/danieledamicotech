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
title: "\U0001F9F0 kSC #23: Gli Oscar di Product Hunt..."
colors: colors-a
backgroundImage:
  type: BackgroundImage
date: '2023-01-25'
client: Awesome client
description: sono arrivati!
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nIl mezzo migliore per creare un'audience?\n\nLe parole che utilizzi.\n\n[Ma come scegliere le parole migliori?](https://twitter.com/jspector/status/1617160237173145601)\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nSei sempre a corto di tempo libero?\n\n​[Allora dovresti trovare dei modi per crearne di più, altrimenti impazzisci.](https://radreads.co/calendar/)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nIl prezzo è una delle leve più importanti che determina le tue possibilità di vendita.\n\n​[Per questo, è importante che tu legga qui.](https://twitter.com/KateBour/status/1572931805476524034)​\n"
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
slug: notion-google-calendar
---
Il mio primo blog era su cinema e serie tv.

Ricordo che, io e gli altri autori, attendavamo con entusiasmo l'arrivo dei primi mesi dell'anno.

Cominciava la stagione dei premi e arrivava la **serata degli Oscar**.

Era un così grande evento che la seguivamo live, facendo le ore piccole e addirittura il **live blogging su Twitter**.

Ora quel blog non c'è più, la passione per quegli argomenti non si è ridotta eh, ma non posso più fare le ore piccole a parlarne su Twitter.

Ma questa newsletter è nata grazie alle **selezioni di Product Hunt.**​

E la **stagione dei premi** è arrivata anche per PH!

***

**TL;DR**

*   Gli Oscar di Product Hunt;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti e 4.

***

Ehi ciao 👋,

questo è il numero 23 del **Kit di Sopravvivenza per Creator**.

Ed oggi ti racconterò **quali prodotti vorrei vincessero i Golden Kitty Awards del 2022.**

<br />

Product of the year, Creator Economy e Produttività.

Il 2022 è stato un anno in cui ho passato tanto tempo su **Product Hunt**.

Perché per mesi ho pubblicato su Linkedin la Product Hunt Curation.

Una selezione dei prodotti più interessanti usciti nell’ultima settimana sulla piattaforma.

E lo so, è da qualche tempo che non la pubblico più.

Ma ho pensato di **rimediare**, in grande stile.

​

## **GLI OSCAR DI PRODUCT HUNT**

Le categoria dei **Golden Kitty Awards** sono tante.

E chi vota deve esprimersi su tutte le categorie, che sono tipo una 20ina.

In pratica, si tratta di una votazione che si prende **minimo 30 minuti del tuo tempo**.

Insomma, una votazione un po’ noiosa.

Ma non ti preoccupare, non parlerò di tutte le categorie in questa newsletter.

Ho scelto le 3 categorie che più erano coerenti con i temi del Kit.

*   Produttività

*   Creator economy

*   Product of the year

E quindi, non perdiamo più tempo, arriviamo ai **voti**!

​

### **PRODUTTIVITÀ**

Il 2022 è stato, ancor più del 2021 e del 2020, un anno di **remote working**.

Ed il remote working è una manna dal cielo, lo adoro e penso che se applicato bene e con le giuste persone possa fare **magie di produttività**.

Diciamoci la verità però, spesso è un casino organizzare i team.

E spesso devi puntare i piedi per terra per **definire confini** che invece il lavoro in presenza rende palesi.

C'è sempre il rischio di finire nell'area della **produttività** (lavorativa e non) che può essere **tossica**.

Per questo penso (e vorrei) che a vincere il premio in questa categoria fosse [Amie](https://www.amie.so/).

Si tratta di un calendar con qualche asso nella manica.Come [altri tool di cui ho parlato qualche tempo fa](https://danieledamico.tech/tags/sistemi-non-bastano/), ti permette di fare **consolidation**.

In pratica, ti permette di centralizzare tante tue attività in un'unica app: il calendar.

Amie, quindi, ti permette di **organizzare i tuoi eventi**, **gestire la tua lista di task**, **gestire i tuoi contatti** e **gestire le tue disponibilità**: tutto nella stessa app e senza integrazioni o casini vari.

Inoltre, ed è questo il motivo per cui dovrebbe vincere secondo me, Amie ti permette di fare tutta sta roba con **serenità** e **gioia**.

Tutto, dalla sua grafica alle micro-interazioni, ti trasmette una sensazione di serenità che non trovi in altri calendar.

Ed è per questo che spero vinca, perché la produttività non deve per forza essere tossica.

*​*

### **CREATOR ECONOMY**

Votare in questa categoria è stato difficile.

Mentre leggevo la lista dei prodotti nominati provavo sempre più terrore al notare che quasi tutti i prodotti erano riguardo gli **NFT**, il **web 3.0** o l'**AI**.

Poi però ho trovato il nome giusto: [Polywork](https://www.polywork.com/?filter_type=all).

Polywork è un prodotto che potremmo descrivere come un'**alternativa a Linkedin**.

Ma se Linkedin nasce come il social network per trovare lavoro, Polywork è il social network per trovare **opportunità di collaborazione**.

Opportunità di collaborazione tra creator, freelancer ecc.

Non c'è giorno in cui io non riceva notifiche di nuove richieste di collaborazione e considera che è un canale che non frequento affatto!

Insomma, è il **Linkedin dei creator ed è una bomba**.

L'unico problema (oppure opportunità) è che, almeno per ora, la maggior parte delle persone che la frequenta è straniera.

​

### **PRODUCT OF THE YEAR**


La categoria regina.

Se agli Oscar c'è il Miglior Film, ai Golden Kitty Awards c'è il Product of the Year.

E pensavo fosse difficile scegliere il vincitore di questa categoria, ma mi sbagliavo.

Perché c'è stato un trend che ha battuto tutti gli altri in questo 2022.

Ed un prodotto, secondo me, che lo ha rappresentato al meglio: l'intelligenza artificiale e [**ChatGPT**](https://chat.openai.com/chat).

Tutti ne parlano ovunque, quindi dirò poco su ChatGPT (che di sicuro avrai provato tu stesso), ma l'intelligenza artificiale ha sconvolto tutti e su Product Hunt ha dominato per mesi e mesi.

Ci sta, quindi, che a vincere sia un prodotto di intelligenza artificiale.

Ed ho votato il **prodotto che più ho utilizzato**.

​

Ora, non so quale prodotto vincerà, le mie sono solo speranze e opinioni.

Devo dire però che sono abbastanza convinto delle possibilità di ChatGPT nella categoria di Product of the Year.

In ogni caso, [puoi scoprire i vincitori qui.](https://www.producthunt.com/golden-kitty-awards/hall-of-fame)

E tu?

Hai votato?

**Rispondi a questa e-mail** e fammi sapere cosa hai votato dai, sono curioso!

Buona settimana e **beccati le risorse**!
