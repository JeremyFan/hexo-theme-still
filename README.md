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

## Activate Google Analytics:

1. Edit and apply your Google Analytics code in layout/mixins/ga.pug.pug

```
    ga('create','UA-XXXXX-X', 'yourDomain.com')
```

If you have only one website, you can apply it as:

```
    ga('create','UA-XXXXX-X')
```

2. Uncomment two lines in layout/partial/copyright.pug showing as below:

```
    // Uncommnet two lines below to activate your Google Analytics
	// Remember to config your Google Analytics ID in mixins/ga.pug first.
	// include ../mixins/ga.pug
	// +ga
```

To:

```
    // Uncommnet two lines below to activate your Google Analytics
	// Remember to config your Google Analytics ID in mixins/ga.pug first.
	include ../mixins/ga.pug
	+ga
```

3. Restart/Re-render your hexo.

### Enable mermeaid

In your hexe's `_config.yml` file, add config for mermaid as blow:

```
mermaid: ## mermaid url https://github.com/knsv/mermaid
  enable: true  # default true
  version: "7.1.2" # default v7.1.2
  options:  # find more api options from https://github.com/knsv/mermaid/blob/master/src/mermaidAPI.js
    startOnload: true  # default true
```

(Please make sure that you have the latest hexo-theme-still update.)
