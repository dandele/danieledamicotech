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
title: "\U0001F9F0 kSC #25: Con Notion puoi creare tutto..."
colors: colors-a
backgroundImage:
  type: BackgroundImage
date: '2023-02-08'
description: Anche un'agenzia!
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nDiciamoci la verità, da quando è uscito ChatGPT tutti hanno cercato di utilizzarlo sui social.\n\nIn qualche caso, l’ho usato anche io con LinkedIn.\n\n​[E da oggi potremo utilizzare questo tool, senza doverci prima studiare ChatGPT.](https://m64.in/linked-xp)\n\n\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nVuoi essere più produttivo?\n\nAllora dovresti riposare.\n\n​[Ma chi ha detto che il solo modo per riposare sia quello di dormire?](https://ideas.ted.com/the-7-types-of-rest-that-every-person-needs/)\n\n​​​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nUno dei mezzi migliori per fare monetization è la creazione di un corso.\n\nMa come si crea un corso? Quale tool utilizzare? Quanto spendere?\n\n​[Con questo, avrai la risposta migliore alla seconda domanda.](https://maven.com/start?ref=producthunt)\n"
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
  - type: CtaSection
    colors: colors-c
    elementId: ''
    backgroundSize: full
    title: Let's do this
    text: >-
      The Stackbit theme is flexible and scalable to every need. It can manage
      any layout and any screen.
    actions:
      - label: Try it now
        altText: ''
        url: /
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-28
          - pb-28
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: col
      title:
        textAlign: center
      text:
        textAlign: center
      actions:
        justifyContent: center
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
slug: agenzia-notion-builders
---
Un anno fa ho ricevuto una **richiesta di collegamento su LinkedIn**.

Era da parte di una ragazza che non conoscevo, Beatrice.

Non avevo idea che da lì ad un anno avrei fondato con lei la prima agenzia italiana di consulenza Notion.

***

**TL;DR**

*   Con Notion puoi creare tutto, anche un'agenzia;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti e 20.

***

Ehi ciao 👋,

questo è il numero 25 del **Kit di Sopravvivenza per Creator**.

Ed oggi ti racconterò **come io e Beatrice abbiamo utilizzato Notion per creare un'agenzia.**

****

Quando Beatrice mi ha scritto, avevo cominciato da poco a pubblicare su LinkedIn.

Parlavo di Notion giusto per testare le acque e vedere come rispondessero le persone.

Di fatto, quei contenuti di test colpirono proprio Beatrice e di lì a poco organizzammo una prima call per fare quattro chiacchiere e parlare di Notion.

Non decidemmo subito di lanciare un’agenzia, anzi, è passato qualche mese da quel nostro primo incontro.

Nel corso di quei mesi ci siamo conosciuti, siamo cresciuti e **abbiamo capito i rispettivi punti di forza**.

Quando poi abbiamo preso la decisione di buttarci in quest’avventura, è stato naturale costruire la casa dei nostri sforzi su Notion.

E oggi ho deciso di **mostrarti proprio questa casa**.

Perché Notion non è solo template, Notion è lo strumento con cui puoi costruire quello che vuoi.

Ma certe volte può essere difficile iniziare senza alcuna **ispirazione**.

​

## **CON NOTION PUOI CREARE TUTTO, ANCHE UN’AGENZIA**

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/h949X9y7u9haYhXoMYGzxF/email)**​**

**​**Ogni volta che io e Beatrice facciamo una call con qualcuno interessato ai nostri servizi, gli mostriamo una cosa.

È una sorta di **demo di quello che Notion può fare**.

Anzi, è una demo di quello che io e Beatrice possiamo fare con Notion.

Di come possiamo utilizzare Notion (e non solo) per **raggiungere determinati obiettivi**.

È la demo di come abbiamo strutturato il **Workspace di Notion Builders**.

La demo di uno spazio Notion nato per costruire un’agenzia, per collaborare da remoto e per gestire i primi clienti.

In particolare, ci sono **3 cose che colpiscono le persone**:

*   La dashboard personale;

*   Il crm;

*   La gestione dei documenti e dei clienti.

Ecco uno sguardo ravvicinato al cuore di Notion Builders.

​

### **LA DASHBOARD PERSONALE**

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/6eerGm4Mc3YAdnp9JMKo8M/email)**​**

****

È giusto partire da questa sezione.

Questa è la sezione che, ogni mattina, io e Beatrice vediamo.

Ed è una **sezione personale**, perché mostra a me solo le cose che riguardano me.

E mostra a Beatrice solo le cose che riguardano Beatrice.

