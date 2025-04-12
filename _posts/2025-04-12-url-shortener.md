---
layout: blog
date: 2025-04-12 22:20:00 +0300
title: URL Shortener!
type: news
---

Sometimes I wonder why there's no service like bit.ly for HTTP, so I made one!\
Unfortunately I had to sacrifice my short domain for this, but it's worth it!
Now, [pyt.pp.ua](//pyt.pp.ua/) can shorten links no worse than in bit.ly, tinyurl.com, and others.

<a href="https://pyt.pp.ua/" style="font-size:larger;text-align:center;display:block">Check it out here!</a>

## API

Yeah, the API is not only free, but also simple as counting to three.

`https://pyt.pp.ua/` is the only endpoint here. Just make a POST request with
this body:
```json
{
    "url": "https://example.com/"
}
```
*of course, don't forget to change example.com to your URL*

The response will look like this:
```json
{
    "status": 200,
    "link": "https://pyt.pp.ua/..."
}
```

`link` field is what you need.

### Errors
Error map looks like this:
```json
{
    400: "Invalid URL",
    404: "Link doesn't exist",
    409: "Alias already exists"
}
```
*HTTP 500 is an unhandled internal error, keep that in mind*
