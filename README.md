# Team 5458: Digital Minds Website

This is based on the [Krishna](https://github.com/sharu725/krishna) theme.

This website run on Jekyll and uses static site generation.

## RUNNING LOCALLY

1. Install [Ruby](https://www.ruby-lang.org/en/downloads/) if not already installed. 
2. Install bundler
   ```
   $ gem install bundler
   ```
3. Pull or download this repository
4. Run the Jekyll site
    ```
    $ bundle exec jekyll serve
    ```
5. The page will auto update while you make changes. Please make sure that you test desktop and mobile before pushing changes.


## FORMATTING

### Pages

ALL PAGES MUST:

- Be in `/_pages/`
- Have a title and a permalink
- Be named the same as their permalink. `eg about-us.md for /about-us/`
- Any pages with children pages should use data pages with `output: true` in `_config.yml`. The `permalink` variable in `_config.yml` should be `/<parent-page>/:name`
    
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

x: importance (0 is high, 5 is low)
y: subimportance (0 is first, 9 is last, if more than 10, use a-z)
z: name of the sponsor (replace spaces with -, use full names or official abbreviations
```

Sponsor images must be `275x160`.

#### History

History entries are located in `/_data/history/` and each year has its own file.

History files are to be named based on the year they happened.