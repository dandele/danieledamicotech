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
title: "\U0001F9F0 kSC #40: A COLAZIONE CON L'AI..."
colors: colors-a
date: '2023-05-28'
description: E MOLOCH
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
      - label: CHE NE PENSI?
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://www.linkedin.com/in/daniele-damico/'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nPer creare un'audience devi essere in grado di gestire l'attenzione delle persone (cosa che spero di aver fatto al meglio nella newsletter di oggi).\n\n​[Ecco 7 modi con cui puoi riuscirci quando scrivi.](https://collabfund.com/blog/attention/?utm_source=ForTheInterestedNewsletter)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nDopo una newsletter come quella di oggi, un altro link sulla produttività potrebbe essere eccessivo, no?\n\n​[Ma se proprio non ti bastano, ora sarai felice.](https://nesslabs.com/illusion-of-productivity)\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nPer riuscire a monetizzare devi imparare a utilizzare il prezzo di quello che offri.\n\n​[E questa è una delle tecniche più importanti per riuscirci.](https://customercamp.co/price-anchoring/)​\n"
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
slug: il-mio-funnel-di-produttivita
---
Ehi ciao 👋,

questo è il numero 362 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò del **demone nascosto dietro la produttività tossica**.

<br>

***

**TL;DR**

*   Il demone nascosto dietro la produttività tossica

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti.

***

<br>

Una gran parte dei contenuti pubblicati negli ultimi mesi su questa Newsletter si è concentrata su **Notion** e sulle sue applicazioni.

Altre volte ho parlato di **personal branding, di creator economy e di produttività**.

Oggi però voglio esplorare un po’ di più la mia curiosità.

E voglio parlarti di un’**area nascosta della produttività**.

<br />

## **IL DEMONE NASCOSTO DIETRO LA PRODUTTIVITÀ TOSSICA**

Ok, fai un bel respiro e fidati di me.

Vedrai che alla fine di questa newsletter ti sarà tutto chiaro, ecco l’**outline** di quello che leggerai.

*   A colazione con l’AI e Moloch

*   Che c’entra la produttività?

*   Come uscire dalla trappola di Moloch?

E ora che ho rivelato, almeno in parte, le mie carte direi che possiamo arrivare al sodo.

​

### **A COLAZIONE CON L’AI E MOLOCH**

Qualche giorno fa stavo ascoltando un **podcast di Lex Friedman sull’intelligenza artificiale** e sul motivo per cui si dovrebbe fermare il suo sviluppo per almeno 6 mesi.

