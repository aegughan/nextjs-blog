# To Create a Next.js app
## Run the below command to create a template applocation of Next.js

npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn-starter/tree/master/learn-starter"

# To run the Next.js application

## Go the the project directory
cd nextjs-blog

## Then, run the following command
npm run dev

It will starts the developement server. To check the application running. Open http://localhost:3000

# Study 
1. Next.js usin the integrated file system routing (i.e) Whenever a file is created it automatically form the route based on the file name.
    Example: 
        1. http://localhost:3000 It is the initial link points towards the file => /pages/index.js

        Let's create an another folder 'posts' inside the page directory. Create a file first-post.js inside the posts directory. So Next.js automatically creates the route.
        2. http://localhost:3000/posts/first-post It is the link points towards the file => /pages/posts/first-post.js
        3. To navigate between pages use 'Link' component. import the Link component from 'next/link'.
        4. While we use a tag instead of Link component, then the whole page gets refreshed.

2. ## Code Splitting and prefetching
    Code splitting has been done automatically in Next.js
    It means that the each page will loaded when only it's neccessary.
    By using the Link component the Next.js prefetches the code for the linked page in background. When we click the link it gets loaded.