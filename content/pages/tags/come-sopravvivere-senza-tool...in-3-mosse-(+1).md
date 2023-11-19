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
title: "\U0001F9F0 kSC #63: CREA IL TUO DIARIO DI SISTEMI PERSONALI..."
colors: colors-a
date: '2023-11-12'
description: SU NOTION (O DOVE VUOI)
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
      - label: "\U0001F4D5 CREA IL TUO DIARIO!"
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: >-
          https://scribehow.com/shared/Crea_un_diario_di_sistemi_personali_su_Notion__VB1-eIvrRlOZWugJth4utQ
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
    text: "## **\U0001F465 INIZIA SU YOUTUBE, SENZA VIDEOCAMERA**\n\nVuoi cominciare a fare video Youtube?\n\n​[Ecco una piccola masterclass su come farne col tuo smartphone.](https://aliabdaal.com/how-to-film-youtube-videos-on-your-phone/)​\n\n​\n\n## **\U0001F680 UN MONDO LIBERO DALLE DISTRAZIONI**\n\nTutti sappiamo che le distrazioni sono un grande ostacolo per la nostra produttività.\n\nMa sapere questa cosa non serve a niente, se non troviamo un modo per risolverla, no?\n\n​[Ecco come potresti farlo.](https://www.nirandfar.com/distraction-tracker/)​\n\n​\n\n## **\U0001F4B8 COME SCEGLIERE COSA FARE?**\n\nAncora non hai deciso a cosa dovresti dedicarti?\n\nVuoi trovare qualcosa che sia richiesto per davvero dalle persone?\n\nOk, è applicato al contesto della creazione di prodotti, ma con un po' di fantasia puoi applicarlo al contesto che vuoi.\n\n​[Ecco un modo facile per trovare la strada.](https://twitter.com/stephsmithio/status/1708226328837968232)\n\n"
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
slug: come-sopravvivere-senza-tool...in-3-mosse-(+1)
---
3 membri e più di 20 guest.

