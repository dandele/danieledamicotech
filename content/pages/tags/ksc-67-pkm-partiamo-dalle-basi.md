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
title: "\U0001F9F0 kSC #67: PKM, PARTIAMO DALLE BASI..."
colors: colors-a
date: '2023-12-10'
description: così non facciamo confusione!
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
    text: "## **\U0001F465 La strada per i primi 10mila iscritti**\n\nLa strada per raggiungere i primi 10mila iscritti può essere oscura.\n\n​[Ma questa è una storia che può fare da guida per tutti noi.](https://www.opensourceceo.com/p/building-in-public-1?ck_subscriber_id=1870002162)​\n\n​\n\n## **\U0001F680 Preferisci raddoppiare oppure moltiplicare per 10?**\n\nMoltiplicare per 10, se le cose sono buone, vero?\n\nMa con la difficoltà, come si fa? Aumenta pure quella, vero?\n\n​[Beh, in realtà non è detto.](https://www.linkedin.com/posts/thatjoshspector_is-10x-easier-than-2x-benjamin-hardy-activity-7128033437461999616-phtA/)​\n\n​\n\n## **\U0001F4B8 Copy che converte**\n\nVuoi scrivere testi che convertano?\n\n​[Ecco una piccola guida per aiutarti.](https://www.stackedmarketer.com/the-crews-insights/the-dos-and-donts-of-writing-sponsor-copy-that-converts/?ck_subscriber_id=1870002162)​\n\n\n\n\n"
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
slug: ksc-67-pkm-partiamo-dalle-basi
---
In questo periodo penso spesso al mio **personal branding**.

Se la parte lavorativa delle mie attività è dedicata a Notion, processi e automazioni per aziende, cosa ne faccio del mio personal branding?

Lo limito ad un motore di attenzione per Notion Builders, oppure lo rendo qualcosa di diverso?

Ancora non ho preso una decisione, ma credo che seguirò la seconda strada.

E più o meno ho capito quali cambiamenti farò, ma questa non è la newsletter per parlarne.

Due cose te le posso dire però.

La prima è che presto vedrai cambiare alcune cose.

La seconda, invece, è che i cambiamenti sono collegati all'argomento della newsletter di oggi: il **knowledge management**.

​

**TL;DR**

*   PMK, partiamo dalle basi

*   La strada per i primi 10mila iscritti

*   Preferisci raddoppiare oppure moltiplicare per 10?

*   Copy che converte

**Il tempo di lettura previsto è**: 5 minuti

​

Ok, fermi un attimo, ma cosa sarebbe?

Diciamoci la verità, è una di quelle cose che più o meno tutti capiscono, ma nessuno riesce a definire per bene.

Hai presente no?

Di quelle che se per strada ti ferma qualche tiktoker a caso e ti chiede "ehi che cos'è il knowledge management?", te inizi a balbettare qualcosa di poco preciso, ma comunque giusto.

Più o meno.

E se poi il randomico tiktoker ti dovesse chiedere "E che cos'è il PKM?"

In tal caso, di sicuro lo manderesti a quel paese, lo so.

Ma visto che sono argomenti di cui parlerò spesso in futuro, è meglio chiarirli fin da da ora.

Così quando le prossime volte ne parlerò, potrò linkare a questa newsletter per farti trovare tutte le definizioni necessarie.

Quindi, oggi capirai queste tre cose:

*   cosa sono il knowledge management e il personal knowledge management?

*   cosa ti aiuta a fare il personal knowledge management?

*   in che modo ti può aiutare il personal knowledge management?

Pronto?

Iniziamo!

​

## **Knowledge Management e Personal Knowledge Management, che sarebbero?**

Hai presente il principio dell' "explain me like I'm five"?

È un principio ideato da **Richard Feynman**.

Di base, ti dice che se sei in grado di spiegare una cosa ad un bambino molto piccolo, allora significa che quella cosa l'hai capita.

E perché?

Perché per farti capire dal bambino, avrai dovuto capire prima di tutto tu la cosa in questione.

