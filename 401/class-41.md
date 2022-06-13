# Next.js: Dynamic Routes & Deployment

### Dynamic Routes

A dynamic route is one where the page path depends on external data.

Next.js allows for statically generating dynamic routes.

1. To identify a page as a dynamic route, enclose its file name in square brackets, e.g. `[dynamic].js`

2. Export an async function called `getStaticPaths` from the dynamic page.  The function returns a list of the path's possible values.

3. Export another async function called `getStaticProps` which takes `{ params }`, an array of objects, each of which has 'params' as its key.  This function fetches the content.

### Deployment

Next.js was created by Vercel, which is seemingly the easiest way to deploy.

1.  Link GitHub repo to Vercel account.
2.  Generally there's no need to change the default settings, but if needed this is the time.

That's it!

Under the hood:
- > Pages that use Static Generation and assets (JS, CSS, images, fonts, etc) will automatically be served from the Vercel Edge Network, which is blazingly fast.
- > Pages that use Server-Side Rendering and API routes will automatically become isolated Serverless Functions. This allows page rendering and API requests to scale infinitely.

#### Develop, Preview, and Ship.

- **Develop**: Write code in Next.js (used the Next.js development server with its hot reloading feature).
- **Preview**: Push changes to a branch on GitHub. Vercel automatically creates a deployment preview available via a URL. Share it with others for feedback.
- **Ship**: Merge the pull request to main to ship to production.

---

### Bonus: Static File Serving

> Next.js can serve static files, like images, under a folder called public in the root directory. Files inside public can then be referenced by your code starting from the base URL (/).



---

### Resources

- [Next.js - Dynamic Routes](https://nextjs.org/learn/basics/dynamic-routes/page-path-external-data)
- [Next.js - Deployment](https://nextjs.org/learn/basics/deploying-nextjs-app)
- [Next.js - Static File Serving](https://nextjs.org/docs/basic-features/static-file-serving)
- [Next.js 10 is here](https://www.youtube.com/watch?v=JWCS5IdECVI)


---

[Back to table of contents](../README.md)
