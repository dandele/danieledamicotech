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
title: "\U0001F9F0 kSC #22: TASK MANAGER COME..."
colors: colors-a
date: '2023-01-15'
description: VESTITI SU MISURA!
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
slug: task-manager-come-vestiti-su-misura
---
Oggi voglio che utilizzi un po' di immaginazione.

Voglio che ti immagini a casa tua.

Dai, è uno sforzo minimo visto che forse già sei a casa tua.

Voglio che però ti immagini di venerdì sera, un venerdì sera di quelli di puro relax.

Sai che domani non dovrai fare nulla, sono le 22.15 e ti puoi rilassare.

Prendi il cellulare, apri qualche social e cominci a passare da un post all'altro.

Cosa stai utilizzando per farlo? Il pollice vero?

Perché non usi l'Apple Pencil?

***

**TL;DR**

*   Task manager come vestiti su misura

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 3 minuti e 40.

***

Ehi ciao 👋,

questo è il numero 243 del **Kit di Sopravvivenza per Creator**.

E oggi ti svelerò **come rendere il task manager una vera arma di produttività**.

<br>

La risposta è ovvia.

Non usi l'Apple Pencil perché non è lo strumento adatto per girovagare su Instagram.

Il pollice serve a passare da un post all'altro, l'Apple Pencil invece serve per fare cose carine sull'ipad.

Ora però ho una domanda per te.

Perché non fai questa distinzione anche con il tuo task manager?

<br>


## **COME RENDERE IL TASK MANAGER UNA VERA ARMA DI PRODUTTIVITÀ**

Il fatto è che il task manager è proprio come un vestito.

Non ti puoi accontentare di qualcosa di standard: è qualcosa che deve essere adatto a te e solo te.

E proprio come esistono decine di fisici diversi per un vestito, così esistono decine di diversi approcci al task manager.

E meriti un task manager che sia adatto al tuo approccio.

Mi sono reso conto della cosa qualche anno fa, quando ho scoperto 3 cose.

3 cose che non rientravano nell'uso canonico di un task manager ma che, dopo averle implementate nel mio task manager, hanno moltiplicato per 10 la mia produttività.

Eccole qui:

-   C'è differenza tra Do date e Due date;
-   Non esistono solo le priorità di Eisenhower; 
-   Non esistono solo le task list;

Ed oggi ho deciso di parlartene e mostrarti come le ho implementate.

Cominciamo subito.

<br>

### **C'È DIFFERENZA TRA DO DATE E DUE DATE**

Sembra così ovvio, eppure l'ho scoperto solo da poco.

Nel tuo task manager non dovresti utilizzare solo la due date, la data in cui è previsto che tu concluda il task, ma anche la do date.

Che differenza c'è?

Beh, la do date è la data in cui tu prevedi di fare il task.

La due date invece è la data di consegna, ma ti consiglio di utilizzarla per tutti i task.

Altrimenti rischi di renderla una fake due date, una data indicativa è che poi non rispetti per davvero.

Limita il suo utilizzo a quelle situazioni in cui ci sono delle conseguenze reali e dirette nella tua vita (o lavoro): pagamento dell'affitto o di alcune bollette, fine di progetti lavorativi importanti, uscite della newsletter ecc.

Per tutti gli altri task, non serve una due date, tutto quello di cui hai bisogno è una do date.

E non è difficile implementare la cosa.

Puoi cambiare qualche etichetta sul tuo task manager di fiducia, oppure se usi Notion puoi creare una nuova proprietà nel tuo database dei task.

La proprietà deve essere di tipo Data ovviamente è la chiami Do Date.

Poi la duplichi e chiami la seconda proprietà Due Date.

E il gioco è fatto.

<br>

### **NON ESISTONO SOLO LE PRIORITÀ DI EISENHOWER**

Alta, media e bassa.

Questi sono i tipi di priorità che più spesso ci ritroviamo ad assegnare ai nostri task.

È un sistema semplice eh, ma poco efficace.

Perché se non lo gestisci bene, presto ti ritrovi con tutti i task in priorità alta.

E quando tutto ha una priorità, allora niente ha una priorità.

E così cerchiamo una soluzione, un'alternativa a questo sistema di priorità così semplice.

Il risultato?

La matrice di Eisenhower, che di sicuro conosci.

Solo che come implementi una matrice in un task manager?

Cambi le opzioni del campo proprietà in quelle della matrice?

In questo modo non hai fatto altro che cambiare la facciata del vecchio sistema, non hai risolto il problema.

Per fortuna c'è un altro modo, almeno su Notion.

- Crei 4 proprietà di checkbox: ognuna che corrisponde ai quadranti della matrice.
- Crea una proprietà formula: questa assegnerà la priorità in funzione dei checkbox che hai selezionato.

Io utilizzo proprio quests struttura per gestire le priorità, anche se non uso la matrice di Eisenhower ma la matrice del 10k Value di Khe Hy, il principio di funzionamento è lo stesso.

Lo scopo è evitare che tu decida sulla complessità e che ti concentri su piccole decisioni del tipo si/no.

<br>

### **NON ESISTONO SOLO LE TASK LIST**

Questa è una tecnica che ho scoperto mentre cercavo di rendere la mia esecuzione di task più consapevole, ne abbiamo parlato qualche newsletter fa.

Si tratta di integrare task manager e journal e si chiama interstitial journaling. 

Più che una cosa da task manager è una cosa che puoi implementare su tool come Obsidian, Roam Research oppure, ovviamente, Notion.

Perché è necessario che tu abbia una daily page a disposizione, che è una cosa che hai sempre a disposizione su Obsidian e Roam, mentre su Notion te la puoi costruire.

In quella daily page, che ovviamente avrà come titolo la data odierna (su Notion puoi utilizzare il comand @today per riuscirci), potrai inserire la tua task list del giorno.

E poi potrai inserire un elenco puntato.

Uno in cui, ogni volta che hai una pausa, fai un piccolo brain dump e scrivi le tue preoccupazioni, come stai è quello a cui stai pensando.

Una cosa veloce ed immediata. 

E ogni entrata, puoi farla iniziare su Notion col comando @now per inserire l'orario in cui stai scrivendo.

<br>

Ecco qui, direi che per oggi è tutto.

Come puoi notare, c'è un motivo per cui adoro Notion: non importa quello che vuoi fare e quanto sia particolare la tua esigenza di utilizzo, con Notion puoi costruire un sistema per metterla in atto.

E chiariamoci, non so se queste tecniche miglioreranno anche la tua di produttività, ma ti posso garantire che hanno migliorato la mia di produttività.

Ti interessa poter implementare queste cose anche sul tuo spazio Notion?

Allora ti lascio un pulsante qui sotto, cliccaci e sarò felice di aiutarti,

Detto questo, buona settimana e beccati le risorse.