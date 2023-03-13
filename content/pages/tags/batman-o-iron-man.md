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
title: "\U0001F9F0 kSC #21: Meeting notes efficaci"
colors: colors-a
date: '2023-01-08'
description: CHI PREFERISCI?
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nUna delle risorse migliori per fare audience building?\n\nAvere una newsletter.\n\n​[E con questo potrai scegliere il mezzo migliore per mandarne.](https://inboxcollective.com/aweber-beehiiv-convertkit-ghost-mailchimp-substack-which-is-the-right-esp-for-your-indie-newsletter/?utm_campaign=Email_alert_01-05-23\\&utm_medium=email\\&utm_source=Inbox_Collective_email_list)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nSarà anche un po’ datato, ma Excel resta una bomba.\n\n​[E questi sono alcuni modi per utilizzarlo e migliorare la tua produttività.](https://twitter.com/fluentinfinance/status/1611807041399705600?s=61\\&t=HrF1ZltgF6iaTV72GO-SWA)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nStai per lanciare qualcosa di tuo?\n\n​[Allora avrai bisogno di tutte ste cose.](https://launchpedia.co/?ref=producthunt)\n\n"
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
slug: batman-o-iron-man
---
Ho letto fumetti per anni.

Oggi sono passato dai classici fumetti Marvel e DC a graphic novel più contorte ed a tratti inquietanti.

Ma c'è una cosa che ricordo in particolare di quando leggevo i fumetti: le ore passate a fare il confronto tra personaggi diversi dei fumetti.

Chi è più forte tra Hulk e Superman?

Chi è più intelligente tra Mr. Fantastic e Batman?

L'hai capito, mi divertivo con poco.

E più simili erano i personaggi, tanto più il confronto si faceva interessante.

Il confronto che generava più dibattito?

Quello tra Batman e Iron-Man.

Perché entrambi erano playboy miliardari, entrambi erano sprovvisti di super-poteri e compensavano con un'armatura.

Inoltre, c'era un'altra cosa che li accomunava: **l'assistente**.

<br>

***

**TL;DR**

*   L'AI migliore;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 40.

***

Ehi ciao 👋,

questo è il numero 236 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò delle **differenze (e somiglianze) tra Notion AI e Chat GPT**.

<br>

Quando si parla di intelligenza artificiale, in questi giorni il primo tool che emerge nella mente è di sicuro ChatGPT.

E ci sta, è un tool davvero interessante e potente.

E sembra che tutto l'internet ci stia giocando.

C'è anche da dire che nello stesso periodo di uscita di ChatGPT, un'altra intelligenza artificiale si è affacciata sui nostri schermi: quella di Notion.

E devo essere sincero con te.

Per quanto ChatGPT sia divertente ed interessante, ho sempre tifato per la versione di intelligenza artificiale made in Notion.

Purtroppo però, tra Notion AI e ChatGPT c'è un chiaro vincitore.

Ed oggi ho intenzione di rivelarti di quale tool si tratta.

<br>

## **L'AI MIGLIORE**

Da un lato c'era Alfred: il vecchio maggiordomo di Batman.

E dall'altro Jarvis: l'intelligenza artificiale creata da Iron-Man.

Entrambi questi assistenti aiutavano l'eroe ad affrontare le missioni e fare tutte quelle cose che fa un eroe.

Ma questi assistenti sono molto diversi tra loro: il primo è un essere umano e il secondo un'intelligenza artificiale.

Jarvis ha accesso a tutte le informazioni del mondo, raggiungibili alla velocità di pochi secondi, mentre Alfred può fare cose vere e proprie (tipo portare il caffè, cosa fondamentale per un individuo che passa la notte a pestare i criminali).

E devo dire che, quando si parla di Notion AI e ChatGPT, vedo tra i due tool una dinamica molto simile a quella che c'è tra Alfred e Jarvis.

*   tra Notion AI e ChatGPT ci sono tante differenze;
*   tra Notion AI e ChatGPT c'è qualche somiglianza;
*   tra Notion AI e ChatGPT c'è solo un tool che ti consiglio di utilizzare.

Ecco cosa ne penso.

<br>

### **LA SOLUZIONE PIÙ COMODA**

Se c'era una cosa che, fin da subito, mi attirava di Notion AI era la possibilità di poter avere un'assistente virtuale (e intelligente) lì nello stesso posto dove faccio cose.

Mi immaginavo già favolose vicende.

Tipo che cominciavo a scrivere i post per la prossima settimana su Linkedin e, non appena ne avevo necessità, potevo chiedere all'intelligenza artificiale di Notion di, non so, propormi qualche idea per gli hook.

Oppure, nel caso in cui mi fossi ritrovato in un blocco creativo, chiedere a Notion AI di fare un po' di brainstorm.

Così non avrei dovuto aprire nuove schede, non avrei dovuto interrompere il mio lavoro.

Tutto a disposizione, lì dove effettivamente fai cose.

E la cosa è fattibile.

Mentre sei lì, a scrivere qualcosa, puoi cliccare su "/" e ti compariranno 10 di comandi di AI che puoi scegliere e direi all'AI cosa vuoi che faccia.

Ed è proprio qui che c'è la prima, grossa, differenza.

A ChatGPT non devi dare nessun comando particolare.

ChatGPT è davvero un assistente: le scrivi in chat quello di cui hai bisogno e l'intelligenza artificiale te lo fornisce.

Notion AI invece no.

Ecco due immagini di confronto.

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/pxs3iBHSnW24wbYHJS8ZXf/email)

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/oPAxs7dhs8NYih5Xv8c9EF/email)

