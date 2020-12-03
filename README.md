# Hexo-theme-still

Still is a minimal, pure colored theme inspired by farbox and hexo-theme-apollo.

![preview](https://raw.githubusercontent.com/JeremyFan/static/images/still.png)

## Install pug renderer
If you got an error page when run `hexo server`:
```
extends partial/layout.pug block container include mixins/post.pug +postList() block pagination include mixins/paginator.pug +home() block copyright include partial/copyright.pug
```
try to install pug renderer:
```
npm install hexo-render-pug --save
```