Avrai dovuto spiegarla con termini semplici, senza paroloni.

E poi avrai dovuto rispondere a tutti i "perché" con cui i bambini sono soliti aggredire gli adulti.

È un buon principio, cerco sempre di utilizzarlo quando studio qualcosa.

Solo che non vado in giro a cercare di spiegare cose ai bambini, sarebbe strano.

Faccio delle cose più moderne.

Chiedo a **ChatGPT** e **Notion AI**.

Eh si, vado su ChatGPT e scrivo questo semplice prompt "Sono un bambino della prima elementare, magari anche più piccolo. Voglio che mi aiuti a capire cos'è X".

E poi utilizzo lo stesso prompt, in un database Notion molto più strutturato e figo.

Un database che ho chiamato Knowledge Hub e di cui ti parlerò in futuro.

Comunque, ecco la risposta che l'intelligenza artificiale mi ha dato alla domanda riguardo il **knowledge management**.

"Certo, posso spiegarlo in modo semplice! Immagina che il "knowledge management" (gestione della conoscenza) sia come un grande armadio magico nella tua mente, dove puoi conservare e organizzare tutte le informazioni importanti che impari ogni giorno.

Quando impari qualcosa di nuovo a scuola, come ad esempio i fatti interessanti sugli animali o le regole della matematica, puoi metterlo nell'armadio magico della tua mente.

La gestione della conoscenza è come tenere tutto in ordine in questo armadio, in modo che tu possa trovare facilmente le informazioni quando ne hai bisogno.

Immagina anche di avere una bacchetta magica che ti aiuta a condividere queste informazioni con i tuoi amici. Quindi, se un amico ha bisogno di sapere qualcosa che hai imparato, puoi usare la tua bacchetta magica (la condivisione di conoscenze) per aiutarlo.

In breve, la gestione della conoscenza è come tenere traccia e organizzare tutte le cose interessanti che impari, in modo da poterle trovare facilmente e aiutare anche i tuoi amici a imparare cose nuove!"

Direi che è un ottimo inizio, in pratica fare knowledge management significa gestire le conoscenze.

Ma che differenza c'è con il **personal knowledge management**?

"Il "personal knowledge management" (PKM), o gestione personale della conoscenza, è come prendere quel grande armadio magico nella tua mente e organizzarlo in modo speciale solo per te.

In altre parole, è il modo in cui tu gestisci, organizzi e sfrutti le informazioni che impari in modo personale, per rendere la tua vita più facile e efficiente.

Immagina che tu abbia un quaderno segreto in cui scrivi le cose che sono davvero importanti per te, come i tuoi pensieri, i tuoi progetti e le tue scoperte.

La gestione personale della conoscenza è come tenere il tuo quaderno segreto in ordine, in modo che tu possa tornare a leggerlo quando ne hai bisogno e trovare facilmente tutte le tue idee speciali.

Quindi, mentre la gestione della conoscenza riguarda l'organizzazione delle informazioni in generale, il personal knowledge management è più specifico ed è come prendere il controllo delle tue idee personali e delle cose che sono importanti solo per te.

È come avere un diario segreto delle tue scoperte e pensieri!"

E devo essere sincero, le due risposte hanno senso.

In pratica, si tratta di separare due mondi.

Da un lato c'è la gestione della conoscenza indefinita e dall'altro quella personale.

Quella generale è regno delle aziende, con tutte le informazioni che devono gestire.

E quella personale è la tua, tutte le conoscenze che acquisisci giorno dopo giorno e che devi gestire in qualche modo.

E lo so, lo so che era tutto intuibile e magari già ne avevi una qualche idea, ora però è tutto più definito.

Vero?

​

## **Parliamo di PKM, cosa ti aiuta a fare?**

Ok, ora parliamo delle cose interessanti.

Perché dovresti cominciare a fare PKM?

Che vantaggi potresti ottenere?

Le 3 cose principali che puoi ottenere sono:

*   che riuscirai a **ricordare**

*   che riuscirai a **fare**

*   che riuscirai a **creare**