Credo che la situazione sia palese.

Nel caso di Notion AI devi prima capire di cosa hai bisogno, dargli una sorta di etichetta.

Con ChatGPT invece non ne hai bisogno, ti basta scrivere in chat quello di cui hai bisogno ed a tutto il resto ci pensa l'intelligenza artificiale.

<br>

### **L'AI PIÙ POTENTE**

Qui la questione si fa più spinosa.

Perché ad oggi i vari tool di AI che ci sono a disposizione, per quanto ci siano magari delle differenze in termini di velocità e altre prestazioni, danno più o meno lo stesso risultato.

Continuiamo l'esempio di prima.

Ho fornito ad entrambe le intelligenze artificiali questa richiesta: "Ehi, mi dai qualche idea di subject line per una newsletter sul confronto tra Notion AI e ChatGPT ?".

E qesti sono i risultati che mi hanno fornito.

Come puoi vedere, al netto delle differenze di utilizzo (e della facilità con cui puoi modificare il risultato fornito da ChatGPT), i risultati sono quasi gli stessi.

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/s23Rao7Azv5ydBFG3JkqqF/email)

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/u8uPCRxX3m1r74jk3Jzjbm/email)

<br>

### **NOTION AI O CHATGPT, QUALE UTILIZZARE?**

Al momento, il mio consiglio è chiaro: dovresti utilizzare ChatGPT.

La qualità dei risultati, almeno nel mio caso, non è mai stata la discriminante.

Perché non mi aspetto davvero che l'intelligenza artificiale faccia tutto il lavoro.

E non è neanche quello che vorrei, sarò sincero.

Io voglio che l'AI mi renda più snelli alcuni processi: dalla cattura di idee, ricerca di informazioni ecc.

Quindi per me è necessario avere la possibilità di fare da editor e dare una struttura ed uno stile a quello che mi ha fornito l'AI.

E questo, per ora, mi è possibile molto meglio con ChatGPT invece che con Notion AI.

Ed è un peccato, perché tutto quello che permetterebbe a Notion AI di raggiungere l'utilità ideale per me (e penso tanti altri come me) sarebbe quell'aspetto più di assistente che ha ChatGPT.

Con questo piccolo vantaggio di comodità e la possibilità di avere tutto nello stesso luogo, Notion AI sarebbe il vincitore assoluto.

<br>

Ecco, per ora è questa la situazione.

Per ora, almeno per me, il vincitore è ChatGPT.

Ma c'è da dire una cosa, una molto importante.

Notion AI è in alpha e ChatGPT è uscita da meno di un mese.

Sono tool che si trovano in una versione del loro sviluppo embrionale e presto li vederemo evolvere, così come vedremo evolvere gli stessi modelli di AI che utilizzano.

In pratica, siamo solo all'alba di qualcosa di molto figo.

Qualcosa che, di sicuro, sarà a pagamento (sia nel caso di Notion che di ChatGPT) ma che potrà avere un impatto molto positivo sul nostro lavoro.

Non ci resta che attendere e vedere.

Te nel frattempo, quale tool preferisci?

Detto questo, per oggi è tutto, buona settimana e beccati le risorse!

Daniele
