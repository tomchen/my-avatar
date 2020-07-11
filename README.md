# Tom Chen's Avatar and GitHub Image Tips

My animated avatar, and tips on using images on GitHub README.md and some other social media websites.

## My Avatar

<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">

![Tom Chen's non-animated SVG avatar](https://github.com/tomchen/my-avatar/raw/master/tomchen.svg "Tom Chen's non-animated SVG avatar")

Version 1.0 was made in 2000s with Adobe Flash.

Current version, v8.0, was made in 2014.

The SVG file is exported from Flash without animation. It is planned to re-add the animation with JavaScript to the SVG file.

## Which social media websites allow animated avatar

Notes on social media:

* ✅ **Google**, **Medium**, **Stackoverflow**, **Dev.to** users can use animated GIF as their profile avatar.
* 😐 Although **Google** accepts animated GIF, but it is sometimes rendered as still image.
* ⛔ **GitHub**, **GitLab**, **Reddit**, **Gravatar** do not accept animated GIF.
* 🤐 **Twitter** used to accept animated GIF before 2012. Old user with an animated GIF avatar can keep it.

## Tips of GitHub image usage

### Image width and height

You can't set width and height on images by using GitHub Flavored Markdown, in order to do so, you have to use HTML

```html
<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

### Image URL

These image URL references are all acceptable:
```
https://github.com/tomchen/my-avatar/raw/master/tomchen.gif
https://github.com/tomchen/my-avatar/blob/master/tomchen.gif
https://raw.githubusercontent.com/tomchen/my-avatar/master/tomchen.gif
../tomchen.gif
```

### Emoji

Unicode character `😊` and GitHub Flavored Markdown `:blush:` render as exactly the same 😊 whose HTML code is:

```html
<g-emoji class="g-emoji" alias="blush" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f60a.png">😊</g-emoji>
```

### SVG animation

In SVG files, SMIL and CSS animation are kept, but JavaScript animation is sanitized.

### GitHub README.md Image Support Tests

[GitHub image rendering test](github_rendering_test)
