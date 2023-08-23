# Photo Gallery

Photo gallery featuring my pets and family. Hosted on GitHub Pages.

## Example Photo

<img alt="Olivia on the left. Honey on the right." src="https://raw.githubusercontent.com/semanticdata/photo-gallery/master/gallery/xhf-photo124.jpg" width="500px"/>

## Screenshot

![website screenshot](screenshot.png)

## Configuration

```json
{
  "input": "./gallery",
  "output": "./build_output",
  "title": "Photo Gallery", // Set your gallery title here
  "sort-albums-by": "title",
  "sort-media-by": "filename",
  "download-photos": "copy",
  "cleanup": true,
  "theme": "cards", // Your theme
  "css": "./custom.css",
  "footer": "Copyright Text", // Set your copyright text here
  "usage-stats": false
}
```

## Themes

You can chose from any of the themes below to set the value for theme key:

- `mosaic` - https://thumbsup.github.io/demos/themes/mosaic/
- `cards` - https://thumbsup.github.io/demos/themes/cards/
- `classic` - https://thumbsup.github.io/demos/themes/classic/
- `flow` - https://thumbsup.github.io/docs/4-themes/built-in/ (no demo available)

You can learn more about the configuration file here: https://thumbsup.github.io/docs/3-configuration/usage/.

## Adding a new album to gallery

1. Go to the gallery folder of the forked repo.
2. Click on Create a new file button.
3. Type AlbumName/.gitkeep in the input box
4. Click Commit Changes button at the bottom.

## Limitations

- Github Pages [terms of service](https://help.github.com/articles/github-terms-of-service/):

- File size limit (100 MB) & Repo size limit (75 GB) & Upload limit(25MB): Github limits the maximum usable filesize as 100MB for all files. This is enough for most users. It also imposes a repo size limit of 75GB. If you add a file to a repository via a browser, the file can be no larger than 25 MB. Visit https://help.github.com/articles/what-is-my-disk-quota/ for more info.

## Tools Used

- [GitHub Pages Gallery](https://github.com/gautamkrishnar/github-pages-gallery) for the template.
- [GithHub Pages](https://pages.github.com/) for hosting.
- [Thumbsup](https://thumbsup.github.io/) for gallery static page generation.
- [Github Actions](https://github.com/features/actions) For continuous deployment.

## License

Source code is available under [MIT](LICENSE).
