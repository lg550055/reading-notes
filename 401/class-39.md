# React 3: useContext & Next.js

### useContext

React context is an essential tool to easily share state in your applications.  It allows us to pass down data without using props, i.e., avoids prop drilling.

Data that does not need to be updated often is suitable for React context:

- Theme data (dark or light mode)
- User data (the currently authenticated user)
- Location-specific data (user language or locale)

> There are four steps to using React context:

1. Create context using createContext
2. Wrap the context provider around the component tree
3. Add data to context provider using the value prop
4. Read that value within any component by using the context consumer

---

### Next.js

*Node.js version 10.13 or later is necessary to install Node.js.*

> In Next.js, a page is a React Component exported from a file in the pages directory.

> Pages are associated with a route based on their file name. For example, in development:

- pages/index.js is associated with the / route
- pages/posts/first-post.js is associated with the /posts/first-post route

#### Link

> In Next.js, you use the Link Component from next/link to wrap the <a> tag. <Link> allows you to do client-side navigation to a different page in the application.

##### Code splitting and prefetching <- this is cool!

Next.js splits code automatically. It only loads what’s necessary for that path, e.g., when the homepage is rendered, the code for other pages is not served initially.  This loads the homepage fast even if you have hundreds of routes (on the same single page app).

Only loading code for the requested page means that if it throws an error, the rest of the application would still work.

In a production build, whenever Link components appear, Next.js automatically prefetches the code for the linked page in the background. Thus, making page (route) transitions nearly instant!

#### Assets, Metadata, and CSS

##### Assets

> Next.js can serve static assets, like images, under the top-level public directory, which is also useful for robots.txt, Google Site Verification, and any other static assets.

Next.js provides an Image component in 'next/image'.   It also provides on-demand Image Optimiztion by defult.  For example, avoids shipping large images to devices with a smaller viewport.

##### Metadata

Use the Head component from the next/head module to add metadata like `<title>` or third-party JS.  Use the Script component from 'next/script' to use the third-party script in the page.

##### CSS

> Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.

A simple approach is to create a styled Layout component to wrap the content of pages.  Then, create a file called components/layout.module.css (generically 'componentname.module.css').  Import the module and apply its classes.

Alternatively, use the 'global.css' file for global style.

Or use TailwindCSS.

---

### Resources

- [Next.js tutotial](https://nextjs.org/learn/basics/create-nextjs-app)
- [React Context for Beginners](https://www.freecodecamp.org/news/react-context-for-beginners/)
-[Learn useContext video](https://www.youtube.com/watch?v=5LrDIWkK_Bc)
- [Next.js Examples](https://github.com/vercel/next.js/tree/canary/examples)

---

[Back to table of contents](../README.md)
