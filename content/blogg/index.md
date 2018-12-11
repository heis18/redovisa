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
Nytt i vardagen
===========================

Den här bloggen var tänkt att bestå av vackra naturbilder, fotograferade med mycket finess och tålamod.
Men det visade sig att inget av detta finns i mitt liv just nu, så istället blev detta en bilddagbok över vad som händer i min och familjens vardag!
