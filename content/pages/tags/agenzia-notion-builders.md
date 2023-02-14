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
title: "\U0001F9F0 kSC #25: Con Notion puoi creare tutto..."
colors: colors-a
backgroundImage:
  type: BackgroundImage
date: '2023-02-01'
description: Anche un'agenzia!
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nI tool di AI sono utili per chiunque voglia creare un’audience.\n\nSolo che sono così tanti.\n\n​[Per questo le selezioni di questo tipo sono utili!](https://twitter.com/heybarsee/status/1619712040041324544?s=61\\&t=WNQAFUwVXgFPIUZTU3mF0Q)\n\n\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\n\n\nC’è una cosa che ha grande impatto sulla tua produttività: il modo in cui utilizzi il tuo browser.\n\n​[E con questo tool, potrai utilizzarlo al meglio.](https://chrome.google.com/webstore/detail/omni-bookmark-history-tab/mapjgeachilmcbbokkgcbgpbakaaeehi?hl=en\\&authuser=0)\n\n​​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nOra che Gumroad è a rischio, tutti i creator cercano alternative.\n\n​[E questa potrebbe essere la più facile.](https://app.unlock.pics/landing)\n"
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
slug: agenzia-notion-builders
---
Una delle tecniche di produttività più efficaci è quella del [time-blocking](https://todoist.com/it/productivity-methods/time-blocking).

Tanti esperti di produttività ne decantano le potenzialità.

E posso confermarle, ne ho visto io stesso gli effetti.

Solo che c’è un problema.

L’ho messa in pratica con **Todoist**, non con **Notion**.

Poi ho deciso che dovevo risolvere.

***

**TL;DR**

*   Da Notion a Google Calendar, andata e ritorno;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti e 20.

***

Ehi ciao 👋,

questo è il numero 24 del **Kit di Sopravvivenza per Creator**.

Ed oggi ti racconterò **come sincronizzare il tuo Notion con il tuo Google Calendar.**



Mettiamo le cose in chiaro, in questa newsletter **non farò il confronto tra Notion e Todoist.**

Sarebbe un confronto particolare, tra due strumenti molto diversi.

Todoist è un tool specializzato per gestire i task.

Notion invece è un tool generale che ti permette di costruire quello che vuoi, anche un task manager.

Ed io non uso più Todoist da qualche anno, ma devo ammettere una cosa.

Adoravo Todoist per la possibilità di **integrazione con Google Calendar**.

E quindi, la possibilità di fare time-blocking.

Inoltre, visto che era una funzione base di Todoist, non dovevi impazzire per utilizzarla.

Con Notion, le cose sono diverse: non c’è integrazione interna con Google Calendar, **te la devi costruire tu**.

E nella newsletter di oggi, ti mostrerò proprio come fare.

​

## **DA NOTION A GOOGLE CALENDAR, ANDATA E RITORNO**

**Notion** ha l’API aperta e pubblica.

Questo significa che puoi utilizzarlo per fare richieste o richiami al codice di Notion e utilizzare le informazioni presenti sul tuo Notion all’interno di altri tool.

Lo stesso discorso vale anche all’inverso.

Questa però è una cosa che sanno fare i **developer** (o chi si studi la cosa con la giusta dose di dettaglio ed ossessione).

E chi non è un developer cosa fa? Utilizza tool come **Zapier, Make e gli altri**.

Si, a voler essere precisi Zapier e Make sono tool di automazione, ma possono essere utili anche a chi vuole fare integrazioni particolari.

Io, ad esempio, ho scelto Make.

E bastano solo tre cose per avere i **task del tuo Notion sul tuo Google Calendar (e viceversa).**

*   Un database Task Manager su Notion;

*   Uno scenario Make da Notion a Google Calendar;

*   Uno scenario Make da Google Calendar a Notion;

Prepara il tuo Notion, prepara il tuo account Make e cominciamo!

​

### **UN DATABASE TASK MANAGER SU NOTION**

Questa è la parte più semplice, la fase dei preparativi.

Per fartela breve: **hai bisogno di account su Notion, Make e Google Calendar.**

Inoltre, su Notion hai bisogno di un database Task Manager.

Cercherò di fartela breve.

Ecco come creare un task manager su Notion, semplice e in poco tempo:

*   Vai sul tuo spazio Notion;

*   Premi il tasto “/” sulla tua tastiera e comincia a scrivere “database”.

*   Seleziona la voce “database inline”.

*   Dai un nome alla tabella che compare: Task Manager;

*   Inserisci alcune proprietà in quella tabella (ricorda di inserire la proprietà Date, è fondamentale).

Ora che hai fatto tutti i passi necessari, dovresti ritrovarti con un bel database di Task Management sul tuo Notion.

Inserisci pure qualche task di prova.

Ora possiamo andare al punto successivo.

​

### UNO SCENARIO MAKE, DA NOTION A GOOGLE CALENDAR

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/3dXNmGnEHo9BorFaTam3hV)​

​

Ok, ora vai [qui](https://www.make.com/en) e, se ancora non ne hai uno, **crea un account**.

Fatto?

Bene, ora sei su Make, complimenti!

Per questo scenario avrai bisogno di due moduli: **Notion** e **Google Calendar**.

Aggiunti i moduli ed integrati i rispettivi tool, puoi passare alla creazione dell’ automazione.

Eccone le fasi:

*   Comincia aggiungendo un primo modulo, è un **modulo di Notion** e si chiama “Watch Database Items”. In pratica, **monitora il tuo database Task Manager** (quello su Notion) per ogni modifica che avviene.

*   Quando crei o aggiorni un elemento di quel database, l’automazione su Make parte e passa al **modulo successivo “Search Events”**;

*   Il modulo “Search Events” cerca eventi sul calendario di Google che gli hai specificato e li cerca con la **query che hai impostato** (la query deve coincidere con il nome dell’oggetto identificato dal modulo Notion);

*   L’informazione passa ad un router che gestisce **SE**:

    *   Se il modulo **Search non trova eventi** con lo stesso nome dell’oggetto su Notion, crea un evento sul calendario;

    *   Se il modulo **Search trova eventi** con lo stesso nome dell’oggetto su Notion, li aggiorna;

    *   Se il modulo **Search trova eventi** con lo stesso nome dell’oggetto su Notion, ma con la proprietà Archived valida, li cancella;

Lo so, sembra una cosa complessa ma non lo è.

Gioca un po’ con Make e vedrai che riuscirai a far tutto.

​

### **UNO SCENARIO MAKE DA GOOGLE CALENDAR A NOTION**

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/2chcbJXziwyFm51ZVLK6i5)​

​

Puoi fermarti anche al punto precedente, diciamoci la verità.

Tutto dipende da quanto giochi sul tuo calendar e quanto spesso sposti gli eventi.

Mettiamo caso che li sposti spesso.

In tal caso, **crea un altro scenario su Make** e chiamalo “Da GCAL a Notion”.

Fai gli stessi passi iniziali del punto precedente: aggiungi i moduli Notion e Google Calendar.

Ecco ora cosa devi fare:

*   **Crea un modulo di Google Calendar “Watch Events”**, che si comporterà proprio come il modulo “Watch Database Items” di Notion: monitora il tuo Google Calendar e non appena fai modifiche o crei cose, parte l’automazione;

*   **Poi crea il modulo di Notion “Search Objects”**, cercherà sul tuo database Task Manager oggetti con la query che hai fornito (il nome dell’evento su Google Calendar);

*   Anche in questo caso, si arriva ad un router e parte un SE:

    *   **Se Search Objects trova degli oggetti**, li aggiorna;

    *   **Se Search Objects non trova degli oggetti**, li crea;

    *   **Se Search Objects trova degli oggetti ma hanno la proprietà “cancelled”**, li aggiorna e cambia il loro titolo in “deleted” (non c’è la possibilità di eliminare direttamente un oggetto da un database).

Anche in questo caso sembra una cosa intricata, vero?

Fidati che è solo impressione, in realtà è tutto molto semplice.

E con questa mappa a grandi linee che ti ho dato, devi solo giocare un po’ con i tool ed andrai alla grande.

​

​

Devo dire una cosa però: è molto strano!

È strano scrivere delle guide di questo tipo e limitarle alla newsletter.

Per una roba del genere servirebbero dei **video, tante immagini** ecc.

Per questo, facciamo così.

Ti lascio un pulsante qui sotto, te cliccaci e arriverai [**al mio canale YouTube**.](https://www.youtube.com/@danieledamico_notionbuilder/about)​

Te iscriviti e, se raggiungo 50 iscritti, potrai vedere un primo **video-tutorial in dettaglio di tutta sta roba con gestione degli errori **(poi, chi lo sa, mini-corso su Notion per creator?)

Che ne dici?

Detto questo, penso sia tutto, buona settimana e **beccati le risorse**.

​
