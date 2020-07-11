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

* :muscle: **Google**, **Medium**, **Stackoverflow**, **Dev.to** users can use animated GIF as their profile avatar.
* :neutral_face: Although **Google** accepts animated GIF, but it is sometimes rendered as still image.
* :no_entry: **GitHub**, **GitLab**, **Reddit**, **Gravatar** do not accept animated GIF.
* :zipper_mouth_face: **Twitter** used to accept animated GIF before 2012. Old user with an animated GIF avatar can keep it.

## Tips of images in GitHub README.md

You can't set width and height on images by using GitHub Flavored Markdown, in order to do so, you have to use HTML

```html
<img src="https://github.com/tomchen/my-avatar/raw/master/tomchen.gif" alt="Tom Chen's animated GIF avatar" title="Tom Chen's animated GIF avatar" height="110px" width="110px">
```

### GitHub README.md Image Support Tests

[GitHub image rendering test](github_rendering_test)
