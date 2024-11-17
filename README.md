# Программа для перевода паролей с русской раскладки на английскую

Я запоминаю пароли только в русской раскладке клавиатуры.  
Без нужной клавиатуры я даже не смогу ввести их, если потребуется.

Однако есть проблема:

- Не на всех компьютерах есть русская раскладка.
- На разных устройствах раскладка может быть настроена по-разному.
- На мобильном телефоне переключение раскладок долгое и неудобное.

Чтобы упростить жизнь, я написал скрипт, который переводит пароль с русской раскладки на английскую и копирует его в буфер обмена:  
[Ссылка на скрипт](https://gist.github.com/istarkov/68075cf400cbd841101bc71b41f557a3#file-zshrc).

Для мобильных устройств я сделал похожее решение:  
[Ссылка на проект](http://CTAPKOB.github.io/keyboard-translate).

Дополнительно программа сохраняет SHA256-хеш пароля в `localStorage`.  
Это позволяет проверить, правильно ли введён пароль: если введённый пароль совпадает с сохранённым хешем, это отображается на экране.

## Как использовать

1. Склонируйте проект (вы же не будете вводить пароли на чужой веб-странице, правда?).
2. Подправьте `transformText` под свою клавиатуру.
3. Опубликуйте проект через GitHub Pages: [Руководство по GitHub Pages](https://pages.github.com/).
