## Introduction

My personal website is based on [bootstrap](https://github.com/StartBootstrap/startbootstrap-new-age).

The template is designed to integrate Markdown files as content input. There's no need to compile the webpage before deployment. Upon loading, the Markdown files are automatically parsed and embedded into the page.

:milky_way: Demo: https://sarmishra.github.io/

## Getting started with this template

### 1. Fork this repository

The repository name should be `<username>.github.io`, which will also be your website's URL.

### 2. Edit page content

(1) Go to the folder where you want to store your project, and clone the new repository:

```
git clone https://github.com/<username>/<username>.github.io.git
```

The directory structure is as follows:

```.
.
├── contents
└── static
    ├── assets
    │   └── img
    ├── css
    └── js
```

(2) Modify the content of each section, which corresponds to `contents/*.md`.

(3) Adjust the title, copyright information, and other text of the website in `contents/config.yml`

(4) Replace background image and photo with new ones for your web pages in `static/assets/img/`

(5) Push it:

```
git commit -am 'init'
git push
```

### 3. Enjoy

Fire up a browser and go to `https://<username>.github.io`

## License

Copyright Saroj Mishra, 2025. Licensed under an MIT license. You can copy and mess with this template.
