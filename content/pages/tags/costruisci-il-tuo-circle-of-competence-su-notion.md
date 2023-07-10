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
title: "\U0001F9F0 kSC #46: NIENTE PIÙ KIT QUOTIDIANO..."
colors: colors-a
date: '2023-06-04'
description: ecco perché
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
      - label: "UN DATABASE = +365 RISORSE \U0001F4DA"
        altText: ''
        showIcon: true
        icon: arrowRight
        iconPosition: right
        style: primary
        type: Button
        elementId: annual_review_button
        url: 'https://danieledamico.gumroad.com/l/yearly-kit-release'
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
    text: "## **\U0001F465 UNA RISORSA PER FARE AUDIENCE BUILDING**\n\nEssere un creator/avere un personal brand richiede parecchie energie.\n\n​[Ma quanto può essere di impatto sulla tua vita?](https://www.timstodz.com/how-to-use-your-personal-brand-to-generate-wealth/)​\n\n<br>\n\n## **\U0001F680 UNA RISORSA PER LA TUA PRODUTTIVITÀ**\n\nTantissime persone indossano ormai dispositivi che misurano la loro attività fisica e salute.\n\n​[Ma se ci fossero dispositivi che misurano la tua produttività?](https://www.trypylot.com/?ck_subscriber_id=1121223563)​\n\n​\n\n## **\U0001F4B8 UNA RISORSA PER LA TUA MONETIZATION**\n\nI corsi sono uno dei metodi più diffusi, ad oggi, per monetizzare.\n\n​[Ma come si crea un corso?](https://creatorscience.com/online-course/)​​\n"
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
slug: costruisci-il-tuo-circle-of-competence-su-notion
---
Ehi ciao 👋,

questo è il numero 368 del **Kit di Sopravvivenza per Creator**.

E oggi ti parlerò del **perché questa newsletter non avrà più il formato quotidiano.**

<br>

***

**TL;DR**

*   Kit di Sopravvivenza per Creator: niente più daily newsletter;

*   Una risorsa per la tua audience building

*   Una risorsa per la tua produttività

*   Una risorsa per la tua monetization

**Il tempo di lettura previsto è:** 5 minuti.

***

<br>

Quasi un anno fa, giorno più giorno meno, ho cominciato a pubblicare questa newsletter.

Era uno dei miei **sogni** rimasto nel cassetto per troppo tempo e, dopo aver ottenuto un bel po' di validazione sul formato e sui contenuti, ho deciso di buttarmi e lanciarla.

