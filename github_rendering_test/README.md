# GitHub README.md Image Support Tests

## Markdown

```markdown
![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif | width=30)
```

renders as:

![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif | width=30)

❌

---

```markdown
![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif =30x110)
```

renders as:

![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif =30x110)

❌

---

## SVG

```markdown
![SVG](SVG_animation_using_CSS.svg)
```

renders as:

![SVG](SVG_animation_using_CSS.svg)

✅

---

```markdown
![SVG](SVG_animation_using_SMIL.svg)
```

renders as:

![SVG](SVG_animation_using_SMIL.svg)

✅

---

```markdown
![SVG](SVG_animation_using_JS.svg)
```

renders as:

![SVG](SVG_animation_using_JS.svg)

✅❌ (the JavaScript animation is sanitized)

---

```markdown
![SVG](https://github.com/tomchen/svg-clock/blob/master/clock.svg)
```

(SMIL-based animation + JavaScript to set current time) renders as:

![SVG](https://github.com/tomchen/svg-clock/blob/master/clock.svg)

✅❌ (the JavaScript code is sanitized, but SMIL-based animation is kept)

---

## URL

```html
<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

✅

---

```html
<img src="https://github.com/tomchen/my-avatar/blob/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="https://github.com/tomchen/my-avatar/blob/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

✅

---

```html
<img src="../tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="../tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

✅

---

```html
<img src="https://raw.githubusercontent.com/tomchen/my-avatar/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="https://raw.githubusercontent.com/tomchen/my-avatar/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

✅

---

## Emoji / Unicode Emoticon

```markdown
😊
```

(:point_up: Unicode character)

renders as:

😊

---

```markdown
:blush:
```

(:point_up: GitHub Flavored Markdown `:EMOJINAME:`)

renders as:

:blush:

---

```markdown
<g-emoji class="g-emoji" alias="blush" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f60a.png">😊</g-emoji>
```

(:point_up: HTML in markdown)

renders as:

<g-emoji class="g-emoji" alias="blush" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f60a.png">😊</g-emoji>

---

(The three aforementioned all render as exactly the same thing)

## ARIA

```html
<img src="https://github.com/tomchen/my-avatar/blob/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" aria-label="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

(HTML image element with `aria-label`) renders as:

<img src="https://github.com/tomchen/my-avatar/blob/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" aria-label="Tom Chen's animated GIF avatar" height="110px" width="110px">

❌ `aria-label` is stripped

## Image License

See [LICENSE.md](LICENSE.md)