Un argomento bello interessante e un po’ inquietante, [ecco il link se vuoi dargli un ascolto](https://www.youtube.com/watch?v=VcVfceTsD0A).

Ad ogni modo, nel corso della discussione con questo tizio chiamato Max Tegmark, si comincia a parlare della spinta umana alla **competizione** anche se questa rischia di essere dannosa.

In particolare, i due si riferiscono a quel tipo di competizione che si crea quando c’è una scoperta importante e tutti cominciano a cercare di accaparrarsi quella scoperta, per usarla come vogliono.

Un po’ com’è successo con la l’energia atomica e la conseguente corsa alle armi.

Ed è in questo contesto che Max Tegmark cita un saggio dal titolo inquietante: “**Meditations on Moloch**”, un saggio che a sua volta cita un poema di Allen Ginsberg, “Urlo”.

In pratica, questo Ginsberg attribuisce al demone Moloch la causa di tanti mali della società.

Ginsberg però è un poeta e quando parla di demoni, in realtà si riferisce ad altro.

In questo caso, quando parla di Moloch si riferisce **alla** **società americana e al capitalismo**, perché stimolano la spinta ad una competizione anche dannosa tra le persone.

E nel podcast, Fridman e Tegmark, fanno notare come questo stesso gioco di competizione malata si stia generando ora nel campo dell’intelligenza artificiale.

Tutti devono fare qualcosa in questo campo, anche se per molti scienziati continuare a sviluppare questa tecnologia, porta dei **grandi rischi per l’intero genere umano**.

Ma non ci si riesce a fermare, perché nessuno vuole farlo, soprattutto se pensa di perdere terreno nei confronti di altri che invece non si fermeranno.

In pratica, tutti **corriamo verso l’abisso** e nessuno riesce a fermarsi.

Pensavi fosse la solita newsletter allegra, eh?

<br>

### **CHE C’ENTRA LA PRODUTTIVITÀ?**

Ora, che c’entra tutta sta roba con la produttività?

C’entra perché mentre Fridman e Tegmark parlavano di AGI e demoni, io pensavo alla produttività e alla sua metà oscura: **la produttività tossica**.

Si tratta di quella produttività in cui finisci quando ti fai prendere dall’**ansia di fare cose** e ti spingi oltre i limiti di **stanchezza e salute**.

“Devo completare tutte le voci nella task list, altrimenti non faccio passi avanti e gli altri mi superano.”

E cosi ti ritrovi a fare le ore piccole, a non riposarti mai ed ecco arrivare il **burnout**.

Quando metti il concetto di produttività insieme al concetto di competizione, allora ecco che emerge Moloch.

Lo vedi con le sue mani demoniache che ti afferra e ti sfida a fare di più, sempre di più.

E chissenefrega se sei stanco e devi riposare, non puoi fermarti perché gli altri non si fermano.

Solo che Moloch non esiste, sia nel caso del poema di Ginsberg, che nel caso dell’intelligenza artificiale.

Nel mondo reale, non c’è nessuno che ci spinge a correre oltre il limite: lo facciamo a causa dell’ansia e di una **malsana competizione** fomentata dalla società e altre cose molto complesse.

​

### **COME USCIRE DALLA TRAPPOLA DI MOLOCH?**

Quindi, Moloch (cioè l’ansia e la competizione) spingono tutti noi a essere sempre più produttivi anche se arriviamo al punto in cui tutta sta **produttività ci fa male**.

E non riusciamo a fermarci, perché non vogliamo perdere il posto nella corsa verso l’abisso.

Che poi, se volessimo fermarci per davvero, come potremmo fare?

Nel podcast, come ho già detto, il modo per fermarsi è tramite lo stop allo sviluppo di AI per i prossimi 6 mesi, figo.

Ma nel caso della produttività tossica, **come ci si ferma**?

Penso che ci siano vari modi che dipendono tutti dalla tua **cazzimma**, come si dice dalle mie parti (sarebbe la grinta).

Ora te li dico in breve, ma in un prossimo numero della newsletter ne parlerò più in dettaglio:

*   Hai tanta cazzimma ma poco controllo sulla tua routine? **Blocca delle giornate** (o anche solo delle ore) ogni settimana per il riposo assoluto (niente pc, niente smartphone e niente attività che ti portino verso i tuoi obiettivi);

*   \- Hai poca cazzimma ma tanto controllo sulla tua routine? Comincia a studiare la [slow productivity](https://www.newyorker.com/culture/office-space/its-time-to-embrace-slow-productivity), [la mindful productivity](https://nesslabs.com/mindful-productivity-2) e prova a metterle in pratica a poco a poco.

*   \- Hai 0 cazzimma e non hai nemmeno idea di cosa sia sta questione della produttività? [Leggi qui](https://www.linkedin.com/feed/update/urn:li:activity:7062831996913225728/).

​

Ok, lo so, è stato un numero di newsletter particolare.

Tuttavia spero che, anche se meno pratico e più critico, questo numero ti abbia permesso di scoprire nuove cose e di **allargare il tuo punto di vista sulla produttività**.

Si tratta pur sempre di un tema presente fin dagli inizi di questa newsletter e dopo quasi un anno di pubblicazione, comincio a voler dire qualcosa di mio, più che curare quello che di altri.

Ma fammi sapere cosa ne pensi, mai come questa volta **sono curioso di sapere il tuo feedback**: preferisci questo approccio oppure lo schema più classico dei consigli su Notion ecc?

Puoi **rispondere a questa stessa email** oppure mandarmi un **messaggio su Linkedin**, ti basta cliccare sul pulsante qui sotto.

E detto questo, buona settimana e **beccati le risorse**.

Daniele
