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
title: "\U0001F9F0 kSC #66: Para, PPV e Zettelkasten..."
colors: colors-a
date: '2023-12-03'
description: qual è il miglior sistema per il tuo cervello digitale?
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
    text: "## **\U0001F465 Audience research, fatta facile**\n\nHai bisogno di informazioni sull'audience che stai cercando di creare?\n\nLe persone che ne fanno parte potrebbero essere su Reddit?\n\n​[Se non sai rispondere a queste domande, questo tool ti aiuterà.](https://gummysearch.com/)​\n\n​\n\n## **\U0001F680 La parte nascosta della produttività**\n\nTanti strumenti cercano di diventare lo strumento che centralizza tutte le cose importanti.\n\nMa è possibile?\n\n​[E se ci fosse un'altra strada per ottenere lo stesso risultato?](https://julian.digital/2020/01/17/superhuman-the-productivity-meta-layer/)​\n\n​\n\n## **\U0001F4B8 Niente storie, solo case study**\n\nLe storie di persone che sono riuscite a monetizzare la loro idea non bastano mai.\n\n​[Soprattutto se più che storie sono veri e proprio case study, no?](https://www.indiehackers.com/post/lessons-from-bootstrapping-my-side-project-to-10-000-monthly-revenue-2bbb83a872)\n\n"
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
slug: >-
  ksc-66:-para-ppv-e-zettelkasten-qual-e-il-miglior-sistema-per-il-tuo-cervello-digitale
---
Qualche tempo fa, Tiago Forte ha pubblicato un nuovo libro.

Ma devo essere sincero, quando ho scoperto il titolo di questa nuova uscita, sono rimasto piuttosto deluso.

Pensavo si sarebbe dedicato a qualche nuova scoperta nel mondo della produttività, invece il libro era un approfondimento su qualcosa di già esplorato.

Il nuovo libro è **The PARA Method: Simplify, Organise and Master Your Digital Life.**

In pratica è un approfondimento su uno degli aspetti più basilari del suo Second Brain, il **metodo Para**.

In ogni caso, ho messo da parte la delusione e ho acquistato il libro.

L'ho cominciato a leggere e devo dire che, per quanto conoscessi e avessi già implementato molte delle cose dette in questo libro, ce ne sono tante altre che ho **scoperto**.

E tante altre che, invece, mi hanno fatto pensare al **rapporto che c'è tra il Para e gli sistemi altri più diffusi.**

Qual è il migliore sistema per gestire le note?

E quale sistema consiglierei a qualcuno che che parte dall'inizio?

***

**TL;DR**

*   Para, PPV e Zettelkasten, qual è il miglior sistema per il tuo cervello digitale?

*   Audience research, fatta facile;

*   La parte nascosta della produttività;

*   Niente storie, solo case study

**Il tempo di lettura previsto è**: 8 minuti

***

Ok, chiariamo una cosa.

Questa newsletter non sarà una disamina approfondita e maniacale di tutti i sistemi per gestire le note.

In questa newsletter ti parlerò di solo tre sistemi:

*   il sistema Para

*   Il sistema PPV

*   Il metodo Zettelkasten

Continua a leggere e capirai cosa sono.

E anche perché ho scelto proprio questi.

​

## **Il metodo PARA**

Questo è il metodo creato da Tiago Forte e alla base del suo Second Brain.

Forse è il metodo più noto, tra tutti quelli che citerò nel corso di questa newsletter.

