# site
Website for Neoteric Consulting

## clone
``` git clone git@github.com:neo-teric/site.git```

##  create a new post
```
hugo new content content/posts/first-post.md (it will be in draft: true)

+++
title = 'First Post'
date = 2024-06-23T15:18:14-07:00
draft = true
+++
```

## run local server
```
- install hugo (brew install hugo)
- hugo server -D
(Web Server is available at http://localhost:1313/ (bind address 127.0.0.1))
```

## publish
- make sure you have draft:false in your post

+++
title = 'First Post'
date = 2024-06-23T15:18:14-07:00
draft = false
+++

- hugo
  it generates the public folder
