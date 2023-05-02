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
title: "\U0001F9F0 kSC #36: A SCUOLA DI PRODUTTIVITà..."
colors: colors-a
date: '2023-04-30'
description: DA CAL NEWPORT
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nE per la serie “non credo a queste guide, ma questa mi sembra sia interessante”, ecco un nuovo episodio.\n\n​[Questa volta si parla di newsletter e come farle crescere.](https://the-soulful-entrepreneur.beehiiv.com/p/8-simple-steps-grow-newsletter-50000-subscribers?utm_source=the-soulful-entrepreneur.beehiiv.com\\&utm_medium=newsletter\\&utm_campaign=8-simple-steps-to-grow-your-newsletter-to-50-000-subscribers)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nOk, Notion Builders non è una startup ma una piccola agenzia con solo due persone.\n\n​[Però sta guida sul lavoro asincrono può essere utile a noi, così come a tante altre realtà che vogliono diventare più produttive.](https://review.firstround.com/the-secret-to-an-in-sync-startup-ditch-your-meetings-and-try-an-asynchronous-culture?ref=refind)​\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nI creator producono contenuti e cercano di monetizzarli.\n\n​[E anche in questo caso, la guida è per le startup ma penso che tutti possano trovarla utile: soprattutto chi vuole imparare a convertire l’attenzione in denaro.](https://www.animalz.co/blog/bottom-of-the-funnel-thought-leadership/)​\n\n<br>\n\n"
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
    text: >+
      <Script async data-uid="a9380e8603"
      src="https://kit-sopravvivenza-creator.ck.page/a9380e8603/index.js" />


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
slug: a-scuola-di-produttivita-da-cal-newport
---
Ehi ciao 👋,

questo è il numero 35 del **Kit di Sopravvivenza per Creator**.

E oggi ti svelerò **3 lezioni di produttività che ho imparato da Cal Newport.**

<br>

***

**TL;DR**

*   A scuola di produttività da Cal Newport;

*   Una risorsa per la tua audience building;

*   Una risorsa per la tua produttività;

*   Una risorsa per la tua monetization.

**Il tempo di lettura previsto è:** 4 minuti e 30.

***

Ok, se ti appassiona la produttività di certo avrai sentito parlare di **Cal Newport**.

È un insegnante alla Georgetown University ma è anche uno scrittore, blogger e podcaster.

Io l'ho conosciuto grazie ad alcuni libri di non poca fama: "So good they can't ignore you", "Deep Work", "Digital Minimalism" e "A World Without Email".

Insomma, come avrai potuto intuire da questi titoli: è un **esperto di produttività**.

Lo conosco da anni, ma è solo in questi mesi che ho approfondito lo studio dei suoi insegnamenti.

E prima ancora di testare il suo sistema di produttività in totale, ho pensato di mettere in pratica solo alcuni **principi** che ne sono alla base.

E il risultato è stato strabiliante.

<br>

## **A SCUOLA DI PRODUTTIVITÀ DA CAL NEWPORT**

Ma facciamo un passo alla volta. Quali sono i principi che mi hanno colpito di più delle opere di cal?

*   L'importanza del Deep Work;

*   L'impatto degli strumenti sulla tua produttività;

*   Anche la comunicazione dovrebbe essere produttiva.

Ti parlerò un attimo di questi **concetti e di come li ho messi in pratica**, poi ti rivelerò il loro **impatto**.

Ci sei?

Possiamo iniziare allora.

<br>

### **L'IMPORTANZA DEL DEEP WORK**

Ok, partiamo dalle basi.

Cos'è il **deep work**?

Per fartela breve, è la capacità di lavorare su degli obiettivi, in sessioni di concentrazione lunghe e **senza interruzione**.

Quando prendi la tua task list, cominci ad affrontare i punti del giorno, indossi le tue cuffie (oppure no), escludi tutte le distrazioni e entri nel flow per 60-90 minuti, puoi essere fiero di te: hai realizzato una sessione di deep work.

Come potrai intuire però, riuscire a fare una sessione di deep work non è tanto semplice.

Perché il mondo è pieno di distrazioni, ci sono le notifiche, gli smartphone, i social e tutto quello che vuoi: un bel casino.

Quindi quale sarebbe la lezione? Che ti devi concentrare?

In realtà no, il fatto che per lavorare al meglio ti devi concentrare è una cosa ovvia.

La lezione è che **l'abilità di lavorare in deep work è rara**.

E il mondo esterno, dal canto suo, è sempre più invasivo, sempre più forte nel distrarci.

Così, con sempre più distrazioni e sempre meno persone in grado di lavorare in deep work, quelle poche persone in grado di lavorare in deep work avranno un **vantaggio competitivo sulle altre**.

E come come metto in pratica questa cosa?

Ogni mia giornata lavorativa è strutturata in **4 blocchi di deep work**: due da 90 minuti e due da 60.

<br>

### **L'IMPATTO DEGLI STRUMENTI SULLA TUA PRODUTTIVITÀ**

Ora, c'è una cosa importante da dire.

Lavorare in deep work non è un talento, non è qualcosa con cui nasci e che rimane stabile per tutta la vita.

È un'**abilità** e la puoi **allenare** di giorno in giorno, proprio come un muscolo.

Ma non dipende solo dall'allenamento, ci sono altre cose che puoi fare per facilitare le tue sessioni di deep work:

*   puoi modificare il tuo ambiente di lavoro;

*   puoi organizzare i tuoi strumenti di lavoro.

Basta poco per fare modifiche del genere.

Io, per esempio, ho un tipo di **cuffie apposta per il deep work** (di quelle che cancellano i rumori esterni ecc).

Inoltre, sfrutto la **funzione "Full Immersion"** di Mac e IOS per eliminare le notifiche all'avvio delle sessioni di lavoro.

E insieme a Beatrice ho strutturato l'intero workspace di [Notion Builders](https://www.notionbuilders.it/) per facilitare le sessioni di deep work.

<br>

### **ANCHE LA COMUNICAZIONE DOVREBBE ESSERE PRODUTTIVA**

La **comunicazione** merita un paragrafo a parte.

Per molto tempo, ho pensato che le **notifiche e-mail, di Whatsapp o Slack** fossero un prezzo da pagare inevitabile.

Quando collabori con altre persone è fondamentale restare in comunicazione e quindi le notifiche sono inevitabili.

Solo che mi sbagliavo.

"A world without email", in particolare, mi ha fatto capire che potevo **creare un flusso di comunicazione** (tra me e Beatrice) che supportasse il nostro lavoro invece di ostacolarlo.

E questo che significa?

Che gestiamo le **comunicazioni in modo asincrono**, su Notion, grazie a diversi processi di cui magari ti parlerò in un'altra newsletter.

Perché il nemico più infame del deep work è il **context switching** (cambiare scheda del browser, interruzioni dovute alle notifiche e tante altre distrazioni) e non è vero che non lo si può sconfiggere.

<br>

Insomma, come hai potuto leggere fin qui, ho cercato di implementare queste tre lezioni nella mia vita quotidiana e qual è stato il risultato?

Non mi sono **mai sentito cosi produttivo**.

E non si tratta solo di percezione ma anche di **risultati oggettivi**, misurati col numero di cose fatte e dalla loro qualità.

E questi risultati mi spingono a testare **l'intero sistema di produttività** creato da [Cal](https://calnewport.com/).

Lo vedo come un esperimento interessante e che potrei documentare in dettaglio da qualche parte.

Ti interesserebbe un contenuto di questo tipo?

Fammelo sapere con una **risposta a questa e-mail**, dai che sono curioso.

E direi che con questo è tutto, buona settimana e **beccati le risorse**.

