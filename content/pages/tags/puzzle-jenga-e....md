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
title: "\U0001F9F0 kSC #49: PUZZLE, JENGA..."
colors: colors-a
date: '2023-07-30'
description: e system thinkin!
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
      - label: PROBLEMI COL TUO SISTEMA?
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://zcal.co/notionbuilders/quick-talk'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nLa credibilità è una componente importante nella creazione di un'audience.\n\nÈ difficile crearla ma è facile perderla.\n\n​[Per questo, dovresti fare tesoro di questa lista.](https://medium.com/the-mission/15-credibility-killing-phrases-to-banish-from-your-vocabulary-1f84f2ebafe6)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nE se i meeting che fai (o che cancelli) avessero un valore economico?\n\nCome ti comporteresti?\n\n​[Da oggi puoi scoprirlo!](https://twitter.com/petergyang/status/1679130177819881475)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nUno dei concetti più interessanti elaborati da Naval Ravikant è quello del personal monopoly.\n\n​[E questo è un modo con cui puoi trovare il tuo, usando l'AI!](https://aisolopreneur.beehiiv.com/p/use-chatgpt-build-navals-personal-monopoly)​​\n"
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
slug: puzzle-jenga-e...
---
Ehi ciao 👋,

questo è il numero 49 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò di **3 lezioni di system thinking applicate a Notion.**

<br>

***

**TL;DR**

*   3 lezioni di system thinking applicate a Notion

*   Justin Welsh e ChatGPT ti aiutano con i contenuti

*   Usa il browser per essere produttivo

*   TI servono idee?

**Il tempo di lettura previsto è:** 5 minuti.

***

<br>

Settimana scorsa ti ho spiegato, a modo mio, cos'è il system thinking e che relazione ha con Notion.

Ora, non sto qui a ripeterti di nuovo le stesse cose.

Se vuoi più dettagli, ti consiglio di recuperare [la vecchia newsletter](https://danieledamico.tech/tags/system-thinking-e-notion-la-(poco\)-strana-coppia/).

Ma in breve ti posso dire che la relazione tra Notion e il system thinking c'è ed è molto forte.

**Notion è lo strumento migliore per mettere in pratica e per comprendere il system thinking.**

Ma a che risultati porta mettere in pratica il system thinking su Notion?

Il risultato più grande è di sicuro quello che impari tante cose sui sistemi e queste sono le tre lezioni più grandi che ho imparato io:

*   Nei sistemi l’espressione 2+2=4 è falsa

*   Start with why

*   Mai sottovalutare i sistemi

Pronto?

​

### **NEI SISTEMI L’ESPRESSIONE 2+2=4 È FALSA**

Iniziamo cosi, mettendo in dubbio la matematica.

E no, non sono impazzito, la cosa ha senso e ora te la spiego meglio.

Pensa al **puzzle**, l'analogia con cui ti ho spiegato il System Thinking nello scorso numero della newsletter.

A comporre il sistema puzzle ci sono diverse cose:

*   **elementi** (i tasselli del puzzle)

*   **relazioni** (i modi in cui puoi unire i tasselli)

*   **scopo** (il motivo per cui fai il puzzle)

E prendere una sola di queste cose, considerandola come unica parte del sistema, significa **guardare al sistema in modo riduttivo** e fare danni.

In pratica, pensare che un sistema sia costituito solo dai suoi elementi (la parte più evidente) è un **errore**.

Perché altri due dei costituenti di un sistema (le relazioni e lo scopo) non sono visibili agli occhi.

E su Notion hai una chiara dimostrazione di sta cosa quando agisci su un solo database, lo modifichi, costruisci pagine diverse per utilizzo e magari non consideri il processo di utilizzo ideale.

Arriva la prima persona che non ha le tue stesse idee e magari utilizza un processo diverso, usa il tuo sistema e tutto **si scassa**.

E questo accade perché ti sei concentrato solo su una parte del sistema, non sul suo complesso.

​

### **START WITH WHY**

Ho conosciuto Simon Sinek qualche tempo fa, quando vidi per caso un [suo video su Youtube](https://www.youtube.com/watch?v=u4ZoJKF_VuA&t=2s).

Parlava di quanto è importante, nelle relazioni umane, partire dai motivi che spingono le persone ad agire.

E chi lo avrebbe mai detto, ma questa cosa è valida anche per i sistemi.

Delle tre parti che costituiscono un **sistema**, infatti, sembra ce ne sia una un po' più importante delle altre.

E questa parte è lo **scopo**.

Perché modificare lo scopo ti permette di **cambiare il comportamento anche delle altre parti**.

Ma cambiamo paragone, così ti sarà più chiaro.

Anche una squadra di rugby è un sistema.

Ci sono gli elementi, che sarebbero i giocatori della squadra.

Ci sono le relazioni, che sarebbero le regole del rugby e i legami tra i giocatori.

E c'è lo scopo, che può essere quello di vincere la partita.

Ora, che succede se provi a cambiare tutti i giocatori?

Niente di che, le regole del gioco restano le stesse e anche lo scopo resta lo stesso.

E che succede se cambi le regole del gioco?

Anche qui, niente di che, puoi lasciare gli stessi giocatori e questi troveranno un modo diverso per vincere.

Ma che succede se invece di puntare alla vittoria della partita, punti al puro divertimento?

Allora **cambia tutto il sistema**.

Per adattarti a questa modifica, dovresti cambiare giocatori, cambiare le regole del gioco e le relazioni tra di loro.

Insomma, un bel casino e solo perché hai agito sullo scopo.

Su Notion puoi creare un **sistema per la produzione dei contenuti** oppure puoi creare un **sistema per pubblicare i post su Linkedin**.

E la **differenza** anche se sembra minima è invece è abissale.

​

### **MAI SOTTOVALUTARE I SISTEMI!**

Questa è forse la lezione più importante.

Perché i sistemi sono fighi, fighissimi, ma sono anche **subdoli**!

Intervenire su un sistema è un po' come giocare a Jenga.

Hai presente no?

È quel gioco dove hai davanti una torre fatta da tanti blocchi collegati tra loro e te devi rimuovere un blocco alla volta, senza far cadere la torre.

Se sposti il blocco sbagliato, cade tutto.

E lo stesso vale per i sistemi, se agisci sulla leva sbagliata sei nei guai.

Perché la verità è che siamo circondati da sistemi e noi stessi siamo sistemi.

Solo che abbiamo sempre una **vista limitata** dei sistemi di cui facciamo parte.

Magari conosciamo gli elementi di un sistema, ma non conosciamo le regole.

Oppure non conosciamo lo scopo.

E questo vale anche su Notion, magari elimini una pagina che pensi essere una semplice tabella e invece è la sorgente del tuo CRM.

E in tel caso, mi dispiace per te, ma il **sistema ti ha fregato**.

​

​

Ora, mi auguro che tu non sia in una situazione del genere, eh.

Ma se così dovesse essere, ho una **soluzione** per te.

Rivolgiti a chi se ne intende di Notion e di sistemi, così non sarai tu a doverti preoccupare di sti casini e potrai concentrarti sul tuo lavoro.

Ti basta cliccare sul **pulsante qui sotto**.

E detto questo, per oggi è tutto, buona settimana e **beccati le risorse**.

Daniele

