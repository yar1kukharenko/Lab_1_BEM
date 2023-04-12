# Лабораторная работа №1

## Ветвление в Git и методология BEM.

---

### Описание человеческого тела с помощью BEM

- Блок body :
  - Элемент: head
    - Модификатор: hair-color_red
    - Модификатор: eye-color_blue
  - Элемент: arms
    - Элемент: left-arm
      - Модификатор: tattoo
    - Элемент: right-arm
      - Модификатор: ring
  - Элемент: legs
    - Модификатор: shoe-color_black
    - Модификатор: pant-style_skinny
- Блок: face
  - Элемент: eyes
    - Модификатор: eyelash-length_long
  - Элемент: nose
    - Модификатор: size_big
  - Элемент: mouth
    - Модификатор: lipstick-color_red
- Блок: clothing
  - Элемент: shirt
    - Модификатор: shirt-color_blue
    - Модификатор: collar-style_button-down
  - Элемент: pants
    - Модификатор: pant-length_cropped
    - Модификатор: pant-color_black

### Создание блоков в нотации Emmet с использованием BEM

- Header

![Header](/form.png)

```
    header.header>div.header__container>div.header__logo+(nav.header__nav>ul.header__nav-list>li.header__nav-item*4>a.header__nav-link)+button.header__menu-button
```

- Form

```
    form.form>div.form__container>fieldset.form__fieldset>(legend.form__legend+label.form__label*3>input.form__input)+button.form__button[type="submit"]
```

- Cards

```
    section.card>(div.card__container>img.card__image+div.card__content>h3.card__title+div.card__cta>a.card__link)*4
```

- Footer

```
    footer.footer>(div.footer__logo_section>div.footer__logo_section__logo+div.footer__logo_section__text+(div.footer__logo_section__links>a.footer__logo_section__link*4))+(div.footer__links>h6.footer__links__header+footer__link*4)*3

```
