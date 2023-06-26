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
title: "\U0001F9F0 kSC #44: 3 TATTICHE PER LA SETTIMANA PERFETTA…"
colors: colors-a
date: '2023-06-18'
description: su notion
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nEsiste un modo per unire la\_**potenza dello storytelling con la brevità dei post social**?\n\n​[Si e questa è la guida definitiva su come metterlo in pratica.](https://www.worldbuilders.ai/p/micro-storytelling)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nHai presente quel problema?\n\nQuello dei\_**meeting**.\n\nQuello per cui ogni volta che hai una call, dovresti prendere appunti ma poi o non lo fai, oppure li prendi e poi li perdi?\n\n​[Ecco, questa potrebbe essere la soluzione migliore.](https://fireflies.ai/)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nCome capire se una\_**nicchia**\_può portarti alla monetization oppure no?\n\n​[Leggi questo e replica per la nicchia a cui stai puntando.](https://www.ramoswriter.com/rising-finance-phenomenon/)​\n"
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
slug: 3-tattiche-per-la-settimana-perfetta-su-notion
---
Ehi ciao 👋,

questo è il numero 371 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò di **3 tattiche per progettare la tua settimana perfetta, su Notion!**

<br>

***

**TL;DR**

*   3 sistemi da usare su Notion per sconvolgerti la vita

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti.

***

<br>

Ho già parlato dell'importanza di **ragionare sulla tua settimana**.

E qualche mese fa, ho parlato di come analizzare la settimana passata ma non di come organizzare quella futura.

E soprattutto, non ti ho mai detto come **riuscire a farlo con Notion**.

Quindi, in occasione di alcune modifiche che ho fatto al mio processo di **weekly planning**, ho deciso di rimediare.

​

## **3 CONSIGLI PER PROGETTARE LA TUA SETTIMANA PERFETTA, SU NOTION!**

Fino a qualche settimana fa, ogni lunedì mattina, dedicavo i primi 60 minuti della giornata (circa) alla review della settimana precedente e alla pianificazione di quella che cominciava.

Poi però, per tutta una serie di motivi, mi sono fermato.

Così, per un paio di mesi, sono andato avanti a braccio.

Avevo il piano nella mia testa e giorno dopo giorno decidevo le cose da fare più importanti, ma non è una soluzione sostenibile.

Perché così **aumenta lo stress**, non hai mai il controllo generale della situazione ecc.

Ora però ho risolto la cosa, con queste **3 modifiche**:

*   Struttura > Caos

*   Day theming

*   Daily ed evening reflection

E oggi ti svelerò come metterle in pratica su Notion e progettare la tua settimana perfetta!



​

### **STRUTTURA > CAOS**

Questa è una cosa che ho dovuto capire con l'esperienza.

Qualche mese fa, quando ho provato per la prima volta a pianificare la settimana su Notion, ho fatto un grande errore.

Ho cominciato a **pianificare**, senza una particolare struttura.

Mi dicevo che l'importante era restare semplici e quindi questa fase di pianificazione era scollegata dalle aree di esecuzione di task, project management e lavoro.

In pratica, facevo delle semplici liste con le cose da fare e quando farle.

Ma dove finivano i progressi verso i miei obiettivi?

Dove finivano i risultati ottenuti nella settimana precedente?

E i task che magari avevo dimenticato?

Erano su Notion, lo so, ma non li avevo a disposizione nella fase di weekly planning.

E questo la rendeva inutile.

Ora invece, ho cambiato le cose.

Ora, quando avvio la fase di planning, ho **accesso a viste di diversi database**: task, progetti, note.

E tutto mi è più chiaro, vedo il quadro generale e posso pianificare al meglio!



​

### **DAY THEMING**

Altra cosa importante.

Mi piace il **time-blocking** e mi piace anche l'idea di associare ogni mia giornata ad un **tema**.

Unendo le due cose, infatti, posso associare con facilità i task al giorno che gli spetta, senza indecisioni strane.

Ad esempio, il lunedì lo dedico ai task del progetto X, quindi ogni lunedì so che devo fare certe cose.

Solo che c'è un problema.

Questo esempio, è basato sui progetti e non sul tipo di attività.

E che significa?

Che se hai diversi progetti, quindi il lunedì lavori al progetto X, il martedì al progetto Y e così via, potrebbe passare una settimana tra gli avanzamenti in un dato progetto.

E in alcuni casi, è troppo tempo.

Quindi ho cambiato le cose.

Ora i **temi delle giornate** riflettono il **tipo di attività**.

Ecco un esempio:

*   lunedì: content creation e marketing;

*   martedì: email, amministrazione e linkedin engagement;

*   mercoledì: costruzione su Notion e automazioni;

*   giovedì: costruzione su Notion e automazioni;

*   venerdì: buffer.

E come implemento sta roba su Notion?

Ogni giorno, in automatico, sul mio Notion viene creata una pagina relativa alla giornata.

E per quella giornata, io seleziono il relativo tema, tramite proprietà "select" del database in cui la pagina è creata.

Semplice ma funzionale.



​

### **DAILY ED EVENING REFLECTION!**

Altra cosa che prima facevo poco e male.

Prima ero solito fare solo una piccola riflessione mattutina, in cui facevo un po' di journaling e decidevo cosa fare nella giornata.

Questa però era scollegata dalla fase di progettazione della settimana.

E le **giornate non finivano mai per davvero**.

Perché non avevo una fase, a fine giornata, in cui dicevo anche al mio sistema che la giornata era finita.

Ora invece, ho creato un piccolo rituale che mi aiuta.

A **fine giornata**, torno sulla pagina della giornata e faccio alcune cose:

*   metto la spunta a tutti i task che ho fatto;

*   sposto la data dei task che non ho fatto;

*   elimino i task che non ho fatto e che penso non siano più importanti;

*   faccio journaling serale.

In questo modo, quando poi arriva la fase di planning della settimana successiva, ho più informazioni su cui posso operare.

Ho una vista d'insieme molto più coerente e precisa.

E questo è un grande vantaggio.

​

Ora, in realtà te puoi mettere in pratica queste cose anche su altri tool.

Non devi per forza farlo su Notion, puoi anche scegliere Obsidian, carta e penna, Apple Notes.

Insomma, puoi farlo dove ti pare.

L'importante però, è che tu introduca una pratica del genere nella tua vita.

E queste modifiche di cui ti ho parlato oggi, potrebbero aiutarti a costruire al meglio il **processo di weekly planning perfetto**!

E niente, direi che per oggi è tutto, buona settimana e beccati le risorse.

Daniele
