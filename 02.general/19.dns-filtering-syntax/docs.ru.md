---
title: Создание правил для DNS фильтрации
taxonomy:
    category:
        - docs
visible: true
---


[AdGuard для Android](https://kb.adguard.com/ru/android) и [AdGuard Home](https://kb.adguard.com/ru/home) предоставляют функцию фильтрации DNS трафика. Чтобы узнать больше о DNS-фильтрации, перейдите в [эту статью](https://kb.adguard.com/ru/general/dns-filtering-android) Базы знаний. В сравнении с [традиционной](https://kb.adguard.com/ru/general/how-ad-blocking-works) блокировкой рекламы, DNS-фильтрация является более "грубым" методом и не даёт таких широких возможностей настройки. Она не поддерживает сложный [синтаксис](https://kb.adguard.com/ru/general/how-to-create-your-own-ad-filters), используемый нами в обычных фильтрах, но зато поддерживает упрощённый синтаксис, позволяющий блокировать конкретные домены.

DNS фильтрация поддерживает два типа правил:

* Основные правила фильтрации, такие как [Базовые правила](https://kb.adguard.com/ru/general/how-to-create-your-own-ad-filters), но с поддержкой ограниченного набора модификаторов:

    * [`$important`](https://kb.adguard.com/ru/general/how-to-create-your-own-ad-filters#important-modifier)
    * [`$match-case`](https://kb.adguard.com/ru/general/how-to-create-your-own-ad-filters#match-case-modifier)
    * Правила с другими модификаторами будут проигнорированы

* "Hosts" правила, синтаксис которых является базовым

Примеры:

1. `||example.org^` - блокирует доступ к example.org и ко всем его поддоменам
2. `@@||example.org^` - разблокирует доступ к example.org и ко всем его поддоменам
3. `0.0.0.0 example.org` - AdGuard будет возвращать 0.0.0.0 адрес для example.org (но не к его поддоменам)
4. `! Это комментарий` - комментирование
5. `" # " И это комментарий` - тоже комментирование
6. `/REGEX/` - блокирует доступ к доменам, соответствующим заданному регулярному выражению

Используйте этот синтаксис, чтобы создавать или импортировать правила в DNS-фильтр. Если у вас есть какие-либо вопросы, вы можете задать их на нашем [форуме](https://forum.adguard.com/index.php?forums/25/).

