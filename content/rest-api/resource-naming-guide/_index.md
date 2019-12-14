+++
title = "Resource Naming Guide"
description = "Resource Naming Guide"
chapter = true
weight = 2
pre = "<b>2. </b>"
+++

# Resource Naming Guide
---

In REST, primary data representation is called Resource. Having a strong and consistent REST resource naming strategy – will definitely prove one of the best design decisions in the long term.

<hr />

### Handle trailing slashes gracefully
##### **Wrong convention**
```
GET: /articles/
```

##### **Correct convention (This is much better version)**
```
GET: /articles
```

<hr />

### Avoid using verbs in URIs
##### **Wrong convention**
```
GET: /articles/:slug/generateBanner/
```
```
POST: /articles/createNewArticle/
```

##### **Correct convention**
```
GET: /articles/:slug/banner
```
```
POST: /articles
```

### Use plural resource nouns
Should you use `/article/:id` (singular) or `/articles/:id` (plural)?

**I recommend using the plural form.**

Why? Because it fits all types of endpoints very well.

I'd agree that `GET /article/2` is fine, but what about GET `/article/`
<br />
Are we getting the one and only one article in the system, or all of them?
<br />
To prevent this kind of ambiguity, let's be consistent (life advice!) and use plural everywhere:

##### **Wrong convention**
```
GET: /article/2
POST: /article
```

##### **Correct convention**

```
GET: /articles/2
POST: /articles
```

<hr />

#### Other articles
---
- https://restfulapi.net/resource-naming/
- https://florimond.dev/blog/articles/2018/08/restful-api-design-13-best-practices-to-make-your-users-happy/
