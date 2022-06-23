---
layout: post
title:  "React: useRef() Hook"
description: "A little introduction to DevOps and Github Actions"
date:   2020-10-26 20:01:21 -0400
type: card-img-top
categories: latin text
image:  # for local images, place in /assets/img/posts/
caption:
last-updated: 2022-06-22 20:01:21 -0400
author: Arshpreet Singh
card: card-2
---

So I recently found out the use of the `useRef() Hook`

Basically it returns a single object with only one property called *current*

```Javascript
const countRender = useRef(0);
// countRender = { current: 0 }
```

## UseCase

Every element in JSX has an attribute called **ref** through which we can pass our 'Refs'.

```Javascript
const messageWindow = useRef(null);

// Some code in middle

<div ref={messageWindow} ...>
// More code
```

Using the above syntax we can play with the `div` element itself as we will get the *element object* as the current value in our ref object.

```Javascript

useEffect(() => {
    messageWindow.current.scrollTop = 500px;
    // scrolls the div container by 500px
})
```

See you soon with more such learnings.

Peace!