Lo spazio Notion di [Notion Builders](https://notionbuilders.it/) stava per trasformarsi in un hotel e presto la cosa sarebbe diventata ingestibile, anche a livello economico.

Per questo, qualche giorno fa, sono andato nella sezione “Settings and members” del workspace che io e Beatrice usiamo per lavorare e ho cominciato a fare **pulizia**.

Solo che ho fatto un errore.

Ho **rimosso anche il mio profilo personale** dai membri e in questo modo sono saltate tutte le integrazioni personali che avevo creato.

Son saltate le integrazioni con Akiflow, con Make e le relative automazioni.

Insomma, un bel casino.

E stava per succederne uno ancor peggiore!

​

**TL;DR**

*   Crea il tuo diario di sistemi personali, su Notion (o dove vuoi)

*   Inizia su Youtube, senza videocamera;

*   Un mondo libero dalle distrazioni;

*   Come scegliere cosa fare?

**Il tempo di lettura previsto è**: 7 minuti (ne vale la pena!)

​

Quando comincio a giocare con integrazioni tra vari tool il mio cervello entra in **modalità ottimizzazione** e comincia a ragionare.

Comincio a chiedermi il motivo per cui utilizzo uno specifico strumento, perché metto in atto uno specifico processo ecc.

Figurati che spesso mi capita di creare automazioni che poi non utilizzo mai.

E lo so, forse sono un caso un po' patologico, ma credo che il discorso valga anche per te (con le dovute eccezioni).

Sono convinto che spesso anche tu ti chiedi se il modo in cui organizzi una data cosa della tua vita sia funzionale oppure no.

E quando poi lo modifichi, ti ci diverti per un po', ma poi **ritorni alle cose che funzionano**.

È un problema comune, lo so.

In ogni caso, mentre riattivavo l’integrazione tra Akiflow e Notion questa parte del mio cervello si è attivata e ho cominciato a farmi tante domande, una più dannosa dell'altra.

Ma ha senso usare Akiflow?

E se creassi questa automazione per inserire i task su Todoist e farli finire su Notion?

E se usassi Things3?

Insomma, cominciavo a pormi sempre più domande fino al punto in cui mi sono chiesto se non fosse stato meglio **gestire tutti i miei task in altro modo**.

E quando comincio a valutare nuovi strumenti o nuovi approcci, allora è chiaro che la **furia mi ha preso**.

È la furia di chi ottimizza le cose per piacere e lavoro e quando mi agguanta è così difficile sfuggirle.

E non lo sapevo, ma ero proprio nelle grinfie della furia mentre mi facevo quelle domande e in poco tempo mi sarei ritrovato a spostare tutto il mio task manager chissà dove.

Così avrei **perso decine di ore** tra lo spostamento, la presa di confidenza col nuovo sistema e le priorità del tutto sballate.

Per fortuna, qualche tempo fa avevo scoperto una cosa.

Avevo scoperto un’arma per combattere contro questa furia: il **diario personale dei sistemi**.

E l'avevo anche **costruita su Notion**!

Quindi l’ho aperta, consultata e la furia è sparita.

E oggi ti svelerò come puoi crearla anche tu, in 3 passi (e una guida dettaglia):

*   Cos'è il diario dei sistemi?

*   Dal dump al database

*   Dal database ai personal SOP

Pronto?

Cominciamo!

​

## **Cos’è il diario dei sistemi?**

Partiamo dalle basi, cos’è un diario dei sistemi personali?

È lo strumento più importante per tutta la tua produttività personale (e non solo).

Si, te lo dico così, senza esagerazioni o falsa modestia.

Perché è la tua **ancora di salvezza** per tutti i casi in cui la [shiny new toy syndrome](https://danieledamico.tech/tags/sistemi-non-bastano/) ti assale, oppure per tutti quei casi in cui scopri un nuovo sistema di produttività e valuti di implementarlo.

In pratica, è lo strumento che ti permette di essere costante con la tua produttività senza sprecare neanche più un minuto dedicandoti ad attività che pensi siano utili, ma che poi non lo sono.

Ok, figo, ma quindi cos'è?

Nella sua versione più semplice è un **documento**.

Un documento che puoi strutturare come vuoi e dove vuoi.

E al suo interno ci puoi inserire tutti i sistemi di produttività, processi, strumenti e abitudini che ti permettono di fare quello che fai.

Dai, tutto quello che utilizzi per **organizzare la tua vita**.

E chiariamolo, non parlo di quelli che vorresti utilizzare.

In questo documento devi inserire solo quelli che metti in atto giorno dopo giorno e per tua scelta.

Oppure puoi inserire quelli che hai deciso di sperimentare.

Tutte le altre cose però non hanno spazio nel tuo diario dei sistemi personali, non le devi inserire.

Quindi, non c’è spazio per i sistemi che vorresti implementare e non c’è spazio per quelli che un tempo mettevi in atto ma ora non più.

E non so se è chiaro, ma te lo dico perché è importante: puoi scrivere questo documento dove ti pare.

Certo, è meglio che tu possa accederci con facilità (e che tu possa trasformarlo in un database), ma puoi crearlo dove vuoi, anche su carta.

Io ho scelto di crearlo su **Notion**, ma avrei potuto crearlo anche su [Obsidian](https://danieledamico.tech/tags/quando-non-hai-altra-scelta-utilizza-obsidian/), su [Tana](https://danieledamico.tech/tags/il-natale-di-notion-o-tana/) o sul mio [bullet journal](https://ckarchive.com/b/e5uph7hp5evpniwlggolea7p2mw22).

​

## **Dal dump al database**

Ok, quindi sto diario dei sistemi è un documento che raccoglie i tuoi sistemi, processi e strumenti.

Lo puoi creare dove vuoi e come vuoi.

E basta così.

Questo è la roba **necessaria e sufficiente** che devi sapere per poter creare il tuo diario.

Ora però voglio darti qualche consiglio su come crearlo al meglio.

È tutta roba **opzionale**, ma credo sia comunque **utile**.

Partiamo dall’inizio.

La prima cosa che devi fare è quella di metterti davanti al pc e **scrivere un elenco di tutti i tuoi sistemi, strumenti, processi e abitudini**.

Non fare troppa filosofia in questa fase, apri un documento a caso e inizia a scrivere.

Ti faccio alcuni esempi di quelli che ho scritto io nel mio:

*   Notion è il mio task manager personale e lavorativo

*   Akiflow è lo strumento che uso per gestire il mio calendar e fare time blocking

*   Ogni mattina scrivo a mano libera, su carta e penna, per 30 minuti

*   Google Calendar: per pianificare gli impegni e tenermi aggiornato sugli appuntamenti

*   Pomodoro Technique: un metodo di gestione del tempo che mi aiuta a rimanere concentrato e produttivo

*   Dropbox: per archiviare e condividere i miei file in modo sicuro

*   LastPass: per gestire e proteggere le password dei miei account online

Sono solo alcuni esempi, ma credo tu abbia capito.

Arrivato al punto in cui non hai altre cose da scrivere (almeno per il momento), puoi fare il **passo successivo**.

E sarò sincero con te, è più semplice farlo su Notion.

Perché su Notion ti basta creare un database, chiamarlo come vuoi e poi selezionare tutto l’elenco che hai scritto e trascinarlo nel database.

In un attimo, ti ritroverai con un database popolato da tutti i punti del tuo elenco.

E potrai cominciare ad aggiungere diverse proprietà (colonne) per **classificare le informazioni**.

Potrai inserire tutte le **proprietà** che vuoi, spetta a te la decisione.

Io però te ne consiglio due in particolare:

*   **Area**: una proprietà di tipo “Multi-Select” che ti permette di selezionare a quale area della tua vita appartiene quello specifico elemento;

*   **Stabilità**: una proprietà di tipo “Select” e ti permette di scegliere se quell’elemento è già stabile nella tua vita o se lo stai sperimentando.

Te l'ho detto, puoi riuscire a fare questa cosa anche con Obsidian, Tana o che ne so.

Solo che Notion è molto più immediato nella creazione di database e per questo te lo consiglio.

Hai provato a creare database su Obsidian?

Hai provato a crearli su Tana?

Fidati, io si e ci ho messo tipo un'oretta per capirlo.

Evita di fare il mio stesso errore, almeno non in questa fase.

Comunque, poi che succede?

​

## **Dal database ai personal SOP**

Succede che passi alla fase seguente.

Hai creato il tuo database e hai creato le proprietà per classificare le informazioni.

Poi hai classificato tutti i record del database, così ogni voce ha una sua area e un suo grado di stabilità.

Ora puoi aprire le singole pagine del database.

E che ci devi fare?

Puoi metterti e **scrivere gli SOP** di quella voce del database.

Ho già parlato in precedenza di come scrivere SOP su Notion, puoi leggere tutto [qui](https://ckarchive.com/b/lmuehmh0rgkd0t6hde0k600).

Sono gentile però e te la faccio breve.

In pratica, per ogni elemento del database, ti basta descrivere quello che fai o come lo fai.

Puoi utilizzare un **elenco numerato oppure checkbox** per descrivere il processo passo dopo passo.

E puoi metterci di mezzo link, collegamenti ad altri processi e tutto quello che ti garba.

Cerca solo di ricordarti di essere **oggettivo**, **descrivere senza ottimizzare** e **scrivere solo le informazioni importanti**.

Alla fine di tutto sto giro, ti ritroverai con un bel database pieno di informazioni utili, stabili e sicure.

La tua ancora sarà pronta e potrai usarla non appena ti rendi conto che la furia sta per prenderti.

​

​

Ok, tutto figo.

Ma perché sta roba ti dovrebbe aiutare?

Perché fornisce **stabilità ai tuoi processi**.

Dopo che hai provato a mettere ordine nella tua vita, dopo che hai descritto in dettaglio le cose che fai e quelle che utilizzi, le probabilità di cedere alla tentazione della furia e mandare tutto all'aria in preda alla distrazione del momento saranno molto più **basse**.

Avrai aumentato di molto la frizione nell'implementazione di un nuovo strumento ed avrai capito che quello che **funziona** nella tua organizzazione.

Inoltre, grazie ad uno strumento come questo, potrai capire subito in che modo i diversi processi, strumenti o abitudini sono **collegati** tra loro.

E potrai vedere che modificandone anche uno solo, rischi di compromettere l’intero castello.

Proprio come succede quando costruisci un bel castello di carte, ne togli una e tutto cade.

Oppure come con le tessere del domino.

Hai capito, no?

Insomma, questo è quello che ho notato io quando ho aperto il mio diario e ho riletto la parte riguardo la gestione dei task.

Ho capito che non aveva senso **rovinare tutto per una semplice distrazione**, non valeva la pena.

Avrei rischiato di perdere ore e di compromettere l'esecuzione di task importanti sia nel mondo lavorativo che in quello personale.

E così, munito di diario, ho combattuto contro la furia.

E l'ho sconfitta.

Non ho cambiato nulla, ho messo da parte l’idea e mi sono **dedicato al mio lavoro**.

Direi che è stata la **scelta più produttiva**, no?

E con questo, direi che per oggi è tutto.

Buona settimana e **beccati le risorse**!

Daniele

​

​

PS:

Penso di aver trovato una soluzione al problema dei **tutorial Notion senza registrare video**.

L'idea di fare video mi attira comunque, ma i lavori sono ancora in corso.

Nell'attesa, per avere una guida dettagliata (passo passo e con immagini) di quello che ti ho descritto, clicca sul pulsante qui sotto.

Troverai tante immagini e poche parole, ne ho usate già tante finora, o sbaglio?