Ed è anche il metodo che mi ha portato alla creazione del [mio primo template Notion](https://danieledamico.gumroad.com/l/easy-second-brain), perché pur sembrando semplice non è così facile da mettere in pratica.

In ogni caso, che roba è?

PARA è l'acronimo di queste parole qui:

*   Projects

*   Areas

*   Resources

*   Archives

E queste parole coincidono con le cartelle/database/pagine in cui dovrai organizzare le tue informazioni.

Sembra facile, ma fidati che non lo è per tutta una serie di motivi.

Innanzitutto, devi scegliere a cosa vuoi che le parti del tuo PARA corrispondano.

Vuoi che siano cartelle?

Vuoi che siano dei database?

Vuoi che siano delle pagine?

E poi perché. devi capire altre cose.

Ad esempio, come devi collegare le parti del tuo PARA tra loro?

E poi, cosa si intende preciso per Projects?

E per Areas?

E per Resources? E Archives?

Dai, penso tu abbia capito la questione.

È un sistema facile da capire nelle sue basi, ma che lascia tanto **spazio di manovra a chi lo implementa.**

Ora però ti dico alcune cose che ti potranno essere utili, se hai intenzione di seguire questo metodo.

Prima di tutto, ricorda che il **modo in cui implementi il PARA dipende dallo strumento** che hai deciso di utilizzare per gestire le tue note (Notion, Obsidian, Evernote ecc.).

Inoltre, ricorda che un **Progetto** è qualcosa che ha una **data di scadenza e che punta ad un obiettivo misurabile.**

Le Areas, invece, sono **aree di responsabilità** che ricopri nella tua vita e che richiedono una tua attività in modo indeterminato.

Infine, ricorda che questo è un metodo di gestione delle note che punta alla **semplicità**.

E per questo, i requisiti minimi di implementazione sono comprensibili in pochi secondi.

Davvero, ti basta creare 4 cartelle su Evernote (più una di Inbox) e il gioco è fatto.

Ma se ti ritrovi a passare troppo tempo nella costruzione e a farti mille domande, **torna alle basi** oppure scegli un altro metodo.

Te lo consiglio se sei quel tipo di persona che vuole dare una prima vera struttura alle sue note e non vuole complicarsi troppo la vita.

Se vuoi saperne di più, Tiago Forte stesso ne parla in abbondanza sul [suo canale Youtube](https://www.youtube.com/@TiagoForte).

Qui sotto, invece, ti lascio uno screen del mio template Easy Second Brain.

​

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/8Pgpp1JAbdKW31HHomjUxT/email) |
| --------------------------------------------------------------------------------------- |

​

## **Il metodo PPV**

Questo è il metodo creato da **August Bradley**, anche lui esperto di produttività come Tiago Forte.

E anche lui Notion Ambassador come me e Beatrice, giusto per dire.

A differenza del PARA, questo è un sistema un po' più strutturato.

Ma questo non significa che non sia poco potente.

Alla base della struttura di sto sistema ci sono:

*   Pillars

*   Vault

*   Pipelines

I pillars sono i pilastri di tutto il tuo cervello digitale.

Sono Le aree dove fai le cose più cruciali, come dormire, mangiare o lavorare e sono l'alternativa ai Projects ed Areas del Para di Tiago Forte. Capire quali sono questi pilastri ti aiuta a capire cosa è davvero importante per te.

E dove metti le cose più importanti?

Le metti nel Vault, la **cassaforte**.

E sta cassaforte è il punto in cui raccogli le informazioni nello strumento da te scelto.

Su Notion possono essere dei database, su Evernote delle cartelle e su Obsidian delle raccolte dataview.

E devi fare particolare attenzione all'ultimo punto, le Pipelines.

Le Pipelines sono i processi, una cosa che non è compresa nel metodo di Tiago Forte ma che è molto efficace.

È il modo con cui August ha provato a rendere più efficace non solo l'**organizzazione** delle informazioni ma anche tutta la loro **gestione** tramite una serie di azioni fisse e fondamentali per l'effettivo funzionamento del sistema.

E questo significa che August introduce il concetto di **manutenzione del sistema**, un concetto molto limitato nel Para.

Qui invece no, è un processo fondamentale e se lo salti tutto il **sistema rischia di diventare inutilizzabile** in poco tempo.

L'ho provato io stesso sulla mia pelle.

Per qualche mese ho messo in pratica il sistema di August Bradley, sul mio Notion personale, e mi piaceva perché riusciva a dare struttura.

Mi sentivo un tantino più saldo rispetto al Para.

Poi però ho saltato qualche Weekly Review e dopo pochi mesi il sistema è diventato inutilizzabile (e quindi sono passato a [questo](https://ckarchive.com/b/e5uph7hp5evpniwlggolea7p2mw22)).

Se sei il tipo di persona con poca disciplina e che non vuole dedicare con regolarità una parte del suo tempo alla manutenzione delle note, allora questo non è il metodo che fa per te.

Se invece vuoi una **struttura definita** e ti piace **organizzare le cose**, magari su Notion (dove il sistema di Bradley è più efficace), allora questo è il metodo che fa per te.

​[Qui](https://www.youtube.com/@augustbradley) trovi tante altre informazioni utili sul sistema.

E qui sotto trovi uno screen della vecchia versione di questo sistema che avevo implementato sul mio Notion personale.

​

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/qJ6w7kScmh9HKzBSSRVU92/email) |
| --------------------------------------------------------------------------------------- |

​

## **Il metodo Zettelkasten**

Questo metodo è interessante.

Questo metodo non si preoccupa tanto di farti fare cose, o di aiutarti a gestire la tua vita personale e professionale.

Questo metodo ti aiuta a **raccogliere le tue idee**, **collegarle** tra loro e permettere a queste di **prendere nuova forma**.

Insomma, è un metodo più volto alla **creazione di contenuti** e all'esplorazione del tuo cervello digitale.

Ne ho parlato parecchio nei precedenti numeri di questa newsletter.

E ne ho anche creato un [template](https://danieledamico.gumroad.com/l/easy-zettelkasten-system), perché proprio come nel caso del Para, sembra semplice ma non lo è.

Qui la situazione è semplice, se non ti importa molto di gestire la tua vita ma vuoi solo gestire le idee tue (e che incontri) per poi vedere dove ti possono portare, questo è il metodo che fa per te.

Puoi trovare più informazioni sul metodo [qui](https://ckarchive.com/b/8kuqhoh0q7x7rckhzxzz399) e [qui](https://ckarchive.com/b/5quvh7hv7v3xvu6hrno0l44) (se vuoi continuare a leggere roba mia) e se invece vuoi leggere roba di altri ti basta cercare su Medium o Youtube.

Qui sotto ti lascio uno screen del mio template Easy Zettelkasten System.

| ![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/gMoqxaSBqQ3VBSdQUSJPhy/email) |
| --------------------------------------------------------------------------------------- |

​

​

Ok, ho cercato in tutti i modi di lasciare le cose semplici.

Il mondo dei framework, sistemi e metodi per gestire le tue note è fitto e pieno di sentieri oscuri.

Avrei potuto dedicare interi numeri di newsletter a solo alcuni di questi metodi, ma credo che la cosa non sarebbe stata sostenibile né per me né per te.

Oppure avrei potuto citare altri sistemi meno noti e più complessi.

Ma ho preferito parlare di quelli che, da quanto ho testato, mi sembrano essere i più efficaci anche per **persone poco esperte**.

E di sicuro questa newsletter non ti sarà utile se pensi di utilizzarla per capire tutto sui metodi che ho citato.

Tiago Forte e August Bradley hanno costruito un'intera carriera su questi metodi, dopo anni e anni di esperienza, e conoscere il frutto di questo loro lavoro grazie alla lettura di poche righe sarebbe folle.

Ti consiglio di prenderla più come un **punto di partenza** per cominciare la tua esplorazione.

Leggila e se trovi che un metodo possa essere adatto alla tua situazione, approfondisci utilizzando i link che ti ho lasciato.

Ti ho anche lasciato alcuni template che puoi utilizzare (sono i miei template, ma ce ne sono centinaia sul web).

Se poi ti piacerebbe che io approfondissi di più uno di questi metodi, **rispondi a questa email** e fammelo sapere, sarò più che felice di farlo.

Un **ultimo consiglio** che ti voglio dare è quello di non vedere questi metodi come una scelta senza ritorno, oppure come qualcosa le cui regole non possono essere violate.

L'efficacia di un metodo dipende da quanto questo aderisca alla tua vita e se è necessario modificarlo, per farlo aderire meglio alla tua vita, allora fallo pure senza problemi.

E soprattutto, non passare ore a valutare la scelta del miglior metodo.

Scegli quello che ti ispira di più, approfondisci un po' e poi buttati.

E se ci sono problemi, scrivimi senza timore!

Detto questo, buona settimana e beccati le risorse.

Daniele
