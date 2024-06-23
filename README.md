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
```
- make sure you have draft:false in your post

+++
title = 'First Post'
date = 2024-06-23T15:18:14-07:00
draft = false
+++

- hugo
  it generates the public folder
- git commit
- git push
- github actions run and site is published.
```

## Draft, future, and expired content

Hugo allows you to set draft, date, publishDate, and expiryDate in the front matter of your content. By default, Hugo will not publish content when:

    The draft value is true
    The date is in the future
    The publishDate is in the future
    The expiryDate is in the past
