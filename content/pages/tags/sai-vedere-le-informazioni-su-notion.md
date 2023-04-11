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
title: "\U0001F9F0 kSC #32: Notion e Obsidian..."
colors: colors-a
date: '2023-04-02'
description: PERCHÈ USARLI ENTRAMBI?
featuredImage:
  type: ImageBlock
  altText: Project thumbnail image
  caption: ''
  url: /images/Frame 14.webp
media:
  type: ImageBlock
  url: /images/Frame 14.webp
bottomSections:
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    title: E se Notion sparisse?
    text: >+
      <iframe width="100%" height="600"
      src="https://www.youtube.com/embed/RcgZ6SUtT9M" title="YouTube video
      player" frameborder="0" allow="accelerometer; autoplay; clipboard-write;
      encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen></iframe>

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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nPer costruire un'audience hai bisogno di catturare l'attenzione delle persone.\n\nE uno dei primi strumenti che hai a disposizione per riuscirci è il titolo di quello che scrivi.\n\n[Ecco alcune lezioni che ti saranno utili a riguardo.](https://twitter.com/VeryGoodCopy/status/1641069776649830400)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nFin dalla sua uscita, Cron Calendar ha ricevuto un sacco di attenzioni positive.\n\nCosì tante che persino Notion l'ha acquisito.\n\n[E sono convinto di una cosa: ora che è accessibile dal web, avrà ancora più successo!](https://cron.com/changelog?ref=creativerly.com)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nNon importa come fai monetization.\n\nScegliere il giusto princing è fondamentale e per questo devi conoscere alcune strategie.\n\n[Queste sono le più utili che ho trovato.](https://thefutur.com/content/3-ways-to-approach-pricing-for-creative-work)\n\n<br>\n"
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
slug: sai-vedere-le-informazioni-su-notion
---
Ehi ciao 👋,

questo è il numero 32 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò **perché utilizzo sia Notion che Obsidian**.

***

**TL;DR**

*   Notion e Obsidian, perché usarli entrambi?

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti.

***

Per anni ho cercato il tool perfetto, quello che mi permettesse di gestire tutto in un unico luogo.

E prima ancora di pensare che fosse **Notion**, ho pensato fosse **Roam Research**.

Mi piaceva tutto di quel tool, dall'esperienza di utilizzo fino al tipo di pensiero che cercava di indirizzare.

Poi peró ho provato per una seconda volta Notion ed è stato amore.

Ma questo non significa che oggi Notion sia l'unico tool che utilizzo, non è affatto così.

Anzi, la verità è che utilizzo **sia Notion che Obsidian**.

Ed oggi ti spiegheró perché.

<br>

## **NOTION E OBSIDIAN, PERCHÈ USARLI ENTRAMBI?**

E arriverò diretto al punto, senza troppi giri.

I motivi per cui utilizzo sia Notion che Obsidian, sono 3:

*   Voglio che alcune informazioni siano immuni al futuro;
*   Se scrivi tanto, hai bisogno di uno strumento che ti renda piacevole scrivere;
*   I professionisti non utilizzano solo un martello, utilizzano un kit.

<br>

### **INFORMAZIONI IMMUNI AL FUTURO**

Per questo punto, la questione è molto vicina alla **paranoia**.

Il fatto è che **non tutte le informazioni sono uguali**, certe informazioni voglio che siano immuni al tempo, così da accedere ad esse anche tra anni e anni.

Altre invece hanno una priorità solo momentanea.

Le pagine di diario che scrivo ogni giorno?

Voglio che queste pagine restino con me per anni.

Ma se il tool in cui sono raccolte sparisse?

In tal caso le perderei, a meno che queste non siano salvate in locale.

Ed è propio questo il primo motivo per cui utilizzo Obsidian che, a differenza di Notion, è disponibile offline e salva le informazioni in locale.

In pratica, le **informazioni sono al sicuro**.

Ma ci sono anche informazioni che devo condividere con altre persone, ci sono cose da costruire, database da sfruttare e magie da fare.

E per questo tipo di utilizzo, Notion non ha rivali: è il tool che utilizzo per gestire i miei task, tutte le informazioni personali momentanee e utili alla collaborazione.

<br>

### **SE SCRIVI TANTO, CONTA DOVE SCRIVI**

Qui emerge un po' di gusto personale.

Perché scrivere su Notion non è affatto problematico, chiariamolo.

Solo che ci sono alcune cose, quando si parla di scrittura, che **preferisco di gran lunga fare su Obsidian invece che su Notion**.

Magari è solo una mia percezione, ma scrivere su Obsidian mi rilassa e mi permette di **concentrarmi al meglio proprio sulla scrittura**.

Il mio spazio su Notion, per quanto organizzato ed efficace, integra troppe distrazioni e questo mi porterebbe di sicuro a perdere tempo.

Inoltre, Obsidian ha alcune **feature piccole e irrilevanti** che però si adattano in pieno alle mie esigenze di scrittura (ad esempio, mostra il numero di caratteri di un testo).

<br>

### **I PROFESSIONISTI NON USANO UN MARTELLO, USANO UN KIT**

Forse questo è il punto più importante.

È una cosa che ho capito qualche tempo fa e che mi ha liberato dal folle desiderio di trovare il singolo tool che potesse gestire tutte le mie esigenze.

Il fatto è che un tool di questo tipo, capace di gestire tutte le tue esigenze, **non esiste**.

E se anche Notion è il tool che più si avvicina alla cosa, questo comunque non lo rende tale.

Le esigenze delle persone cambiano nel tempo e sono fin troppo variegate per essere soddisfatte da un solo tool.

Per questo, **hai bisogno di un kit di strumenti** da utilizzare a seconda delle tue esigenze.

Proprio come faccio io con Notion e Obsidian, a seconda della mia necessità decido quale tool sia meglio utilizzare.

E con questo **approccio ibrido**, finora non ho mai beccato delusioni.

<br>

E quindi?

Questo che significa?

Che devi utilizzare Notion e Obsidian, insieme?

No, per niente.

In realtà non so questo cosa significhi, cerco solo di condividere la mia esperienza e di aiutarti a farne tesoro.

Il punto è che **i tool sono solo strumenti** e prima di scegliere quello da utilizzare, ha senso capire bene le proprie **esigenze e obiettivi**.

Solo così potrai ottenere il massimo dal tool (o dai tool) che scegli.

Proprio ieri, ho rilasciato un nuovo video YouTube che parla proprio di tool e cose interessanti.

Se ti interessa la questione, dovresti dargli uno sguardo, lo trovi qui sotto.

E direi che per oggi è tutto, buona settimana e beccati le risorse.

Daniele
