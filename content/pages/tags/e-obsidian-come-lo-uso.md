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
title: "\U0001F9F0 kSC #45: UN MVP PER I TUOI PROGETTI DI VITA…"
colors: colors-a
backgroundImage:
  type: BackgroundImage
  url: /images/bg2.jpg
date: '2023-07-02'
client: Awesome client
description: su Notion
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

questo è il numero 371 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò di **dell'MVP dei grandi progetti, su Notion!**

<br>

***

**TL;DR**

*   Creare un MVP per i tuoi grandi progetti, su Notion!

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 4 minuti e 30.

***

<br>

Ok, tutti devono avere obiettivi nella vita.

È una cosa ovvia.

C'è chi preferisce avere obiettivi a distanza di un anno, chi a due anni e chi di più.

Io però ho sempre avuto un **problema sulla questione**.

Ho sempre avuto difficoltà a capire se un obiettivo poteva rendermi soddisfatto per davvero.

Sarà una paranoia mia, ma quando mi metto a fare i piani del futuro, mi ritrovo sempre a dire una cosa del genere.

"Ok, ora mi metto e mi impegno per i prossimi 4-5 mesi per raggiungere questo obiettivo.

Ma se poi mi rendo conto che l'obiettivo non mi rende felice?"

​

## **L'MVP DEI GRANDI PROGETTI, SU NOTION**

In tal caso, succede che hai sprecato tempo.

E ok, magari hai imparato cose, ma il risultato è comunque uno spreco.

Quindi che si fa?

E che c'entra Notion?

*   Tim Ferriss, gli esperimenti di due settimane e i progetti di 6 mesi

*   Come creare il tuo MVP su Notion;

*   E dopo l'esperimento?

Come avrai intuito, ora te lo spiego.

​

### **TIM FERRISS, GLI ESPERIMENTI DI DUE SETTIMANE E I PROGETTI DI 6 MESI**

Per anni il dubbio è rimasto nella mia testa.

Poi ho sentito un [podcast di Tim Ferriss](https://podclips.com/c/LacN4G) e ho capito una cosa fondamentale!

Ho capito che puoi fare **esperimenti anche con i tuoi progetti a lungo termine**.

Esperimenti in cui provi una versione ridotta del tuo obiettivo a lungo termine, senza dedicarci mesi ma solo un paio di settimane.

Così, alla fine delle due settimane, se la cosa ti è piaciuta e hai ottenuto risultati rilevanti, allora puoi passare all'obiettivo a lungo termine.

Altrimenti, cambi esperimento o cambi obiettivo.

In pratica, **un MVP per gli obiettivi di vita**.

E la cosa mi ha fatto scoppiare il cervello.

​

### **COME CREARE IL TUO MVP SU NOTION**

E dato che ho le mie fisse, ho preparato un **sistema per costruire questi MVP su Notion**.

Come ci sono riuscito?

*   Ho usato il database Area

*   Ho usato il database Goals

*   Ho creato il database Sprint/Esperimenti

Il primo database, quello "Area", è un semplice database in cui inserisco le **aree principali in cui suddivido la mia vita**.

In particolare, le aree sono: Lavoro, Relazioni e Salute.

Poi, è il turno del secondo database, quello chiamato Goals.

In questo database, inserisco tutti gli obiettivi che vorrei raggiungere a lungo termine.

Cerco di avere un **limite massimo di 3 obiettivi a lungo termine per area**.

Infine, è il turno del database Sprint/Esperimenti.

E questo è il contro principale di questo piccolo sistema.

All'interno di questo database, inserisco le date di inizio e di fine dell'esperimento e altre proprietà utili (se l'esperimento è attivo, quali sono i criteri di successo ecc).

Infine, creo due proprietà.

Una **Relation** al database Goals (che uso per collegare l'esperimento all'obiettivo a lungo termine di cui è un MVP) e poi una proprietà **Rollup** che mostra, in automatico, l'area a cui questo esperimento appartiene.

​

### **E DOPO L'ESPERIMENTO?**

Così, ogni volta che mi salta in mente un nuovo obiettivo a lungo termine, penso prima al modo in cui lo posso sperimentare.

E questo cambia tutto.

Perché così, ogni obiettivo a lungo termine porta in sé fin dall'inizio, una **maggiore possibilità di successo**.

Non è più un semplice obiettivo nell'etere, è qualcosa di pratico fin dall'inizio.

E c'è un piano, ci sono dei task, l'investimento di tempo è minimo.

Insomma, per me è un sistema molto efficace.

​

Ora, non dico che per te possa rivelarsi utile allo stesso modo, eh.

Ma credo che, se hai incontrato le mie stesse difficoltà in passato, allora dovresti farlo un tentativo.

Consideralo un esperimento, che dici?

Capita la battuta?

E niente, direi che anche per oggi è tutto, buona settimana e **beccati le risorse**.

Daniele
