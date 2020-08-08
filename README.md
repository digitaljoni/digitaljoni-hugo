# Digitaljoni Website

Digitaljoni website is developed using [Hugo](https://gohugo.io/)

## Getting Started

Follow instructions on [installing Hugo](https://gohugo.io/getting-started/installing/) on your machine.

## Instructions
Git Clone using --recurse-submodules -j8
```
git clone --recurse-submodules -j8 git@github.com:digitaljoni/digitaljoni-hugo.git digitaljoni_hugo
```


## Commands

Run Development Server
```bash
hugo server --buildDrafts --watch
```

Add new content page
```bash
hugo new privacy.md
```

Add new blog post
```bash
hugo new blog/test.md
```

Deploy
```bash
./deploy.sh
```


## Generate Thumbnails in Gallery

```
for i in `find static/images/galleries -type f ! -name "*-thumb.png" -name "*.png"`; do echo $i; if [ -f ${i%.*}-thumb.png ]; then continue; fi; convert $i -thumbnail 100x100 ${i%.*}-thumb.png; done
```