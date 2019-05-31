Using Hexo for this blog. It supports markdown and embedded LaTex (tiny examples of LaTex embedding https://github.com/thcd/hexo-katex, full editable cheat-sheet https://math-on-quora.surge.sh/)

Use all CLI commands in the blog-site folder. The source for posts themselves are stored in `source/_posts`.

- New post: `hexo new "Some Title"` (makes `some-title.md`)
  - Also `some-title` folder for images, if any e.g. see `hasura-and-database`
- Edit `some-title.md` starting from title, date, tags, etc. at top
- Locally view the site: `hexo server`
- Publish to web:
  - Git add, commit, push (pushes source `.md` files etc)
  - Remove old generated site: `hexo clean`
  - Generate new site html & publish: `hexo deploy --generate`
- Detailed commands here: https://hexo.io/docs/commands.html
- Configuration is in file `_config.yml`

