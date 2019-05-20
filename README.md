Using Hexo for my blog. Supports markdown and embedded LaTex (see small LaTex example https://github.com/thcd/hexo-katex)

Use all CLI commands in the blog-site folder. The source for posts themselves are stored in `source/_posts`.

- New post: `hexo new "Some Title"` => `some-title.md` (
  - Also `some-title` folder for images, if any e.g. see `hasura-and-database`
- Edit `some-title.md` starting from title, date, tags, etc. at top
- Locally view site: `hexo server`
- Publish to web:
  - Git add, commit, push (pushes source files)
  - Remove old generated site: `hexo clean`
  - Generate new site & publish: `hexo deploy --generate`
- Detailed commands here: https://hexo.io/docs/commands.html
- Configuration is in file _config.yml

