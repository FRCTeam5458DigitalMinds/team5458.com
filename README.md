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

Sponsors are located in `/_data/sponsors.yml`

Sponsor entries are to be made accordingly:

```
# (R) - Required, (O) - Optional
# name - The display name of the sponsor (R)
# image - The image to display for the sponsor (O)
# link - A hyperlink to the sponsor's website (O)
# importance - A ranking system of how large to display the sponsor, 0 is more important than 5. (R)
```

Sponsor images must be `275x160`.

#### History

History entries are located in `/_data/history/` and each year has its own file.

History files are to be named based on the year they happened.
