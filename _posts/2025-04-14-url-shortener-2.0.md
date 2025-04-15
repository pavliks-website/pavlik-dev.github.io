---
layout: blog
type: news
title: URL Shortener 2.0
date: 2025-04-14 17:30:00 +0300
---
Here's some updates for my URL shortener service.

## The source code got completely rewritten from scratch.
The first version used [this code as a base](https://github.com/xyTom/Url-Shorten-Worker/), but 2.0 is now fully made by me. (yeah no AI involved too)
The source code will be available soon.

## Modes!
Now you can make links with different lengths, from 4 to 10 characters wide.\
For this you need to specify `mode` field in JSON payload:
```json
{
    "url": "https://google.com/",
    "mode": "normal"
}
```
The available at this moment modes are:
- `short`: 4 characters
- `normal`: 6 characters *(default)*
- `long`: 10 characters

### Which one do I need?
Well, there is no difference at all. You can use any length without fear that someone else will overwrite it. The code automatically selects only the link that is not taken.

But in case every link is taken, and the service errors out, you could try a longer link. Or just try again.

## API is now a little different.
Now to shorten a URL, you must use `/create` endpoint.\
And you can provide a wanted mode with `mode` field.\
And the output link got moved to `url` instead of `key`*???*\
**Its still free though ;)**

## Random links
1.0 used SHA256 hash and then truncated it to 4 characters to generate a link.\
2.0 now generates a pseudo-random links, which means its harder to predict the result. Not sure why would you want to predict it though.

<a href="/url-shortener/" style="font-size:larger">Go check it out here!</a>

So... yeah! This was **URL Shortener 2.0!** See you there!