Doveva essere una newsletter in cui fornivo ogni giorno una risorsa utile per i creator e la domenica (l'edizione settimanale) doveva fornirne tre.

**L'all you can eat delle risorse per creator (e non solo).**

So che è successo un anno fa perché ho contato i giorni e le newsletter.

E l'ho fatto grazie alla newsletter quotidiana andata avanti fino a qualche giorno fa, fino al numero 365.

E perché?

Quali fattori ho valutato per prendere questa decisione?

Oggi te li spiego, magari ti potranno essere utili.

<br />

## **COME FERMARTI QUANDO VAI DI CORSA**

Quando fai qualcosa per tutti i giorni succedono cose.

Ottieni dei dati importanti.

Ed è importante interpretare questi dati per decidere i prossimi passi del tuo operato.

Ecco quali fattori che ho considerato per **eliminare il formato quotidiano**:

*   Curiosità o automatismo? La differenza è sottile

*   Divertimento o disciplina? La differenza è sottile

*   Rumore o valore? La differenza è enorme

Ora te ne parlo in dettaglio.

​

### **CURIOSITÀ O AUTOMATISMO? LA DIFFERENZA È SOTTILE**

Partiamo da questo punto, la questione più semplice.

Ho cominciato a pubblicare questa newsletter nel formato quotidiano per una sfida con me stesso.

L' obiettivo era quello di **creare qualcosa, tutti i giorni per un anno.**

Mi avrebbe insegnato tante cose sui lettori e su di me.

E soprattutto mi avrebbe insegnato tante cose sulla creazione di contenuti.

E ci sono riuscito, dopo tantissime iterazioni ho trasformato un processo creativo in qualcosa di automatico.

Cosi tanto automatico che non soddisfa più la mia curiosità.

Ho scomposto il concetto di newsletter, l'ho trasformato in un tweet che fa selezione, con la libertà di condividere quello che preferisci fregandotene che i link piacciano o meno alla piattaforma.

E cosi riuscivo a **raggiungere più obiettivi**.

Innanzitutto, riuscivo a dare al mio lettore il minimo carico informativo possibile.

Inoltre, riducevo lo sforzo creativo anche per me, il creatore della newsletter.

Ma per riuscire a fare sta cosa, dovevo **plasmare il processo creativo**, rendendolo adatto al meglio alle mie esigenze.

All'inizio scrivevo ogni newsletter nel giorno stesso in cui usciva, mi svegliavo un'oretta prima, selezionavo, scrivevo e pubblicavo entro le 7 di mattina.

Poi il processo è cambiato (perché sono cambiate le mie abitudini e anche la mia vita) e quindi ho cominciato a preparare le newsletter in batch e programmarle.

Nelle sue ultime iterazioni, il processo durava un paio di ore per una settimana circa di pubblicazione.

Tutto in un unico blocco di il lunedì mattina.

Solo che è diventato così automatico che potrei andare avanti per anni senza perdere neanche una giornata.

Ma a quale scopo?

​

### **DIVERTIMENTO O DISCIPLINA? LA DIFFERENZA È SOTTILE**

Quando l'atto creativo non è più difficile, diventa **noioso**.

Non so te, ma io funziono così.

Quando una sfida mi attira per la sua difficoltà, mi ossessiona e non sono soddisfatto fino a quando non l'ho risolta.

E la questione del "processo sostenibile" di cui ti ho parlato al punto precedente, era proprio una sfida di questo tipo.

Una volta che l'ho conclusa, non è più divertente ed è diventato prioritario per me capire altre cose.

Ho dovuto capire quali fossero i pro e i contro di proseguire.

Da un lato i **vantaggi**: continuare a raccogliere dati sui gusti dei lettori, continuare ad avere uno spazio quotidiano per eventuali sponsorship, continuare a stare sempre presente nel loop dei contenuti ecc.

Ed ho considerato gli **svantaggi**: noia per me e per il lettore (ma ne parleremo al punto successivo), blocchi di tempo che potrei riservare ad altro ecc.

E gli svantaggi si sono rivelati più dei vantaggi.

​

### **RUMORE O VALORE? LA DIFFERENZA È SOTTILE**

E arriviamo quindi a questo punto, quello più importante.

Alla base di una newsletter di selezione (come quella quotidiana e in parte questa) deve esserci una priorità secondo me, la più importante: **creare valore.**

E se non crei valore, allora crei rumore.

Perché diciamoci la verità, **di contenuti ne è pieno il mondo** e per quanto tu possa cercare di dare il tuo contributo, è importante capire se quel contributo crea valore oppure si disperde nel mare di contenuti che tutti noi consumiamo ogni giorno.

E qui i numeri parlano chiaro.

Più di un lettore mi ha rivelato che quelle newsletter quotidiane finivano automaticamente in una cartella specifica.

Che significa?

Significa che il valore nella selezione c'era, cosi tanto dal creare una cartella specifica su Gmail e attingere alle risorse condivide, ma non abbastanza da prendere azione subito.

Che è un problema che ho riscontrato in tante selezioni.

Ora, non so per te, ma **questo per me è rumore e non è valore.**

​

​

Ora però di sicuro ti starai facendo una domanda.

E ora?

Ora il Kit resterà, ma solo nel **formato settimanale** (quello che stai leggendo).

Il processo creativo che ho ottimizzato e reso automatico avrà nuovi obiettivi, su cui non ti faccio spoiler.

**E tutte le risorse che per un anno ho inviato tutti i giorni?**

Questa è la parte interessante, quella che ti porterà a **cliccare sul pulsante qui sotto (almeno spero).**

Tutte le risorse che ho pubblicato fanno parte di un mio database su Notion.

E non sono 365, sono molte di più.

Sono suddivise per categorie, con relativi dettagli ecc.

**E quel database non sparirà, resta vivo per il mio utilizzo e anche per il tuo.**

Se finora hai ricevuto la newsletter quotidiana, puoi accedere a tutti i link recuperando l'e-mail, salvando il link e tanti altri casini.

Se invece sei iscritto solo alla newsletter settimanale, certe risorse non le hai mai viste.

Quindi ho deciso di prendere il database, con tutte le risorse e dartene l'accesso.

In pratica, un anno di selezione, tutta disponibile oltre questo pulsante qui sotto.

E continuerà a crescere, fidati.

Il prezzo per l'accesso al database non è fisso, dopo i primi acquisti aumenterà a blocchi, quindi **ti consiglio di fare veloce**.

E detto questo, buona settimana e beccati le risorse.

Daniele

