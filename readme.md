# Hugo + Cloudflare pages

background: I was thinking of making a quick web project to write essayesque things on and while looking for some inspiration by other devs I stumbled across cloudflare pages and decided to try it out along with hugo (another thing I wanted to try out)
---

## Procedure

1. Get the hugo cmdline utility 
2. create new hugo project using utility
3. add ur desired theme using `git submodule`
4. make a dummy post in content/posts
5. upload to github
6. go to dashboard then create new project, link with repo
7. In build settings mostly default but with following changes:
  - `framework/build command`: hugo (don't use the one given in the cdflare guide)
  - Inside ENV Variables add the latest version of Hugo, `HUGO_VERSION`:`0.110.0`
8. watch the build happen and reap your rewards

## Final thoughts 
The whole thing is real *fast* both the build process and the final static site generated. I'm really happy with it.

### Next steps
- Customise the style of the site to my preferance
  - [astro paper](https://astro-paper.pages.dev/)
  - [hagel](https://anna099.github.io/hegel/#int) for book style font and vibes
  - [papermod](https://adityatelange.github.io/hugo-PaperMod/) archive, search, tags features in menu
- write a script or something along those lines to 
  - Create the font matter automatically in the markdown editor I chose to use
  - Single command to publish new page written and then show the deployment when complete 
  
> note to self use `draft: true` in fontmatter to write what on my mind without worrying about polish