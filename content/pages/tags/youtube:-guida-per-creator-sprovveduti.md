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
title: "\U0001F9F0 kSC #31: youtube, guida per creator..."
colors: colors-a
date: '2023-03-26'
description: sprovveduti!
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nUna delle sfide che trovo più difficili riguardo il build in public è quella dei format.\n\nNon si può sempre pubblicare grafici dei tuoi risultati, statistiche ecc.\n\nDevono pur esistere altri format per fare Build in public, vero?\n\n[È proprio così ed eccone 8 che ti saranno utili.](https://kp.substack.com/p/here-are-8-unique-ways-to-build-in)\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nQual è la tecnica di produttività più potente?\n\nNon è il titolo di una puntata di Dragon Ball, è una domanda lecita.\n\n[E questa è la risposta.](https://www.nirandfar.com/timeboxing/)\n\n<br>\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nVuoi raggiungere risultati, vero?\n\nLo so, tutti vogliono farlo.\n\nSolo che per riuscirci hai bisogno di alcune cose, soprattutto di tempo.\n\n[Inoltre, avrai bisogno anche di un business model.](https://thedankoe.com/the-best-online-business-model-to-make-1-million-in-2023/)\n"
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
slug: 'youtube:-guida-per-creator-sprovveduti'
---
Ehi ciao 👋,

questo è il numero 312 del **Kit di Sopravvivenza per Creator**.

E oggi ti racconterò dei **3 errori che ho fatto nel creare il mio primo video su Youtube**.

***

### **TL;DR**

*   Youtube: guida per creator sprovveduti;
*   Una risorsa per la tua audience building;
*   Una risorsa per la tua produttività;
*   Una risorsa per la tua monetization.

Il **tempo di lettura** è di 4 minuti.

***

Ok, come (spero) avrai saputo, ho pubblicato da qualche giorno il [mio primo video su Youtube](https://www.youtube.com/watch?v=tZnICTt7ogo).

Diciamoci la verità, era necessario.

I **tutorial su Notion** sono difficili da scrivere (e da leggere), è molto meglio mostrare certe cose in **video**.

Inoltre, con Youtube, posso andare a risolvere un piccolo problema riguardo il mio **creator funnel**.

Ma questo non è il punto della newsletter di oggi.

Oggi ti voglio raccontare di **3 cose a cui dovresti fare attenzione nella creazione del tuo primo video su Youtube**.

<br>

## **YOUTUBE: GUIDA PER CREATOR SPROVVEDUTI**

Sono sempre stato del parere che fatto è meglio che perfetto.

Per questo, quando qualche settimana fa ho deciso di cominciare a pubblicare video su YouTube, mi sono buttato abbastanza "a caso".

Ho comprato un po' della strumentazione necessaria, ho preparato uno script e mi ho registrato.

L'idea su cosa pubblicare già c'era (LinkedIn mi aveva aiutato), un po' di competenze nel montaggio video le ho e nel corso di una giornata ho pubblicato il primo video.

Ora, ovviamente, questo primo video non è perfetto, anzi.

Ci sono state delle sbavature nel processo di creazione e alcune erano previste, altre no:

*   devi fare una ricerca, una che non fai per la newsletter;
*   fai attenzione allo script;
*   Youtube non si fida.

<br>

### **DEVI FARE UNA RICERCA, UNA CHE NON FAI PER LA NEWSLETTER**

Questo è il punto più importante.

E quello che non avevo proprio ipotizzato.

Il fatto è che i **video su YouTube non sono come le newsletter**.

C'è un tipo di ricerca che non è necessario fare per le newsletter e che invece è fondamentale per i video su YouTube.

Pensaci, come fai a vedere un video su YouTube?

Vai sulla piattaforma, cerchi quello che ti interessa, il motore di ricerca ti propone una lista di risposte e tu scegli quella che più ti aggrada.

E come fa un video ad avere un posizionamento in quella lista?

Perché, proprio come con la SEO di Google, vuoi che il tuo video finisca ai primi posti di quella lista, così le persone lo vedranno ecc.

E proprio come con la SEO di Google, devi creare il contenuto in modo tale che **rispetti i criteri di posizionamento previsti dall'algoritmo di YouTube**.

Quindi, devi fare una **keyword research**, devi dire le parole giuste nel corso del video, utilizzare gli **hashtag** adatti nella descrizione del contenuto e tante altre cose del genere.

Se non lo fai, il video avrà poche probabilità di finire nella prima pagina di YouTube.

Insomma, non è come una newsletter.

Alle mie newsletter ci accedono le persone che arrivano da LinkedIn (e da Youtube), il traffico è pilotato e non richiede ricerca.

Più attenzione porto da LinkedIn (o Youtube) e più lettori (o iscritti) ci saranno alla newsletter.

Insomma, è una bella differenza.

<br>

### **FAI ATTENZIONE ALLO SCRIPT**

Questo punto invece sapevo che era necessario, ma non pensavo avrebbe creato tanti problemi.

Mi aspettavo che **creare lo script** del primo video fosse più facile: mi bastava un elenco di punti che facesse da canovaccio per andare spedito.

Sbagliato.

Con uno script così strutturato, **ho provato a registrare il video per 4-5 volte e non ho avuto successo**.

Poi ho capito che era meglio **scrivere in dettaglio** cosa avevo intenzione di dire, l'ho fatto ed ho registrato.

Ma ho **fallito** di nuovo.

Perché questa volta non ricordavo cosa dovevo dire e mi perdevo.

Quindi ho riletto lo script e l'ho **capito**, l'ho reso parte del mio discorso senza recitarlo a memoria (o leggerlo) e le cose sono andate meglio.

Insomma, ho scritto lo script in dettaglio ma l'ho utilizzato quasi a braccio: un mix efficace.

<br>

### **YOUTUBE NON SI FIDA**

Di questa cosa non ne avevo manco idea.

Ho registrato e montato il video nel corso della stessa giornata, perchè mi sono ridotto all'ultimo con la deadline che mi ero posto: alle 18 il video doveva uscire.

E alle 17.45 vedo con orgoglio che la terza esportazione del video era andata bene.

Apro YouTube e comincio a caricare il video, scrivere la descrizione e al suo interno inserire i link vari.

Ma ecco che arriva il primo stop.

Per caricare un video più lungo di 10 minuti serve la **verifica dell'indirizzo e-mail**.

Ok, verifichiamola.

Procedo con l'inserire i link, ma **Youtube mi ferma di nuovo**: per poter inserire i link devo aver verificato la mia identità.

Posso farlo via telefono, ma parlo a telefono solo quando ordino qualcosa fuori.

Posso farlo caricando una foto del mio documento d'identità, ma non so manco dove sia.

Posso farlo con un'altra opzione che non ricordo, ma che era altrettanto improbabile.

Quindi che faccio?

Non inserisco link, sono le 18 e il video devo uscire, li inserirò in un secondo momento.

E ovviamente quel secondo momento è arrivato dopo 4-5 giorni.

<br>

Insomma, come puoi vedere la creazione di un contenuto dipende molto dalla piattaforma che scegli.

E si, lo so che è un'ovvietà.

Ma fino a quando non ci sbatti la faccia, non te ne rendi mai conto per davvero.

Spero che con questa newsletter però, ti risparmi questi errori e tu possa farne tesoro.

E direi che per oggi è tutto, buona settimana e **beccati le risorse**.

Daniele
