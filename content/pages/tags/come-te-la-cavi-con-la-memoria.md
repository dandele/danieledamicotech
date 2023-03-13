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
title: "\U0001F9F0 kSC #29: Meeting notes efficaci"
colors: colors-a
date: '2022-12-18'
description: ESISTONO?
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nTutti usano ChatGPT ormai.\n\nChe sia per giocare o per pubblicare quel post in cui dicono di aver usato ChatGPT.\n\nMa se vuoi usarla per davvero, magare per creare la tua audience?\n\n[Allora dovresti leggere sta roba.](https://www.neatprompts.com/p/create-a-social-media-calendar)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nIl potere di ChatGPT ormai è noto a tutti.\n\nMa presto cambierà tutto.\n\n[Presto arriverà la sua evoluzione, prima di quanto pensi.](https://www.heise.de/news/GPT-4-is-coming-next-week-and-it-will-be-multimodal-says-Microsoft-Germany-7540972.html)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nVuoi monetizzare?\n\nAllora non dovresti considerare solo come vendere di più.\n\n[Dovresti considerare anche queste cose.](https://www.thetilt.com/business-operations/personal-finance-for-creators)\n\n"
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
slug: come-te-la-cavi-con-la-memoria
---
![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/36d499c7-f6d8-47f1-8e68-31b7b0dd71dd/Untitled.png)

Guarda l’immagine qui sopra.

È un post che ho pubblicato circa 3 mesi fa.

È stato visto quasi 1200 volte ed i miei follower sono quasi 1200 su Linkedin.

Ma sai una cosa?

Scommetto che non lo hai visto.

Oppure, se lo hai fatto, scommetto che non lo ricordi.

---

## **TL;DR**

- Non hai idea di quante persone NON vedano i tuoi contenuti
- Una risorsa per la tua audience building
- Una risorsa per la tua produttività
- Una risorsa per la tua monetization

**Il tempo di lettura previsto è**: 5 minuti.

---

Ehi ciao 👋,

questo è il numero 215 del **Kit di Sopravvivenza per Creator**.

Ed oggi ti racconterò di **come riutilizzo i miei vecchi contenuti**.

Ok, so so cosa stai pensando.

Stai pensando che riutilizzare contenuti vecchi non sia produttivo.

Perché il gioco non vale la candela.

Che se non hai niente di nuovo da dire, allora è meglio stare in silenzio.

E cosa accadrebbe, poi, se qualcuno ti sgamasse?

Ecco, io credo che, se hai chiari gli obiettivi ed il processo, nessuno ti scoprirà a riutilizzare vecchi contenuti.

Purtroppo però, in tanti pensano che riutilizzare vecchi contenuti sia sbagliato e quindi, quando la creatività finisce, perdono un’occasione importante per far sentire la propria voce.

Ed il motivo è uno solo.

## NON HANNO IDEA DI QUANTE PERSONE NON VEDANO I LORO CONTENUTI

Basta fare qualche **calcolo**.

Prendi un canale, quello che più utilizzi per pubblicare i tuoi contenuti.

Quante sono le persone che li ricevono? 10? 100? 1000? Di più?

Non importa il numero preciso.

Importa il fatto che le persone che consumano per davvero i tuoi contenuti sono solo una percentuale di quelli che li ricevono.

È la differenza tra Open Rate delle e-mail e lettura effettiva (magari interpretabile dal numero di click).

La differenza che c’è tra le Impression di un post Linkedin ed i commenti/like/click sul link.

Insomma, la differenza tra esposizione e consumo.

Poi ci sono tante altre variabili di mezzo.

Quanto spesso pubblichi? Quanto spesso cambia il numero di persone che ricevono i tuoi contenuti?

E le persone che poi non ricevono i tuoi contenuti direttamente?

Insomma, un **casino**. 

Justin Welsh però la spiega bene in [questo tweet](https://twitter.com/thejustinwelsh/status/1571122303009804288):

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6de4fb00-6b14-472e-8e0f-08dbdb8c2655/Untitled.png)

Ora, non so quanto siano affidabili i numeri che ha dato.

Ma Justin punta a dimostrare una cosa.

E dopo aver parlato con decine e decine di creator (o aspiranti tali) in questi mesi, ho capito perché così tanto non riutilizzano i vecchi contenuti:

- Perché non sanno quali contenuti abbia senso pubblicare di nuovo;
- Perché vogliono pubblicare i vecchi contenuti, ma non sanno come modificarli;
- Perché non sanno come rendere quei contenuti rilevanti al periodo di nuova pubblicazione.

Ed io oggi voglio mostrarti come riesco a risolvere io questi tre problemi, magari ti sarà d’ispirazione.

Ecco il mio **processo**:

### COME TROVO I CONTENUTI DA RIPUBBLICARE

Hai presente tutti i numeri di cui ti ho parlato prima?

**Impression, Open Rate, Click Rate ecc?**

Tutte queste cose sono dati.

Dati che aiutano a capire quali contenuti hanno generato più interesse e quali no.

E qualsiasi sia il canale che utilizzi, potrai trovare con facilità dati di questo tipo.

Mettiamo il caso che utilizzi, come me, Linkedin.

Ogni post Linkedin viene misurato con:

- Impressions;
- Commenti;
- Likes;
- Condivisioni;
- Click su eventuali link.

E basta poco per capire quale contenuto è più interessante di altri.

Di solito un contenuto che attira tanti commenti (o condivisioni) e tante impression è un contenuto che interessa.

E lo è ancor di più se attira tanti **click sul link** che hai condiviso (e se magari quello invita ad iscriversi a qualcosa).

Insomma, la regola che applico è semplice: se un contenuto ha fatto tanti commenti, tante impression o tanti click allora in quel contenuto c’è qualcosa di **interessante**.

Ed indovina il posto dove applico questa regola? Su Notion, che ti aspettavi?

Tramite qualche magia riesco ad esportare i dati dei miei post Linkedin su un **database Notion**.

Lì li filtro per vedere i contenuti che più rispettano la regola che ti ho detto poco fa.

Et voilà, capisco quale contenuto potrei riutilizzare.

Ecco un’immagine del database.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7b2dc450-6970-487a-829e-346b9f122565/Untitled.png)

