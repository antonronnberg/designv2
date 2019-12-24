---
views:
    main:
        template: anax/v2/article/default
        data:
            class: blog

    byline: false
    block-about: false
    article-toc: false

    blog-list:
        region: main
        template: anax/v2/blog-list/default
        sort: 2
        data:
            dateFormat: j F Y
            meta:
                type: toc
                orderby: publishTime
                orderorder: desc

    blog-toc:
        region: sidebar-right
        template: anax/v2/blog-toc/default
        sort: 2
        data:
            meta:
                type: copy
                view: blog-list

---
Nytt och Noterat
===========================

Blogginlägg om vardagen och äventyren, med inslag av bildhantering genom Cimage.
Bilderna är tagna med default inställning och utan filter. Enheter som användes
var antingen en iPhone SE eller GoPro Hero 5.

<!-- Kortare blogginlägg om vad som händer på dbwebb.se, kurserna samt webbprogrammering och webbutveckling med HTML, CSS, JavaScript, PHP och SQL i allmänhet. -->
