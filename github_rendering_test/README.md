# GitHub README.md Image Support Tests

## URL

```html
<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

```html
<img src="https://github.com/tomchen/my-avatar/blob/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="https://github.com/tomchen/my-avatar/blob/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

```html
<img src="../tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="../tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

```html
<img src="https://raw.githubusercontent.com/tomchen/my-avatar/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

renders as:

<img src="https://raw.githubusercontent.com/tomchen/my-avatar/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

## Markdown

```html
![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif | width=30)
```

renders as:

![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif | width=30)

```html
![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif =30x110)
```

renders as:

![Tom Chen's animated GIF avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.gif =30x110)


## SVG

```markdown
![SVG](SVG_animation_using_CSS.svg)
```

renders as:

![SVG](SVG_animation_using_CSS.svg)

```markdown
![SVG](SVG_animation_using_SMIL.svg)
```

renders as:

![SVG](SVG_animation_using_SMIL.svg)

```markdown
![SVG](Ampel.svg)
```

renders as:

![SVG](Ampel.svg)


## Image License

See [LICENSE.md](LICENSE.md)
