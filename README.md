# Team 5458: Digital Minds Website

This is based on the [Krishna](https://github.com/sharu725/krishna) theme.

This website run on Jekyll and uses static site generation.

## FORMATTING

### Pages

ALL PAGES MUST:

- Be in `/_pages/`
- Have a title and a permalink
- Be named the same as their permalink. `eg about-us.md for /about-us/`
- All pages with child pages must be in their own folder with an index file inside
  - Directory structure for a `/robots/` page with a `/robots/2019/` child page would be:
    - `/_pages/robots/index.md`
    - `/_pages/robots/2019.md`
    
#### Page Front Matter

Pages can contain the `parent:` front matter, which will add a back button to the header of the page. Use this for child pages such as `/robots/2019/`. `parent:` front matter is absolute, so the front matter for `/robots/2019/` is `/robots/`
    
### Images

ALL IMAGES MUST:

- Be in `/images/`
- Be in a folder which is named the same as the page they are on. `eg an image on /about-us/ must be in /images/about-us/`
- Be named in an intelligent manner, no `f696003dc681653e603a83b2ae0ba982.jpg`

### Collections

#### Sponsors

Sponsors are located in `/_data/sponsors/` and each have their own file.

Sponsor files are to be named accordingly:

```
xy-zzzz.md

x: importance (0 is high, 6 is low)
y: subimportance (0 is first, 9 is last, if more than 10, use a-z)
z: name of the sponsor (replace spaces with -, use full names or official abbreviations
```
