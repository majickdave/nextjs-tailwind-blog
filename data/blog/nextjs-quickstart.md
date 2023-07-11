---
title: Creating Your First Website with Next.js
date: '2023-07-11'
tags: ['javascript', 'markdown', 'React', 'nextjs']
draft: false
summary: How to build your first Next.js project
---

written with GPT-4

# Creating Your First Website with Next.js

Next.js is a powerful open-source development framework built on top of Node.js, allowing you to create server-side rendered and static web applications using React. It brings a robust set of features to the table such as pre-rendering, automatic code splitting, and hot module replacement. In this blog post, we will walk through the process of creating your first website with Next.js.

## Prerequisites

Before you start, you need to have the following installed:

- Node.js (version 12.0 or later)
- NPM (which is included with Node.js)

## Step 1: Setting up Your Next.js Project

The first step is to create a new Next.js application. Open a terminal and run the following command:

```bash
npx create-next-app@latest my-first-next-app
```

This command will create a new Next.js application in a directory named `my-first-next-app`. Feel free to replace `my-first-next-app` with the name of your project.

Once the project has been created, navigate to the project directory:

```bash
cd my-first-next-app
```

## Step 2: Understanding the Project Structure

Let's take a brief look at the main files and directories:

- `pages/`: This directory contains your application's pages. Each file corresponds to a route based on its name.
- `public/`: This directory stores static files, such as images, that can be served by your application.
- `styles/`: This directory is where you'll put any global CSS files.
- `package.json`: This file contains metadata about your application, such as its name, version, and dependencies.

## Step 3: Creating a New Page

In Next.js, a page is a React Component exported from a `.js`, `.jsx`, `.ts`, or `.tsx` file in the `pages` directory. Let's create a new page named "About". Create a file in the `pages` directory named `about.js` and add the following content:

```jsx
export default function About() {
  return (
    <div>
      <h1>About Me</h1>
      <p>This is the about page of our first Next.js website.</p>
    </div>
  )
}
```

You can access this page by going to `http://localhost:3000/about`.

## Step 4: Running Your Next.js Application

You can start your Next.js application by running the following command in the terminal:

```bash
npm run dev
```

This will start your application in development mode, and you can view it by opening `http://localhost:3000` in your web browser.

## Step 5: Building and Deploying Your Application

Once you're done with development, you can build your application for production by running:

```bash
npm run build
```

This will create a `.next` directory with the compiled version of your application.

To start your application in production mode, you can run:

```bash
npm start
```

You can then deploy the `build` output (`/.next` folder) to a static server or a Node.js server.

## Conclusion

Congratulations! You've just created your first website with Next.js. This blog post only covered the very basics, but Next.js has many more features like API routes, dynamic routes, and support for CSS and SASS modules. I encourage you to check out the [Next.js documentation](https://nextjs.org/docs) to learn more.

Happy coding!
