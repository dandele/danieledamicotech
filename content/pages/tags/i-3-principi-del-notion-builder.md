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
date: '2023-04-23'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nDi solito, le guide di questo tipo non mi piacciono.\n\n[Ma questa, con le dovute precisazioni riguardo il canale che preferisci ecc, mi sembra abbastanza veritiera.](https://arunimakhunteta.medium.com/how-to-reach-1000-followers-in-45-days-on-twitter-2f269983856c)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nNon esiste solo il Second Brain, esistono anche le sue evoluzioni!\n\n[E questa è una delle evoluzioni più interessanti, da usare al meglio con Obsidian.](https://reasonabledeviations.com/2022/04/18/molecular-notes-part-1/)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nCi sono tanti libri che ti aiutano a far crescere un business.\n\nSolo che è difficile capire quali possono essere utili per davvero.\n\n[Questa lista però potrebbe essere un buon inizio.](https://medium.com/@SLight20/i-read-210-books-to-learn-how-to-grow-my-business-only-these-4-actually-helped-c45650491a3f)\n\n<br>\n\n"
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
slug: i-3-principi-del-notion-builder
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

Una cosa interessante di Notion è l'**aspetto estetico**.

Non so te, ma la prima volta che ho aperto Notion, ho pensato:" Wa quanto è bellino!".

Bisogna essere sinceri, prima di qualsiasi ragionamento in termini di funzioni, produttività e quello che ti pare, la **cosa che più colpisce di Notion è il design**: semplice e pulito.

A me piace un sacco.

Ma il fatto che sia cosí carino di base, non significa che non possa essere **personalizzato** (o migliorato).

<br>

## **NOTION AESTETHIC: NON SI PARLA SOLO DI FUNZIONALITÀ**

La community di Notion è sempre attiva a fare cose.

E, tra tutti i template creati, ce ne sono alcuni che danno un po' più di peso all'aspetto estetico.

E oggi gli daremo il giusto spazio.

Negli ultimi giorni ho fatto una **ricerca approfondita** nei meandri del web, per portarti i **3 design di Notion** per me più belli (e gratis).

*   The visual journal;
*   Pastel calendar;
*   Your daily dashobard.

Eccoli qui e ora te ne parlo in dettaglio.

<br>

### **THE VISUAL JOURNAL**

![](https://global-uploads.webflow.com/5eea51a7e2d10b853f4385b9/62a493672428887f6b258f90_Theundefined20Journal.jpg)

Come ho già detto, Notion mi piace perchè è **minimal** al punto giusto, senza essere noioso.

Ma devo dire che si tratta comunque di uno strumento che, di base, non offre molto in termini visivi.

Ed è per questo che The Visual Journal mi ha colpito: migliora Notion, senza snaturarlo.

E così il **punto d'entrata di tante tue attività su Notion** (il journal) diventa una schermata vivace e molto bella, il tutto però senza esagerare.

[Lo puoi trovare a questo link!](https://notion.notion.site/The-Visual-Journal-8a5ce185f88b4899b585bfd845c1d966)

<br>

### **PASTEL CALENDAR**

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/hQD15d14NYR9ayD6sg6J8X/email)

Ok, devo riconoscere che **Pastel Calendar** non è molto adatto ai miei gusti: direi che ci sono giusto un po' **troppi colori**.

Ma al netto di questo, non posso dire che non sia di **impatto**.

In termini di funzionalità, non c'è molto da dire, tranne il fatto che hai la possibilità di aggiungere un giorno coerente con il tuo stato mentale.

Che è una cosa particolare, utile oppure no decidilo tu.

[Lo trovi a questo link.](https://www.notion.so/p-a-s-t-e-l-d-a-y-3087ee01829640ad8ff488e87dee4042)

<br>

### **YOUR DAILY DASHBOARD**

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/rJ5Q7WbTN249LDp1Ax834E/email)

Di tutti i template mostrati finora, questo è di sicuro quello più vicino al mio stile.

Sembra una schermata presa direttamente dal **mio workspace**, a dire il vero: c'è solo un po' **troppo giallo**.

È semplice, funzionale, accedi a tutto quello che serve e c'è anche una **citazione** per darti la giusta spinta.

[Lo trovi a questo link!](https://hermione-2.notion.site/hermione-2/Your-daily-dashboard-cbb588bd72b9445da9560544cf8a620b)

<br>

Ok, mettiamo subito in chiaro una cosa.

Quelli che ti ho mostrato finora sono template in cui il **tratto principale è l'aspetto estetico**, non quello funzionale o organizzativo.

Sono tutti gratis e puoi giocarci quanto vuoi, ma non posso garantirti che l'esperienza che avrai sarà al top.

Perché è difficile trovare un equilibrio tra estetica e funzionalità.

Quindi, considera questi template più come **ispirazione** che come effettive proposte di utilizzo.

L'obiettivo di questa newsletter era proprio quello di dimostrarti **fino a dove puoi spingere Notion** in termini estetici, oltre che darti un po' di **ispirazione**.

E spero di esserci riuscito.

Te che ne pensi di questi template?

Fammelo sapere rispondendo a questa e-mail.

E per il resto, direi che per oggi è tutto, buona settimana e **beccati le risorse**.

Daniele
