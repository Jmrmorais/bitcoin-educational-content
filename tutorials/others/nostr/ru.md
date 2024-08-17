---
name: NOSTR

description: Откройте для себя и начните использовать NOSTR
---

По окончании этого руководства вы поймете, что такое Nostr, создадите аккаунт и сможете его использовать.

![Появился новый вызов](assets/1.webp)

## Что такое Nostr?

Nostr — это протокол, который может заменить Twitter, Telegram и другие социальные медиа платформы. Это простой открытый протокол, способный создать глобально устойчивую социальную сеть раз и навсегда.

## Как это работает?

Nostr основан на трех компонентах: парах ключей, клиентах и ретрансляторах.

У каждого пользователя есть одна или несколько идентичностей, и каждая идентичность определяется криптографической парой ключей.

Для доступа к сети вам нужно использовать клиентское программное обеспечение и подключаться к ретрансляторам для приема и передачи контента.

![Система ключей](assets/2.webp)

## 1. Криптографические ключи

В отличие от Facebook или Twitter, где пользователи должны предоставить адрес электронной почты и множество информации частной компании, Nostr работает без центрального органа. Пользователи генерируют криптографическую пару ключей, секретный ключ (также известный как закрытый ключ) и открытый ключ.

Секретный ключ, nsec, известный только пользователю, используется для аутентификации и публикации контента.

Открытый ключ, npub, является уникальным идентификатором, к которому прикреплен весь контент, опубликованный пользователем. Ваш открытый ключ подобен имени пользователя, которое позволяет другим пользователям находить вас и подписываться на вашу ленту Nostr.

## 2. Клиенты

Клиенты — это программное обеспечение, позволяющее взаимодействовать с Nostr. Основные клиенты:

> iOS: damus
> Android: amethyst
> Web: iris.to; snort.social; astral.ninja

Клиенты позволяют пользователям генерировать новую пару ключей (эквивалент создания аккаунта) или аутентифицироваться с существующей парой ключей.

## 3. Ретрансляторы

Ретрансляторы — это простые серверы, которые вы можете покинуть в любое время, если вам не нравится контент, который они вам доставляют. Вы также можете запустить свой собственный ретранслятор, если хотите.

> 💡 Совет профессионала: Платные ретрансляторы обычно более эффективны в фильтрации спама и нежелательного контента.

# Руководство

Теперь вы знаете достаточно о Nostr, чтобы начать и создать свою первую идентичность в этом протоколе.

Для целей этого руководства мы будем использовать iris.to (https://iris.to/) как этот веб-клиент работает на любой платформе.

## Шаг 1: Генерация ключей

Iris создаст для вас набор ключей, и вам не нужно будет делать ничего, кроме как ввести имя (настоящее или вымышленное) для вашего профиля. Затем нажмите на GO и все готово!

![Главное меню](assets/3.webp)

> ⚠️ Внимание! Вам нужно будет следить за своими ключами, если вы хотите иметь возможность снова получить доступ к своему профилю после закрытия сессии. Я покажу вам, как это сделать в самом конце этого руководства.

## Шаг 2: Публикация контента

Чтобы опубликовать контент, это так же просто и интуитивно понятно, как написать несколько слов в поле публикации.

![Публикация](assets/4.webp)

Вот и все! Вы опубликовали свою первую заметку на Nostr.

![Пост](assets/5.webp)

## Шаг 3: Найти друга

Найдите меня на Nostr и никогда больше не будете одиноки. Я подпишусь в ответ на всех, кто подпишется на мою ленту. Для этого просто введите мой открытый ключ

npub1hartx53w6t3q5wv9xdqdwrk7h6r5866t8u775q0304zedpn5zgssasp7d3 в строке поиска.
![Мой профиль](assets/6.webp)
Нажмите на "подписаться", и в течение нескольких дней я тоже подпишусь на вашу ленту. Мы будем друзьями. Буду также рад прочитать ваше сообщение, если захотите мне написать.

И обязательно подпишитесь на ленту Agora256, чтобы получать уведомление каждый раз, когда мы публикуем что-то новое: npub1ag0rawstycy7nanuc6sz4v287rneen2yapcq3fd06972f8ncrhzqx

## Шаг 4: Настройка вашего профиля

Вам еще предстоит немного работы, чтобы настроить ваш профиль. Для этого нажмите на аватар, который iris автоматически сгенерировал для вас, в правом верхнем углу экрана, а затем нажмите на "редактировать профиль".

![Профиль](assets/7.webp)

Теперь все, что вам нужно сделать, это указать iris, где найти ваше изображение и баннер профиля в интернете. Я рекомендую хостить свой контент: защищайте то, что принадлежит вам.

![Другой вариант](assets/8.webp)

Если хотите, вы также можете загружать изображения, они будут храниться для вас iris на nostr.build, бесплатном сервисе хостинга визуального контента для Nostr.

Как видите, вы также можете настроить свой клиент для приема и отправки сатоши. Таким образом, вы сможете вознаграждать авторов контента, который вам понравился, или, что еще лучше, накапливать сатоши за отличный контент, который вы будете публиковать.

## Шаг 5: Резервное копирование пары ключей

Этот шаг критически важен, если вы хотите сохранить доступ к своему профилю после выхода из клиента или истечения сессии.
Сначала нажмите на иконку "настройки", представленную в виде шестеренки
![Настройка](assets/9.webp)

Затем скопируйте и вставьте по одному ваш npub, npub hex, nsec и nsec hex в текстовый файл, который вы будете хранить в безопасности. Я рекомендую зашифровать этот файл, если вы знаете, как это сделать.

![Ключ](assets/10.webp)

> ⚠️ Обратите внимание на предупреждение от iris. Хотя вы можете без опаски делиться своим публичным ключом, совсем другая история с вашим приватным ключом. Любой, у кого он есть, сможет получить доступ к вашему аккаунту.

## Заключение

Вот и все, маленький страус, вы сделали первые шаги на Nostr. Теперь вам нужно научиться бегать на скорости молнии. Мы скоро опубликуем руководства, которые покажут вам, как управлять вашими ключами и как интегрировать молнию в ваш опыт использования Nostr с помощью getalby.