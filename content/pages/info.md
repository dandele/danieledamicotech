---
title: About
layout: PageLayout
colors: colors-a
backgroundImage:
  url: /images/Midnight-City-c404f5b8.webp
  backgroundSize: cover
  backgroundPosition: center
  backgroundRepeat: no-repeat
  opacity: 75
sections:
  - elementId: ''
    colors: colors-f
    backgroundSize: full
    text: "Ehi ciao, sono **Daniele D'Amico**.\n\nSono nato su un piccolo pianeta nel sistema solare ed è lo stesso in cui vivo ancora oggi.\n\nDopo aver lavorato per un paio di anni come freelancer e nel mondo delle startup, ho fondato la prima agenzia di consulenza Notion in Italia: [**Notion Builders**](https://www.notionbuilders.it/).\n\nQuando non leggo libri, creo contenuti sul web (in particolare su **Linkedin**).\n\nQuesto testo deve essere breve, se vuoi dettagli ulteriori **scorri la pagina verso il basso** \U0001F447\n"
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-16
          - pb-12
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
    type: HeroSection
    media:
      type: ImageBlock
      url: /images/Daniele D'Amico-c0ef85eb.webp
      altText: altText of the image
      caption: Caption of the image
      elementId: ''
  - type: DividerSection
    styles:
      self:
        width: wide
        padding:
          - pt-8
          - pb-8
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
        borderStyle: solid
  - type: TextSection
    colors: colors-f
    elementId: ''
    variant: variant-a
    title: Alcune cose su di me
    subtitle: null
    text: "Mi è sempre piaciuto costruire cose digitali e poi scomporle, analizzarle per comprenderle fino all'elemento più piccolo.\n\nSe c'è un tratto comune nella mia carriera direi che è proprio questo della costruzione e comprensione di cose.\n\nCon il senno di poi, risulta evidente in tutte le mie attività.\n\n1️⃣ Fin da quando a 18 anni ho creato, con alcuni miei amici, il mio primo blog e l'ho fatto crescere fino ad avere un certo seguito.\n\n2️⃣ Poi all'università, prima con la laurea in Scienze della Comunicazione e poi con quella specialistica in Corporate Communication and Media, scomponevo ogni concetto nei suoi elementi essenziali, li comprendevo appieno e poi li riutilizzavo, come lettere di un alfabeto, per formulare ragionamenti.\n\n3️⃣ E nel mondo del lavoro, prima come consulente freelancer di Digital Marketing e poi di UX Design (con focus sulla user research) aiutando alcuni business ad avviare la loro presenza nel mondo digitale e, dopo aver abbandonato il mondo della consulenza, oggi nel ruolo di Product Manager per una startup di Cyber Security che aiuto nel creare i nuovi sviluppi dei suoi prodotti digitali. Esperienza che mi ha portato, negli ultimi mesi, ad affacciarmi al mondo del product management, grazie anche al Master in Product Management di Edgemony.\n\n4️⃣ Infine nel tempo libero che passo in una miriade di attività solo sconnesse in apparenza (il fil rouge è evidente solo a chi sa guardare bene):\n\n\U0001F7E2 usare Notion non solo per prendere appunti ma per creare automazioni e mini-prodotti che mi migliorano la vita;\n\n\U0001F7E0 creare siti web con piattaforme come Netlify e framework come Hugo solo per il gusto di comprenderli;\n\n\U0001F6E1 leggere libri e newsletter a tema product management e startup per poi rilassarmi la sera leggendo qualche romanzo fantasy;\n\n\U0001F3A7 ascoltare podcast;\n\n\U0001F5B1️ utilizzare Figma per creare MVP di nuove idee di business.\n\nSe ti interessa uno di questi argomenti o vuoi scrivermi per altre questioni, mandami un messaggio qui su Linkedin, oppure scrivimi una mail a \U0001F449 dandele93@gmail.com\n\nSe invece vuoi leggere un pò di cose, ti consiglio di leggere i miei post, non dico che ti cambieranno la vita ma magari possono essere interessanti!\n"
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
    styles:
      self:
        width: wide
        padding:
          - pt-8
          - pb-8
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
        borderStyle: solid
  - type: TextSection
    variant: variant-a
    subtitle: 'Contact:'
    colors: colors-f
    text: |
      [daniele@danieledamico.tech](daniele@danieledamico.tech)
  - type: DividerSection
    styles:
      self:
        width: wide
        padding:
          - pt-8
          - pb-8
          - pl-4
          - pr-4
        justifyContent: center
        borderWidth: 1
        borderStyle: solid
  - type: ContactSection
    backgroundSize: full
    title: "Facciamo 4 chiacchiere ? \U0001F4AC"
    colors: colors-f
    form:
      type: FormBlock
      elementId: sign-up-form
      destination: ''
      action: /.netlify/functions/submission_created
      fields:
        - name: firstName
          label: First Name
          hideLabel: true
          placeholder: Come ti chiami?
          isRequired: true
          width: 1/2
          type: TextFormControl
        - name: lastName
          label: Last Name
          hideLabel: true
          placeholder: Ed il tuo cognome?
          isRequired: false
          width: 1/2
          type: TextFormControl
        - name: email
          label: Email
          hideLabel: true
          placeholder: Email
          isRequired: true
          width: full
          type: EmailFormControl
        - name: message
          label: Message
          hideLabel: true
          placeholder: Di cosa vorresti parlare?
          isRequired: true
          width: full
          type: TextareaFormControl
      submitLabel: "Submit \U0001F680"
      styles:
        submitLabel:
          textAlign: center
    styles:
      self:
        height: auto
        width: narrow
        margin:
          - mt-0
          - mb-0
          - ml-4
          - mr-4
        padding:
          - pt-12
          - pb-12
          - pr-4
          - pl-4
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        textAlign: left
      text:
        textAlign: left
---
