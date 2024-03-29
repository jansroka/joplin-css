# My Joplin CSS

**Archive Note:** I was testing and playing with Joplin in H1/2023 and found it to be a very interesting project. So much that I started customizing it with my own CSS (this repo). It however lacked quite a few features that I needed, thus I switched back to my previous note taking app and archived this repo.

This repo contains the CSS that I use to customize how [Joplin Desktop](https://joplinapp.org/) on OSX looks. The default is a a bit, well, meh to my eyes.

## How to set up
1. Delete both css files, if they exist, from your Joplin config dir
```
rm ~/.config/joplin-desktop/userstyle.css
rm ~/.config/joplin-desktop/userchrome.css
```

2. Softlink the `userstyle.css` and `userchrome.css` files in this repo into the Joplin config dir
```
ln -s <local path to repo>/userstyle.css ~/.config/joplin-desktop/userstyle.css
ln -s <local path to repo>/userchrome.css ~/.config/joplin-desktop/userchrome.css
```

Now you have these 2 files under source control.

## How to know which style to change?
As a starting point, check here: https://discourse.joplinapp.org/t/introduction-to-customising-joplin-userchrome-css-userstyle-css/21370

## What is the development flow?
- Start Joplin
- Show Dev Tools from the menu at `Help->Toggle development tools`
- Edit css file
- Reload all files by hitting `CMD+Shift+R` while the dev tools are open (shortcut won't work if the dev tools are not open)

## License
MIT
