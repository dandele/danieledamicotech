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
title: "\U0001F9F0 kSC #64: Come sopravvivere senza tool..."
colors: colors-a
date: '2023-11-19'
description: in 3 mosse (+1)
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
40 ore (o più) a settimana per il lavoro.

8 ore (o poco meno) al giorno per dormire.

Altre 2-3 ore per il cibo.

Qualche altra ora in viaggio, per lo sport ecc.

Diciamoci la verità, quando si parla di controllo del nostro tempo è difficile essere soddisfatti perché c’è sempre qualcosa che cerca di sottrarci il controllo.

E messa in questo senso, è normale che alcune persone vadano in fissa con la **produttività**, o sbaglio?

Si tratta pur sempre di un tentativo per riprendere il controllo del nostro **tempo**.

Con la produttività cerchiamo di ottenere il meglio dal tempo che abbiamo, di massimizzare lo sforzo ecc.

E come lo facciamo?

Con gli strumenti, con tool tipo Notion e Obsidian.

Ma sono necessari?

Hai davvero bisogno di Notion per essere più produttivo?

Hai davvero bisogno di Obsidian?

Hai davvero bisogno di uno degli altri tool che ci sono In commercio?

**Cosa accadrebbe se non ci fossero questi strumenti? Riusciremmo a sopravvivere?**

***

**TL;DR**

*   Come sopravvivere in un mondo senza tool?

*   Riutilizzare i vecchi contenuti, con l’AI;

*   Guida rapida al monk mode;

*   Gli errori che insegnano.

**Il tempo di lettura previsto è**: 4 minuti

***

Tutto dipende da come li utilizzi.

Se passi il tuo tempo a **ottimizzare il tuo spazio Notion**, senza poi utilizzarlo per migliorare il tuo lavoro, allora non lo stai usando per produttività.

È diventato solo il tuo nuovo giocattolo.

Qualcosa con cui procrastinare, avendo la scusa di essere più produttivo.

In tal caso, sei finito nella **produttività tossica**, sei nelle sabbie mobili.

Sei diventato un productivity bro (oppure sis, o che ne so) e passi il tempo alla ricerca di hack di produttività su Twitter, riorganizzando in modo ossessivo il tuo tool preferito.

Per fortuna però puoi cambiare, ti puoi salvare.

Ti basta guardare alla produttività per quello che è nella sua forma piu pura.

Un insieme di principi che ti permettono di prendere il controllo del tuo tempo, senza che tu dipenda da uno specifico tool.

E i principi in questione sarebbero questi:

*   devi sapere cosa fare

*   devi sapere quando farlo

*   devi poter pianificare

Continua a leggere, ti spiegherò meglio cosa intendo.

​

## **Devi sapere cosa fare**

Partiamo da questo principio.

È importante sapere cosa devi fare, visto che lo devi fare.

E come fai a saperlo senza che ci siano Notion, Obsidian o quel che ti pare a dirtelo?

Con un’ **obligations list**.

È una lista di tutte le cose in cui tu hai delle responsabilità da adempiere: il lavoro, la famiglia, le relazioni ecc.

In pratica, stiamo parlando delle famose **Aree** del Second Brain di Tiago Forte.

Devi avere sempre chiaro in mente quali sono queste aree e quali sono le tue responsabilità, se riesci a ricondurre le tue attività a questi punti è tutto più semplice.

E potresti non avere mai bisogno di alcun tool.

Sono serio, ti basta anche una **lista su un foglio di carta a caso**.

Fai la lista sul foglio di carta e poi te lo porti con te.

Così sai sempre cosa devi fare, perché hai bene in mente le responsabilità che devi coprire.

​

## **Devi sapere quando farlo**

Ok, in questo caso bisogna fare un po’ di attenzione alla semantica.

Perché questo principio si riferisce all’utilizzo di un **calendario**.

Che in un certo senso è un tool, ma non nei termini che vogliamo evitare (cioè non parliamo di calendario tipo [Akiflow](https://danieledamico.tech/tags/sistemi-non-bastano/), Cron, Google Calendar ecc.).

Parlo più del calendario classico.

Una lista dei tuoi impegni con il relativo orario in cui avvengono.

E hai tanto bisogno di un calendario.

Anche quando andavo all’università avevo bisogno di un piccolo calendario che mi dicesse quali lezioni frequentare, quando e dove.

Utilizzare la nostra memoria per conservare certe informazioni è uno spreco.

E anche in questo caso, non è necessario che tu utilizzi per forza un qualche tool digitale per gestire il tuo calendario.

Puoi anche prendere appunti su sticky note e attaccarli al frigorifero.

Non conta il modo, conta solo che tu sappia quando devi fare quello che devi fare.

​

## **Devi poter pianificare**

Passiamo la maggior parte del nostro tempo a pensare al futuro, oppure al passato.

E per evitare una cosa del genere, ci sono tante cose da fare, non ne basta solo una.

Questo principio però potrebbe essere una delle soluzioni più di impatto.

Tutto quello che devi fare è **sederti e organizzare le tue cose**.

Non basta che tu lo faccia una volta sola però, devi farlo con frequenza regolare.

L’ideale è che tu lo faccia ogni **tre mesi, ogni settimana e ogni giorno**.

E che nel corso di queste sedute, cerchi di pianificare le attività che devi fare fino alla prossima seduta.

Come per gli altri principi, non serve che utilizzi alcun tool in particolare, ti basta carta e penna.

Ma se c’è una cosa importante da fare in questa fase allora si tratta di riuscire a **saltare tra i diversi livelli di pianificazione con la giusta flessibilità**.

Cioè?

Nell’aggiornamento settimanale, per esempio, devi considerare le cose pianificate nell’aggiornamento trimestrale.

E nell’aggiornamento quotidiano, devi tenere conto di quelli settimanali, che a loro volta tengono conto di quelli trimestrali.

In questo modo, le tue attività quotidiane saranno collegate ai tuoi progetti trimestrali.

Sarà tutto più coerente, fidati di me.

​

E ti dirò una cosa.

Questi tre principi, si affiancano a [quello di cui ti ho parlato settimana scorsa](https://danieledamico.tech/tags/63-ksc-crea-il-tuo-diario-di-sistemi-personali...su-notion-\(o-dove-vuoi\)).

Metti insieme queste 4 cose e riuscirai a essere più produttivo, senza fissarti sul singolo tool oppure sulla singola tattica.

E detto questo, per oggi è tutto, buona settimana e **beccati le risorse**!

Daniele