### COME RINNOVARE I VECCHI CONTENUTI

Qui la creatività esplode.

Ci sono **decine di modi** per poter riutilizzare vecchi contenuti.

I modi che che preferisco io sono questi:

- **Cambio il formato del contenuto**: questo è il modo che la maggior parte delle persone utilizza quando pubblica da un canale all’altro.
    
    L’esempio migliore è quello del **thread di Twitter** che finisce su **Linkedin come carosello**.
    
- **Cambio le parole (in particolare l’hook)**: penso tu sappia cosa penso degli **hook** di un post.
    
    Sono la parte più importante di un contenuto e puoi generarne decine per la stessa idea. 
    
    Prima di pubblicare un post io ne scrivo più di uno e scelgo quello che mi incuriosisce di più. 
    
    Gli altri però non li cancello perché li **riutilizzo in futuro**. 
    
    E per quanto riguarda il resto del contenuto, lì mi diverto a fare la “parafrasi” della vecchia idea (oppure lo lascio fare [all’AI](https://chat.openai.com/auth/login?next=%2Fchat)).
    
    Ecco un esempio.
    

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/920dbd7a-ef49-47ec-b70c-f5165ea8cea5/Untitled.png)

### COME RENDO I CONTENUTI RILEVANTI

Qui la questione è molto **semplice**.

Anzi no.

O forse si.

Il fatto è che qui entrano in gioco cose come la **strategia**, il tuo **funnel da creator** e tante cose che sembrano complesse ma che poi non lo sono.

Te la faccio semplice per evitarti troppi scazzi, è pur sempre domenica.

I contenuti che pubblico sono sempre e comunque parte di una **strategia**.

Ed in quanto tali sono coerenti tra loro, per forza di cose.

Se un contenuto Linkedin ha successo, allora lo faccio evolvere in newsletter o lo ripubblico su Linkedin dopo qualche tempo.

La strategia è verticale in termini di funnel ed orizzontale in termini di canali.

Quindi se hai definito il tuo **focus**, il tuo **target** e li tratti con disciplina puoi stare certo che i contenuti che hai pubblicato 3 mesi fa saranno comunque **rilevanti**.

Ecco, questo è il processo che utilizzo per pubblicare più volte uno stesso contenuto.

Lo trovo, capisco come modificarlo e prima ancora di crearlo mi sono accertato che fosse coerente.

Ora, non ti dico che questo processo sia il migliore e non è detto che tu debba seguirlo.

Ma ti posso dire che per me, almeno per ora, **funziona**.

Vuoi aiuto con un processo simile? 

Magari nell’implementarlo su Notion?

Possiamo fare una call, clicca sul **pulsante qui sotto**!

E direi che per oggi è tutto, ti auguro buona settimana e **goditi le risorse**.

Daniele