Nella Dashboard personale, infatti, sia io che Beatrice vediamo la stessa struttura di contenuti: i documenti e i task.

Solo che, in questa sezione, **io non voglio vedere i task e i documenti di Beatrice.**

Vederli mi manderebbe in **confusione**, mi farebbe provare **ansia** o altre robe per niente positive.

E lo stesso vale per lei.

Insomma, ci farebbe provare la stessa sensazione che provi anche tu quando qualcuno **interrompe la tua colazione domenicale con una brutta notizia**.

Hai presente, no ?

Ecco, noi non vogliamo provare quella sensazione, vogliamo uno spazio che ci permetta di essere produttivi ed efficienti.

E lo vogliono anche i nostri clienti.

​

### **CRM**

**​**![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/dbDnkm63sSPijDCtZkqHzX/email)

​

Ok, una Dashboard personale è una cosa carina e pulita, ci sta.

Ma è una cosa che ti possono fornire anche altri tool, dov’è la novità?

La cosa innovativa è rappresentata da questo secondo punto, più o meno.

Il fatto è che più sotto della Dashboard personale, ci **sono altre Dashboard**.

C’è quella per **gestire i task complessivi**, con cui sia io che Beatrice possiamo vedere i task dell’altra persona.

C’è quella per **gestire i clienti**, prospect e tutte le persone con cui Notion Builders entra in contatto.

C’è quella per **gestire gli OKR**.

C’è quella per **gestire i documenti** in modo asincrono e senza perdere nulla.

E quella per **gestire le risorse**.

E forse lo hai capito tu stesso, la cosa innovativa è che puoi **gestire tutta sta roba da un solo tool**.

Tutte le informazioni in un unico luogo, tutte che emergono quando servono, dove servono e soprattutto senza che sia tu a doverle cercare.

La sola cosa di cui hai bisogno è la **capacità di costruire il sistema adatto a te**, alle tue esigenze e quelle del tuo team.

E quando non hai quella capacità, è lì che ci chiami.

Come i ghostbusters, che li chiami quando c’è qualcosa di terrorizzante nel tuo vicinato.

​

### **LA GESTIONE DEI DOCUMENTI E DEI CLIENTI**

![](https://embed.filekitcdn.com/e/cdkvYa3enxKN3USgaH1Ddk/s4qTfRX4k6F2AfnYesKkdm/email)

Questa è forse una delle cose che colpisce di più.

Perché avere una vista personale su quello che ti riguarda è utile.

Avere tutte le informazioni nello stesso posto e poter gestire diversi processi da un unico strumento invece che mille è fantastico.

Ma la possibilità di **liberarsi dalla dipendenza da e-mail, notifiche e call è un sogno di tante persone**.

Io ho cercato per tanto tempo un tool che mi aiutasse a fare queste cose, ne ho testati decine.

Poi però ho capito che se non trovi nulla di già pronto, allora **sei tu a doverti costruire la soluzione**.

E quindi la casa di Notion Builders è una casa costruita proprio in questo modo.

Non ci sono messaggi che io o Beatrice dobbiamo cercare su Whatsapp per poter recuperare le password di accesso a qualche servizio.

Non ci sono e-mail che dobbiamo recuperare per ricordare quali sono le esigenze di un cliente.

È tutto su Notion.

Quando uno di noi ha un’idea, crea un nuovo documento su Notion, la descrive in dettaglio e mette in atto un processo che abbiamo definito insieme.

Un **processo** che poi fa finire il documento sulla “scrivania” della persona giusta al momento giusto.

E lo stesso vale per i **clienti**.

Ogni cliente ha accesso ad una Dashboard personale in cui può vedere lo sviluppo dei lavori e come stanno andando le cose.

Il tutto riducendo al minimo lo scambio di e-mail, messaggi o call.

Così siamo tutti più **tranquilli**, con più tempo a disposizione per le cose a cui teniamo e la **serenità** di lavorare nel modo più efficiente possibile.





Ora, queste sono solo alcune delle cose presenti sul nostro Notion.

Ci sono tante altre cose che non ti posso mostrare ancora.

Spero però di averti chiarito le **potenzialità** dello strumento e di cosa ti permette di fare.

L’unico scoglio è la parte di **implementazione e progettazione**.

Ma per quello, se vuoi, c’è [**Notion Builders**](https://www.notionbuilders.it/).

Anzi, nel caso in cui tu non l’abbia già fatto, ti lascio un pulsante qui sotto.

È il **pulsante per prenotare una call con noi**, una rapida e senza impegno.

Cliccaci pure e facciamo quattro chiacchiere!

Detto questo, penso sia tutto, buona settimana e **beccati le risorse**.



​
