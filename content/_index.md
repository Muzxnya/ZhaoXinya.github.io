---
# Leave the homepage title empty to use the site title
title: ''
summary: 'Персональный академический сайт Чжао Синья'
date: 2026-03-07
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Скачать резюме
        url: uploads/resume.pdf
      headings:
        about: 'О себе'
        education: 'Образование'
        interests: 'Интересы'
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 Обо мне'
      subtitle: ''
      text: |-
        Меня зовут **Чжао Синья**. Я студентка **Российского университета дружбы народов (РУДН)**.

        - **Группа:** НПИбд-03-25
        - **Номер студенческого:** 1132258332
        - **Направление:** Прикладная информатика

        Я изучаю операционные системы, программирование и современные информационные технологии. Этот сайт создан для публикации моих учебных и научных проектов.

        *Добро пожаловать на мой сайт!*
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Избранные публикации
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Недавние публикации
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Доклады и выступления
      filters:
        folders:
          - events
    design:
      view: card
  - block: collection
    id: news
    content:
      title: Последние новости
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 10
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the HugoBlox Kit demo site
    content:
      title: 👉 Создайте свой академический сайт
      text: |-
        Этот сайт создан с помощью HugoBlox Kit — бесплатного генератора статических сайтов на Hugo.

        Легко настраивайте внешний вид без программирования!
      button:
        text: Начать
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-gradient-to-br from-primary-500 via-primary-600 to-secondary-600 text-white shadow-2xl'
        css_style: ''
---
