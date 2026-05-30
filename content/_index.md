---
# Leave the homepage title empty to use the site title
title: 'Чжао Синья'
summary: 'Персональный академический сайт Чжао Синья'
date: 2026-05-31
type: landing

sections:
  - block: markdown
    content:
      title: '👤 О себе'
      text: |-
        ## Чжао Синья

        **Группа:** НПИбд-03-25  
        **Номер студенческого:** 1132258332  
        **Направление:** Прикладная информатика  

        Студентка 1 курса факультета физико-математических и естественных наук РУДН.  
        Изучаю операционные системы, программирование и информационные технологии.

        *Добро пожаловать на мой сайт!*
    design:
      columns: '1'

  - block: markdown
    content:
      title: '📚 Образование и интересы'
      text: |-
        **Образование:**  
        - РУДН, Прикладная информатика, 2025-2029  

        **Интересы:**  
        - Операционные системы  
        - Программирование  
        - Информационные технологии  
        - Open Source  

        **Контакты:**  
        - GitHub: [Muzxnya](https://github.com/Muzxnya)  
        - Email: 1132258332@rudn.ru
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: '📄 Публикации'
      text: ''
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: news
    content:
      title: '📰 Последние новости'
      subtitle: ''
      text: ''
      page_type: blog
      count: 5
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]
---
