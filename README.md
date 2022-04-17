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

-   Install dotenv - npm install dotenv
-   Create a .en file

API-KEY=valuer
SECOND_API_KEY=value

-   Make sure .env is in my .giignore (everytime you change your .env. file)
-   At the top of my JS file, import dotenv's config

js
import "dotenv/config";

const
const secondApiKey = process.env
