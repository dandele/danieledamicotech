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
title: "\U0001F9F0 kSC #28: Meeting notes efficaci"
colors: colors-a
date: '2023-03-13'
description: Grazie a 3 libri
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nScrivi bene e penserai bene.\n\nScrivere ti aiuta a creare un'audience ma anche a pensare al meglio.\n\n[Solo che devi saper scrivere e questa risorsa ti può aiutare.](https://blog.stephsmith.io/learning-to-write-with-confidence/)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nLa produttività è fatta dalle abitudini che adotti.\n\nEsiste un'abitudine più importante di tutte?\n\n[Dipende dai punti di vista, questa però potrebbe essere un'abitudine interessante.](https://www.sahilbloom.com/newsletter/the-single-greatest-habit-you-can-build)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nOk, hai creato qualcosa e la vuoi vendere, bene!\n\nMa come fai a sapere che risultati avrà?\n\nCome fai a sapere che risultati avrà, prima ancora di crearla?\n\n[Magari qui puoi trovare un aiuto.](https://fortelabs.com/blog/how-i-used-amazon-reviews-to-predict-sales-of-my-book/)\n"
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
slug: meeting-notes-efficaci
---
Ehi ciao 👋,

questo è il numero 292 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò di **3 libri che mi hanno aiutato a passare da creator ad agenzia**.

***

**TL;DR**

*   Da creator a Notion Builders: 3 libri per la trasformazione;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 40.

***

La questione di oggi è semplice.

La questione è che leggo parecchio, fin da quando ero piccolo.

I **libri** mi hanno accompagnato in tutte le fasi della mia vita: hanno plasmato il mio modo di pensare e anche i miei obiettivi.

In realtà, credo che la cosa non valga solo per me, valga un po' per tutti i lettori.

Ad ogni modo, sono tanti i libri che hanno influenzato il mio modo di pensare.

Ma ce ne sono 3, in particolare, che mi hanno portato ad **abbandonare la strada del creator per prendere quella dell'agenzia**.

E oggi voglio parlartene.

<br>

## **DA CREATOR A NOTION BUILDERS: 3 LIBRI PER LA TRASFORMAZIONE**

Come al solito, arriviamo subito al sodo.

Ecco i 3 libri di cui parlo:

1.  Il libro che mi ha fatto capire la verità sulla mia strada: The Pathless Path;

2.  Il libro che mi ha fatto capire la giusta grandezza: Company Of One;

3.  Il libro che mi ha fatto capire le giuste parole: Radical Candor.

In che modo mi hanno aiutato?

In che modo mi hanno fatto cambiare idea e mi hanno portato sulla strada su cui mi trovo?

Insomma, quali sono le lezioni che mi sono portato a casa, dopo aver letto questi libri?

<br>

### **The Pathless Path**

[Questo libro](https://amzn.to/3ESlA3E) è un manifesto.

È più **self-help** che business, infatti al suo interno non troverai molti consigli su cosa fare o come farlo.

Leggendolo però avrai l'opportunità di **riflettere**, riflettere tanto.

In particolare, comincerai a riflettere sulla tua vita lavorativa e non.

Ansia eh? Ci sta.

Sembra strano ma la maggior parte delle persone si butta in un percorso lavorativo senza aver pensato bene a **cosa vuole dalla vita**.

Certo, molto spesso ci sono le condizioni a dettare certe scelte, ma se non si sa bene cosa vogliamo dalla vita, non potremo mai ottenerlo.

E questo è proprio un libro che ti aiuta a capire sta roba.

Per fartela breve, arriva un momento nella vita in cui ognuno di noi deve decidere tra **due opzioni**:

*   **la via normale**: la vita "automatica", quella in cui facciamo tutto quello che serve per diventare di **successo**, mettiamo al primo posto il lavoro e la sicurezza che ne deriva.

*   **la via senza via**: questa è la strada che segue chi non si trova bene sulla strada già tracciata da altri, preferisce correre dei **rischi** e mettere al primo posto la **vita che desidera**.

Nessuna delle due strade è preferibile all'altra, tutto dipende da chi prende la scelta.

Ma dopo aver passato qualche anno nel primo sentiero, proprio la lettura di questo libro mi ha permesso di capire al meglio la mia volontà di **cambiare strada**.

Fare il grande salto, avviare qualcosa di mio, ci siamo capiti no?

<br>

### **Company Of One**

E una volta aver deciso quale strada prendere, cosa dovevo fare?

Ho risposto a questa domanda grazie a [questo libro](https://amzn.to/3Zwms63).

È un libro scritto da Paul Jarvis e parte da un **concetto fondamentale**: la parola che meglio descrive tanti dei business di oggi è la parola "più".

Bisogna fare più soldi, per fare più soldi servono più clienti, per soddisfare più clienti servono più persone, per assumere più persone servono più soldi e via col loop.

Jarvis però mette in dubbio una cosa, una all'origine: perché il di "più"?

Di quanti soldi puoi mai aver bisogno per mandare avanti una tua attività?

Insomma, applica il **minimalismo** al business.

E poi propone tutta una serie di idee per non farsi prendere dalla trappola del "devo fare di più" nel momento in cui si avvia un proprio percorso imprenditoriale.

Eccone alcune:

*   Per avere successo, non puntare sempre a qualcosa in più, metti dei **limiti di profitto**;

*   Il tuo obiettivo dovrebbe essere quello di raggiungere un'audience specifica, più di **nicchia** è e meglio è;

*   Evita di fare grossi investimenti prima (sia temporali che economici), punta a fare **piccole scommesse** con piccoli rischi.

Sto libro è uno spettacolo, ti fa pensare tanto e ti fa capire ancora di più.

<br>

### **Radical Candor**

Ok, questa è un'altra bomba.

Questo è un [libro](https://amzn.to/3ZfUGuU) indirizzato ai leader d'impresa che vogliono riuscire a comunicare al meglio con i propri colleghi e dipendenti.

In realtà, penso che non sia utile solo ai leader, ma che sia utile un po' a tutti: compresi i membri di un'agenzia appena nata come [Notion Builders](https://www.notionbuilders.it/).

L'idea è quella che, per ottenere il meglio da una collaborazione, bisogna investire tanto sulla **comunicazione**.

E ci sono tutta una serie di piccole regole e consigli che permettono alle persone di uscire dalla trappola del "devo essere sincero o omettere?".

Eccone alcune:

*   Quando vai a lavoro, lasciati **coinvolgere totalmente dai tuoi colleghi**;

*   Sii **trasparente** e aperto a tutti.

Insomma, è una bomba e te lo consiglio.

Ecco, come potrai intuire dal mio breve resoconto di questi libri, ognuno di questi mi ha insegnato qualcosa.

E con queste lezioni, posso lanciarmi nell'avventura imprenditoriale che è Notion Builders: sicuro di essere sulla mia strada e che metterò tutto me stesso per costruirla al meglio.

Quali sono i libri che più ti hanno aiutato?

Consigliamene altri dai, basta rispondere a questa email.

E detto questo, buona settimana e beccati le risorse.

Daniele
