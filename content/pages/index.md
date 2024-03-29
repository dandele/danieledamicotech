---
title: Home - Daniele D'Amico
layout: PageLayout
colors: colors-e
backgroundImage:
  backgroundSize: cover
  backgroundPosition: center
  backgroundRepeat: no-repeat
  opacity: 100
sections:
  - elementId: hero_home
    colors: colors-a
    backgroundSize: full
    title: 'Ciao, sono '
    title2: Daniele D'Amico
    subtitle: 'Un giovane '
    subtitle2: in costante crescita!
    styles:
      self:
        height: screen
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-0
          - pb-0
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: row-reverse
        borderStyle: solid
      title:
        textAlign: left
      subtitle:
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
    type: HeroSection
    actions:
      - type: Button
        label: COMINCIA QUI
        altText: ''
        url: /info
        showIcon: false
        icon: arrowRight
        iconPosition: right
        style: primary
        elementId: ''
        colors: colors-c
  - type: FeaturedPostsSection
    colors: colors-f
    elementId: featured-posts-home
    showDate: false
    showAuthor: false
    showExcerpt: true
    showFeaturedImage: true
    showReadMoreLink: true
    variant: variant-b
    actions:
      - type: Link
        label: VUOI ALTRI CONSIGLI?
        altText: VUOI ALTRI CONSIGLI?
        url: /blog
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-24
          - pb-24
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: center
    subtitle: Non sai da dove cominciare? Ecco qualche consiglio!
    posts:
      - content/pages/blog/postlayout-5zj57kmef.md
      - content/pages/blog/postlayout-gqcucb13d.md
      - content/pages/blog/post-five.md
  - type: LabelsSection
    colors: colors-c
    elementId: scorciatoie
    title: Scorciatoie
    items:
      - type: Label
        label: Product Management
        url: /tags/product-management
      - type: Label
        label: Notion
        url: /tags/notion
      - type: Label
        label: Curation
        url: /tags/curation
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-36
          - pb-36
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: left
      subtitle:
        textAlign: left
    subtitle: >-
      C'è un argomento che ti interessa in particolare? 

      Ho raccolto quelli che più tratto in questo sito e ne ho creato delle
      scorciatoie, cliccaci e potrai entrare nella tana del bianconiglio!
  - type: FeaturedPostsSection
    elementId: ''
    colors: colors-f
    variant: variant-d
    subtitle: Alcune delle cose che ho scritto
    showFeaturedImage: true
    actions:
      - type: Link
        label: LEGGI DI PIÙ
        url: /blog
    posts:
      - content/pages/blog/post-seven.md
      - content/pages/blog/post-six.md
      - content/pages/blog/post-one.md
    showDate: false
    showExcerpt: true
    showReadMoreLink: true
    styles:
      self:
        height: auto
        width: narrow
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-28
          - pb-48
          - pl-4
          - pr-4
        justifyContent: center
        borderRadius: none
        borderWidth: 0
        borderStyle: none
        borderColor: border-dark
      title:
        textAlign: left
      subtitle:
        textAlign: left
      actions:
        justifyContent: flex-end
  - type: ContactSection
    colors: colors-f
    backgroundSize: full
    title: "Sempre aperto a collaborazioni, Facciamo 4 chiacchiere \U0001F4AC!"
    form:
      type: FormBlock
      elementId: sign-up-form
      destination: ''
      fields:
        - name: firstName
          label: Nome
          hideLabel: true
          placeholder: Com'è che ti chiami?
          isRequired: true
          width: full
          type: TextFormControl
        - name: email
          label: Email
          hideLabel: true
          placeholder: Email
          isRequired: true
          width: full
          type: EmailFormControl
        - name: updatesConsent
          label: Mi voglio iscrivere alla newsletter
          isRequired: false
          width: full
          type: CheckboxFormControl
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
          - ml-0
          - mr-0
        padding:
          - pt-24
          - pb-24
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
