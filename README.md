# Photo Gallery

Photo gallery featuring my pets and family. Hosted on GitHub Pages.

<img alt="Olivia on the left. Honey on the right." src="https://miguelpimentel.do/photo-gallery/media/large/xhf-photo124.jpg" width="500px"/>

## Why this project?

This project contains starter code for anyone who wants to deploy his/her photo/video galery on Github Pages,
**Zero Coding Needed**. Since Github pages is a free hosting service offered by Github to host static pages, it
offers a decent bandwidth. So it is a great choice for photographers to showcase their works. Github Actions is a CI & CD
platform that offers unlimited builds for open source projects. Combining the power of GitHub pages with Github Actions is
a zero dollar solution to get your gallery online.

## How to use

Follow the steps below to get your Gallery online. You will be using GitHub web interface to do everything.
:wink: No frustrating CLIs:

1. SignUp for a Github account and verify your email ID: https://github.com/join
2. Click on the use this template button:
3. Type a Name for your new repository
4. Click on the settings tab. Click on the **Pages** option under the **Code and automation** section. Make sure that you have the **GitHub actions** selected as the **Source** for the GitHub pages.
5. Edit [config.json](config.json) by clicking on the edit button in the newly created repository under your account:

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

You can chose from any of the themes below to set the value for theme key:

- `mosaic` - https://thumbsup.github.io/demos/themes/mosaic/
- `cards` - https://thumbsup.github.io/demos/themes/cards/
- `classic` - https://thumbsup.github.io/demos/themes/classic/
- `flow` - https://thumbsup.github.io/docs/4-themes/built-in/ (no demo available)

You can learn more about the configuration file here: https://thumbsup.github.io/docs/3-configuration/usage/.

1. Go to actions tab of your new repository, Wait till the Initial build completes. It will show you the check mark.
2. You are all set with your new awesome gallery! Add Albums or photos to make it live.

#### Adding a new album to gallery

1. Go to the gallery folder of the forked repo.
2. Click on Create a new file button.
3. Type AlbumName/.gitkeep in the input box
4. Click Commit Changes button at the bottom.

#### Adding Media

1. Go to gallery folder. Open any albums if any.
2. Click on Upload files button
3. Select files. Once it finishes upload, click Commit Changes button.

#### Finding your website URL

If you had done all the above steps then your website will be live now. Please check Github Actions tab in your repository for the sttaus of the
deployment. Once it is done, Go to settings tab again and scroll down to the Github Pages section to find your public gallery URL.

## Limitations

- Github Pages [terms of service](https://help.github.com/articles/github-terms-of-service/):

- File size limit (100 MB) & Repo size limit (75 GB) & Upload limit(25MB): Github limits the maximum usable filesize as 100MB for all files. This is enough for most users. It also imposes a repo size limit of 75GB. If you add a file to a repository via a browser, the file can be no larger than 25 MB. Visit https://help.github.com/articles/what-is-my-disk-quota/ for more info.

## Tools Used

- [Github Actions](https://github.com/features/actions) For continuous deployment.
- [Thumbsup](https://thumbsup.github.io/) for gallery static page generation.
- [GithHub Pages](https://pages.github.com/) for hosting.
