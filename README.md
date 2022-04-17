# Parcel & Vercel

## Hosting

-   Set up Git locally in your project
-   Make sure your package.json doesn't have a "main" key
    and you have your "build" script (get these from this repos package.json)
-   BEFORE you add or commit
-   Set up your .gitignore file (get the value of this from this repo)
-   Add, Commit
-   Create a new GitHub repository
-   Follow the steps for "Uploading an exisitng repo" 1 by 1
-   Log in/sign up to Vercel
    -   Go to your Dashboard and click "New Project"
    -   Import your Parcel Github repsitory
    -   Set the framework preset to Parcel
    -   Customize all of the Build and Output Settings
    -   Build command is `npm run build`
    -   Output directory is `dist`
    -   Install command `npm install`

## Hiding API Keys

-   Install dotenv - `npm install dotenv`
-   Create a .env file

```raw
API-KEY=value
SECOND_API_KEY=value
```

-   Make sure .env is in my .giignore (everytime you change your .env. file, you have to restart your server)
-   At the top of my JS file, import .dotenv's config

```js
import "dotenv/config";
```

-   Access environment variables through `process.env`

```js
const apiKey = process.env.API_KEY;
const secondApiKey = process.env.SECOND_API_KEY;
```

-   Tell Vercel about your environment variables
    -   Project Settings
    -   Environment Variables
    -   "Add New"
        -   For each line of your .env file, add them here
    -   Redeploy your project (by addings, committing and pushing)
