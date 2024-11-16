# Homepage
Ref:
- https://github.com/adityatelange/hugo-PaperMod/?tab=readme-ov-file
- https://gohugo.io/getting-started/configuration/
- https://jessewei.dev/blog/2023/papermod/#why-did-i-switch
  - https://github.com/jesse-wei/jessewei.dev-PaperMod


# New Post
```bash
hugo new posts/my-first-post.md
```


# Theme
Needed when first time clone
```bash
git submodule update --init --recursive
```

To update the theme, run:
```bash
git submodule update --remote --merge
```


# Deploy
```bash
hugo server -D

hugo --minify
```
