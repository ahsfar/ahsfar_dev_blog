
---
published: true
title: "Implement a generic oneOf type with Typescript"
cover_image: "https://raw.githubusercontent.com/ahsfar/ahsfar_dev_blog/master/blog-posts/name-of-your-blog-post/assets/cover.jpg"
description: "Implement a generic oneOf type with Typescript"
tags: typescript
series:
canonical_url:
---

Testing 
Uh 😵... Now can you imagine what it'd look like if we made an update to the game to add 5, 10 or 15 new animals? 🤕

This simply doesn't scale.

# Best of both worlds

How cool would it be to have something like the following:

```ts
type Animal = {
  id: string;
  name: string;
} & OneOf<{
  dog: Dog;
  wolf: Wolf;
  eagle: Eagle;
  mouse: Mouse;
}>;

interface Player {
  // ... same ...
}
```




# Found a typo?

If you've found a typo, a sentence that could be improved or anything else that should be updated on this blog post, you can access it through a git repository and make a pull request. Instead of posting a comment, please go directly to https://github.com/maxime1992/my-dev.to and open a new pull request with your changes. If you're interested how I manage my dev.to posts through git and CI, [read more here](https://dev.to/maxime1992/manage-your-dev-to-blog-posts-from-a-git-repo-and-use-continuous-deployment-to-auto-publish-update-them-143j).
