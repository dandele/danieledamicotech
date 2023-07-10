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
title: "\U0001F9F0 kSC #46: COSTRUISCI IL TUO CIRCLE OF COMPETENCE..."
colors: colors-a
date: '2023-07-09'
description: SU NOTION
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
      - label: "UN DATABASE = +365 RISORSE \U0001F4DA"
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://danieledamico.gumroad.com/l/yearly-kit-release'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nEssere un creator/avere un personal brand richiede parecchie energie.\n\n​[Ma quanto può essere di impatto sulla tua vita?](https://www.timstodz.com/how-to-use-your-personal-brand-to-generate-wealth/)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nTantissime persone indossano ormai dispositivi che misurano la loro attività fisica e salute.\n\n​[Ma se ci fossero dispositivi che misurano la tua produttività?](https://www.trypylot.com/?ck_subscriber_id=1121223563)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nI corsi sono uno dei metodi più diffusi, ad oggi, per monetizzare.\n\n​[Ma come si crea un corso?](https://creatorscience.com/online-course/)​​\n"
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
slug: costruisci-il-tuo-circle-of-competence-su-notion
---
Ehi ciao 👋,

questo è il numero 368 del **Kit di Sopravvivenza per Creator**.

E oggi ti mostrerò **come creare il tuo Circle of Competence su Notion.**

<br>

***

**TL;DR**

*   Costruisci il tuo Circle of Competence, su Notion!

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti.

***

<br>

Nel 1996 Warren Buffet scrive una lettera ai suoi investitori.

È una di quelle lettere agli investitori famose, come quelle di Bezos.

In pratica, sti grand imprenditori, si mettono ogni anno e scrivono qualcosa ai loro investitori.

​[In questa lettera](https://www.berkshirehathaway.com/letters/1996.html) però, Buffet pone le basi di un concetto: il **Circle of Competence**.

Secondo lui, e il suo amichetto Charlie Munger, è importante valutare ogni opportunità in funzione del proprio Circle of Competence.

E non conta quanto sia grande questo cerchio, quel che conta è **dove sono i suoi limiti e cosa c’è oltre**.

In pratica, fino a quando sei all’interno del tuo Circle of Competence, sei al sicuro ed è molto probabile che le opportunità che cogli abbiano **risultati positivi**.

Se però esci da quel cerchio, allora aumenta il rischio di fallimento, perché non hai competenza e ti muovi al buio.

Inoltre, devi fare in modo che col tempo questo cerchio si ingrandisca sempre di più.

Insomma, un bel casino.

Ancora di più se provi a implementarlo su Notion.

No?

​

## **COSTRUISCI IL TUO CIRCLE OF COMPETENCE, SU NOTION!**

Allora, questo framework ti aiuta a valutare le opportunità e capire se puoi portarle a risultati positivi oppure no.

Ma richiede che tu faccia una **lucida valutazione delle tue competenze**.

E come puoi riuscire a fare una cosa del genere su Notion?

Questa è una buona strada:

*   Il database Competenze

*   La vista Valutazione

*   Il passo finale

E ora ti spiego come percorrerla!

​

### **IL DATABASE COMPETENZE**

Ok, questo è il fulcro centrale di quello che costruiremo.

Serve un database che ospiti tutte le nostre **competenze** e dobbiamo pure classificarle.

Inoltre, vogliamo avere i risultati della valutazione davanti ai nostri occhi quando consideriamo una **opportunità**.

Come facciamo una cosa del genere?

*   In una pagina vuota digita / e poi seleziona l’opzione “Database - Full page”

*   A questo database dai il nome “Competence”

*   Inserisci una proprietà Select (cliccando sul + vicino al tasto blu con scritto “New”, seleziona Properties e scegli l’opzione Select)

*   Tra le opzioni della proprietà, inserisci queste tre voci: Danger Zone, Safe Zone, Explorer Zone

Il risultato dovrebbe essere una cosa del genere.

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/gw6EuN38WpyZYX9f51Z8Uu/email) |
| --------------------------------------------------------------------------------------- |

​

### **LA VISTA VALUTAZIONE**

Ok, ora che hai creato il database, bisogna creare **la vista che ci permette la valutazione**.

È con questa vista, infatti, che potremo rendere al meglio la questione di **aree di competenza che si allargano sempre di più**.

Perché mica vuoi che le tue competenze restino fisse?

Ecco come puoi fare:

*   in un’altra pagina, digita / e seleziona l’opzione “Linked view of a database”

*   nella finestra “Select data source” che si apre, seleziona il database che hai creato prima, quello chiamato Competence

*   nella nuova finestra, clicca su “New empty view”

*   seleziona l’opzione “Board”

*   alla voce “Group by” seleziona l’opzione “Zone”

Ok, ora dovresti ritrovarti davanti una cosa del genere.

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/oi8AdAPMWUNSdUauPUBVjF/email) |
| --------------------------------------------------------------------------------------- |

E puoi **spostare con facilità anche le competenze**.

Nella “Safe Zone”, ovviamente inserisci le competenze di cui sei sicuro.

Nella “Explorer Zone” inserisci quelle che stai esplorando.

Nella “Danger Zone”, invece, inserisci quelle di cui non capisci proprio niente.

E mano a mano che ti dedichi ad una nuova competenza, la sposti dalla “Danger Zone” fino alla “Safe Zone”.

​

### **IL PASSO FINALE**

Ora però diciamoci la verità.

Una semplice valutazione non è che ci può aiutare a molto.

Si tratta di un framework per valutare le opportunità in funzione delle nostre competenze.

Ed è proprio per fare questo che devi **aggiungere una nuova proprietà al database originale**.

Ti basta fare lo stesso procedimento con cui hai aggiunto la proprietà Select, solo che questa volta devi selezionare l’opzione **Relation**.

E tra le opzioni che avrai davanti, dovrai scegliere il database in cui raccogli i tuoi progetti/opportunità.

Ora puoi collegare ogni competenza ad uno specifico progetto e puoi fare l’inverso.

E sfruttando bene la proprietà Rollup, quando selezioni le competenze di cui hai bisogno per un dato progetto, dovresti poter vedere anche la zona di competenza per ognuna di queste.

E magari pure un valore medio, grazie a una formula.

​

Ok, ora però sto complicando le cose.

Il **passo finale** che finora ti ho mostrato è opzionale ed è un po’ più complesso.

Così complesso che risulta un **incubo** spiegarlo in questa newsletter.

Quindi facciamo una cosa.

​[**Iscriviti al mio canale Youtube**](https://www.youtube.com/channel/UCsF5XnLAXWNxySHjTD3HZrQ), se non lo hai già fatto, e registrerò un video in cui ti mostro come fare tutta sta roba, compresa la parte finale.

E se sei già iscritto, ma vuoi comunque vedere il video, **rispondi a questa email** e lo capirò!

Ti basta cliccare sul pulsante qui sotto per iscriverti.

Detto questo, anche per oggi è tutto, buona settimana e **beccati le risorse!**

Daniele

