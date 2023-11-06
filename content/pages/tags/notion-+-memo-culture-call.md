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
date: '2023-11-05'
description: '- Call'
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
“Bella idea, Dani, facciamo una call!”

È una delle frasi che la mia socia Beatrice pronuncia più spesso, anzi no, pronunciava.

Perché parlo al passato? Cos’è successo?

Niente di che, non ti preoccupare.

Solo che Beatrice non dice più quella frase, abbiamo preso una decisione.

In Notion Builders non ci sono più call inutili, in Notion Builders c’è una memo culture.

Ed è con Notion che l’applichiamo.

​

TL;DR

Notion + Memo Culture = - Call
Il ROI dei fallimenti;
È sempre un problema di priorità;
Quanti soldi sono abbastanza soldi?
Il tempo di lettura previsto è: 4 minuti

​

Ok, facciamo le cose con calma.

La memo culture si ha quando un’azienda preferisce la comunicazione scritta a quella orale.

E non parlo per forza di e-mail, parlo soprattutto di di documenti, memo, cose che richiedono una scrittura dettagliata e lettura concentrata.

Lo scopo di avere una cultura simile è favorire le decisioni strategiche perché la scrittura aiuta il pensiero, come accennavo qui.

E devo dire la verità, mi è sempre sembrato difficile implementare una cultura del genere.

Poi ho realizzato che Notion poteva risolvere le difficoltà da me ipotizzate e abbiamo portato la memo culture in Notion Builders.

Abbiamo seguito queste 3 regole:

Ti devi sedere (ma non per forza) e devi scrivere, tanto
Devi gestire l’archivio di quello che scrivi
Dopo aver scritto, devi agire
Ed ora te le spiego meglio.

​

Ti devi sedere (ma non per forza) e devi scrivere, tanto
Ok, c’è una cosa a cui proprio non puoi rinunciare: la scrittura.

Devi scrivere, tanto.

Chiariamo, puoi farlo dove vuoi e come vuoi: su carta e penna, in piedi oppure su tool diversi da Notion.

Non conta il modo, conta il cosa.

E per capire il cosa, ti basta fermarti qualche secondo prima di prendere una decisione.

Ti fermi, apri il tuo laptop e cominci a scrivere.

So che può sembrare una sfida difficile, ma qui puoi leggere qualche trucchetto per facilitarla.

Ti basta applicare quelle domande alla tua decisione ed il gioco è fatto.

Inizierai a ragionare in modo lucido e così scriverai il documento di cui hai bisogno.

Tutto qui.

Devi solo scrivere, non importa il come, importa solo il cosa.

Io, per esempio, scrivo la prima bozza di documenti su Obsidian (che preferisco a Notion per esperienza di scrittura) e quando è pronta alla condivisione, la passo su Notion.

​

Devi gestire l’archivio di quello che scrivi
Quando il documento arriva su Notion, comincia il suo viaggio.

Nel momento in cui lo condividi, quel documento diventa una risorsa con un grande valore.

Devi dare una casa stabile a quel documento e devi fare in modo che qualcuno lo legga.

È qui che entra in gioco Notion e la Document’s Inbox che abbiamo creato.

​

​

Si tratta di una dashboard Notion in cui, sfruttando le assegnazioni di un documento, io e Beatrice possiamo vedere con facilità quali sono i documenti che dobbiamo visionare.

Guarda l’immagine qui sopra, nella colonna di sinistra ci sono i documenti che devo rivedere io e che Beatrice ha scritto nei giorni precedenti.

Nella colonna di destra ci dovrebbero essere i documenti che ho scritto io e che Beatrice deve rivedere.

Ma Beatrice è molto precisa e come puoi vedere li ha già letti tutti.

Li ha letti, ha commentato, poi ha messo un tag ed i documenti sono spariti.

Tutto visibile a me, tutto visibile a lei (in modo speculare).

Tutto nella stessa schermata.

Tutto recuperabile, sempre.

Una casa sicura per le nostre decisioni.

​

Dopo aver scritto, devi agire
Ok, scrivi un documento, lo condividi, lo gestisci e poi che succede?

Finisce tutto lì?

Per niente, quello che hai scritto deve diventare oggetto di discussione e magari di azione.

Ma come?

Con la creazione di task all’interno del documento!

Puoi creare un semplice template che gestisce i documenti e al suo interno puoi inserire queste cose qui:

le domande per farti ragionare;
un accesso al database dei task;
un accesso al database dei progetti.
In questo modo, dopo qualche commento, tu e il tuo team potete prendere decisioni e poi potete passare all’azione assegnando task e progetti rilevanti.

​

Fidati, avere una memo culture porta parecchi vantaggi.

In fondo, credo ci sia un motivo se aziende come Amazon, Notion e tante altre, adottano questo tipo di cultura.

Come al solito se vuoi una guida più precisa su come usare Notion per la memo culture nella tua azienda, basta che rispondi a questa email e chiedi.

Detto questo, per oggi è tutto, buona settimana e beccati le risorse.

Daniele

​

👥 IL ROI DEI FALLIMENTI
Come puoi trasformare un format di poco successo in uno di successo?

​Cambiando le metriche con cui lo analizzi.​

​

🚀 È SEMPRE UN PROBLEMA DI PRIORITÀ
Gran parte dei problemi di produttività dipende dal fallimento di determinare le priorità o di perseguirle.

​Ecco un modo per risolvere il primo caso.​

​

💸 QUANTI SOLDI SONO ABBASTANZA SOLDI?
​Certe volte, tutto quello che conta è la prospettiva.

