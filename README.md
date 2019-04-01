# md2html

Адрес страницы: https://slavamilin.github.io/md2html/

Конвертирует md в html. На выходе готовая вёрстка прогоняется через типограф и бьютифаер.

## Заголовки

Заголовки начинаются с 3 уровня. По умолчанию всем заголовкам прописывается id = содержимому заголовка. Для того, чтобы задать собственный id заголовку нужно добавить `{}` после текста.  
**Пример:** 
```markdown
# Стандарты вёрстки{spec-1-1}
```
**Конвертируется в**
```html
<h3 id="spec-1-1">Стандарты вёрстки</h3>
```

## Ссылки

Если ссылка якорная, то её `href` дублируется в `id`

**Пример:**

```markdown
- [1.1](#1-1) Стандарты вёрстки
```

**Конвертируется в**

```html
<ul>
  <li><a href="#1-1" id="1-1">1.1</a> Стандарты вёрстки</li>
</ul>
```
