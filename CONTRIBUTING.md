# 👨‍💻 Contributing

### 1. Forking the Repo
A fork is a local copy of the repository that is on your GitHub account, and you can make changes on that repository.
#### [Click here to Fork](https://github.com/oyepriyansh/DevTweet/fork)

### 2. Creating a Post
You can create a post super easily by making a new file in the `src/content/posts` directory.

For example, you could create the file `hello.md`. Now, you need to fill in the frontmatter of the post. This stores basic data about the post.

You can also supply `image` and `slug` to the frontmatter.

```md
---
layout: ../../layouts/PostLayout.astro # Always use this layout, it's so the post gets properly styled
title: the title of the post
excerpt: a short description about the post
createdAt: the date
author: your name
---

**This is the content of the post.**
```

### 3. Adding an Author

Go to  `src/util/authors.ts` file. just extend the array by adding your github username.

```ts
// Before:
export const AUTHORS = ["oyepriyansh", "WilliamDavidHarrison"] as const;

// After:
export const AUTHORS = ["oyepriyansh", "WilliamDavidHarrison", "YOUR_GITHUB_USERNAME"] as const;
```

### 4. Author Image

You can add an image for yourself by uploading an image to the `/public/authors` directory. Please make sure that is it spelt the exact same as your github username in the `src/util/authors.ts` file.

> **Note**:  Capitalization does not matter for the image file, make it all lower-case.

### 5. Pull Request
- You can now commit changes to tha t repository. Once you've made the changes you want, [create a pull request](https://github.com/oyepriyansh/DevTweet/pulls) on the main repository.
- Once you have submitted pull request, it will be reviewed and merged as soon as possible