Insomma, quando inserisci un'informazione nel tuo sistema di PKM (che poi sarebbe il tuo cervello digitale) le puoi dare una nuova forma oppure la puoi spostare nel tempo.

Se hai bisogno di **immagazzinarla per il futuro**, puoi fare in modo che quando arriva il momento di doverla recuperare, tu possa farlo senza problemi.

Se hai bisogno invece di **utilizzare quell'informazione**, potrai trasformarla in un task e passare all'azione.

Infine, se hai bisogno di **creare qualcosa**, potrai prendere quell'informazione e collegarla ad altre informazioni, così da stimolare la tua creatività e creare qualcosa di nuovo.

Per fartela breve, il PKM ti può aiutare in queste 6 aree diverse:

*   **PMM** (memory management): ti aiuta a gestire quello che devi ricordare

*   **PIM** (idea management): ti aiuta a gestire le tue idee

*   **PWM** (writing management): ti aiuta a gestire quello che scrivi

*   **PPM** (productivity management): ti aiuta a gestire la tua produttività

*   **PSM** (skill management): ti aiuta a gestire le tue abilità

*   **PRM** (relationship management): ti aiuta a gestire le tue relazioni
    Dai, direi che ci puoi fare un sacco di cose!

​

## **E in che modo ti aiuta a farlo?**

Arriviamo alla parte pratica, in che modo un sistema di PKM ti può aiutare?

Questa è forse la parte più **incasinata**.

Perché è la parte in cui ci sono **centinaia di strumenti** che ti aiutano a gestire le tue informazioni.

E ci sono **centinaia di approcci**, metodi, framework che ti aiutano col modo in cui gestire le informazioni.

Hai presente il [Second Brain, lo Zettelkasten](https://danieledamico.tech/tags/ksc-66:-para-ppv-e-zettelkasten-qual-e-il-miglior-sistema-per-il-tuo-cervello-digitale/) e tanti altri metodi di cui ho parlato in passato in questa newsletter?

Ecco, quelli sono **framework** di PKM, ti aiutano con il modo.

Poi ci sono gli **strumenti**.

E qui abbiamo Notion, Obsidian, Mem, Tana e tutti gli strumenti di cui parlo.

Diciamoci la verità, inoltrarsi in questo mondo è rischioso.

Da una parte ci sono dei **vantaggi chiari**, ma sulla strada per arrivarci ci sono un sacco di trappole come la [produttività tossica](https://danieledamico.tech/tags/come-sopravvivere-senza-tool...in-3-mosse-\(+1\)), l'ottimizzazione eccessiva di uno strumento, la scelta di framework non adatti al nostro stile ecc.

Ed è proprio per questo che penso ci sia bisogno di qualcuno che ti aiuti nel percorso, non credi?

​

​

Ecco, direi che per oggi mi posso fermare.

Questa newsletter aveva lo scopo di scendere in dettaglio su un concetto che spesso risulta poco chiaro.

E porre le basi per i **nuovi sviluppi** dei miei contenuti.

Mai come in questo caso, mi piacerebbe sapere cosa ne pensi nel modo che più preferisci.

Puoi **rispondere con una mail**, oppure cliccare su uno dei **tre link qui sotto** ed esprimere un voto.

Detto questo, per oggi è tutto, buona settimana e beccati le risorse.

Daniele

​

PS:

Tutti quelli che lasciano un voto, in qualche modo, riceveranno un bonus e potranno esprimersi sul nuovo nome della newsletter!

<br/>
<br/>

## **Che ne pensi di questa newsletter?**

*   ​[👍 Mi è piaciuta molto!](https://hook.eu1.make.com/ktrkrhvgqmoxiya3wbj3tf5n42iiks7w?10_12_23_yay)​

*   ​[🤢 Meh](https://hook.eu1.make.com/ktrkrhvgqmoxiya3wbj3tf5n42iiks7w?10_12_23_nah)​

*   ​[👎 Non mi è piaciuta](https://hook.eu1.make.com/ktrkrhvgqmoxiya3wbj3tf5n42iiks7w?10_12_23_nay)
