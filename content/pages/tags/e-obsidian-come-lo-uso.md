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
title: "\U0001F9F0 kSC #47: E OBSIDIAN?"
colors: colors-a
backgroundImage:
  type: BackgroundImage
date: '2023-07-02'
description: COME LO USO?
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nSei alla ricerca di una nicchia nuova da aiutare?\n\n​[Questa potrebbe fare al caso tuo, non ne parla ancora nessuno ma è in esplosione.](https://www.ramoswriter.com/rising-finance-phenomenon/)​​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nQuando si parla di produttività, scommetto che pensi a risparmiare tempo.\n\nO almeno, a utilizzarlo in modo più efficace.\n\n​[E in tal caso, dalla newsletter](https://emiliodalbo.substack.com/p/4-abitudini-da-1-minuto-per-salvare) [Trasumanare](https://emiliodalbo.substack.com/p/4-abitudini-da-1-minuto-per-salvare)[  che secondo me dovresti seguire, questo articolo ti potrebbe aiutare proprio a raggiungere questo obiettivo.](https://emiliodalbo.substack.com/p/4-abitudini-da-1-minuto-per-salvare)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nL'hub centrale di tutti i tuoi tentativi di monetization?\n\nL'homepage del tuo sito (o con un po' di sforzo, il profilo del social che più utilizzi).\n\n​[Ma come costruirla al meglio?](https://twitter.com/jspector/status/1673044526221631488)​\n"
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
slug: e-obsidian-come-lo-uso
---
Ehi ciao 👋,

questo è il numero 374 del **Kit di Sopravvivenza per Creator**.

E oggi ti E oggi ti racconterò di **3 cose che faccio con Obsidian, senza passare per Notion!**

<br>

***

**TL;DR**

*   3 cose che faccio con Obsidian, senza passare per Notion!

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 30.

***

<br>

Ok, ormai sai che uso sia **Notion** che **Obsidian**.

Il primo è al centro di tante mie attività sia personali che lavorative.

E te ne ho già parlato tante volte.

Di come utilizzo il secondo, invece, te ne ho parlato poco.

E, pur avendo detto che uso entrambi gli strumenti per obiettivi diversi, non ti ho mai detto con precisione **per cosa uso Obsidian**.

E oggi ho deciso di rimediare.

​

## **3 COSE CHE FACCIO SU OBSIDIAN, SENZA PASSARE PER NOTION**

E no, non ho intenzione di farti una sconfinata lista di tutte le cose per cui utilizzo Obsidian e non Notion.

Ti racconterò di **3 utilizzi in particolare**.

*   ODG di Notion Builders

*   Scrittura newsletter

*   Reading hub

Non perdiamo tempo e cominciamo!

​

### **ODG DI NOTION BUILDERS**

Lo so, sembra una battuta ma ti giuro che non lo è!

È su Obsidian che gestisco i meeting notes delle riunioni di allineamento settimanali che Beatrice ed io facciamo per [Notion Builders](https://www.notionbuilders.it/).

E fidati di me, c’è un valido **motivo**.

Quando facciamo queste riunioni, io e Beatrice analizziamo tutta una serie di questioni in tante aree diverse.

E pur avendo l’ODG ben mappato sul nostro Notion (grazie a Beatrice), io ho bisogno di processare le informazioni e ragionare utilizzando **mappe concettuali**.

Per questo, mentre passiamo da un punto all’altro, io creo un nuovo **Obsidian Canvas** e faccio la mappa concettuale.

Puoi vedere uno screen qui sotto, ripulito da tutti i dettagli scottanti.

E si, lo so che le mappe concettuali si possono creare anche su Notion, [sono anche bravo a farle](https://danieledamico.tech/tags/sai-vedere-le-informazioni-su-notion/).

Ma devo ammettere che non la trovo ancora una funzione immediata, Obsidian invece ti permette di creare le mappe con molta più facilità.

Inoltre, all’**interno di ogni nodo della mappa puoi linkare una relativa pagina di note**.

E questo mi permette di introdurre nella stessa mappa le risorse che utilizzeremo per risolvere un dato problema.

In pratica, Obsidian Canvas è una bomba!

​

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/efKLJmBYH6M7xEQZR8sN8J) |
| --------------------------------------------------------------------------------- |

​

### **SCRITTURA NEWSLETTER**

Mi piace scrivere più su Obsidian che su Notion, soprattutto quando si parla di testi lunghi.

Obsidian ti permette, grazie ai tanti plugin creati dalla community, di avere un maggiore controllo su quello che scrivi.

Infatti, puoi usare plugin che ti permettono di:

*   vedere l’outline di quello che scrivi;

*   accedere ai tuoi appunti in multitasking;

*   contare le parole che utilizzi e il tempo di lettura.

Insomma, l’**esperienza di scrittura su Obsidian** è di gran lunga migliore rispetto a Notion.

Ma la limito alla newsletter che stai leggendo e **non ai post di Linkedin**.

E perché?

Perché su Linkedin pubblico un post al giorno.

Questo significa che in poco tempo il mio Obsidian sarebbe pieno di tante cose scritte che andrebbero a produrre rumore di fondo.

E non è il motivo per cui uso Obsidian.

Obsidian lo uso in modo più selettivo: è la **parte creativa** del mio Second Brain, non quella organizzativa.

​

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/6i85udbW5Ypn9QHpVQPQFv) |
| --------------------------------------------------------------------------------- |

​

### **READING HUB**

Come forse hai già letto in passato, utilizzo Readwise Reader per leggere e prendere appunti.

Il vantaggio di questo strumento è che ti permette di salvare gli appunti e gli highlights di quanto leggi.

Poi li prende e li esporta in automatico dove vuoi, nel mio caso su Notion e Obsidian.

E una volta che questi appunti finiscono su Obsidian, **li analizzo di nuovo e cerco di creare cose nuove**.

Solo che alcuni li leggo su Obsidian, altri su Notion.

Tutti gli appunti che sono personali, li analizzo su **Obsidian**, e quelli che invece possono essere utili a me o altri li analizzo su **Notion**.

Su Notion, infatti, taggo tutte le letture che voglio condividere con Beatrice, per esempio, e lei ha accesso ai miei appunti, li può commentare e possiamo lavorarci insieme.

Una cosa del genere non sarebbe possibile con Obsidian.

​

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/d23xmr36k1jEq4e1WNzkdi) |
| --------------------------------------------------------------------------------- |

​

Ecco, spero che ora tu abbia un quadro più chiaro di come utilizzo Obsidian e in quali casi lo utilizzo.

Magari hai capito pure lo spazio che riservo a Obsidian e Notion, a seconda delle esigenze.

E magari questa lettura ti aiuterà ad avere un po’ di ispirazione su come utilizzare questi strumenti.

Detto questo, per oggi è tutto.

Buona settimana e **beccati le risorse**.

Daniele

