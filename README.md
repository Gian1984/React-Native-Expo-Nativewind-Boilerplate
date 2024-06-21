# How to install React Native / Expo / Nativewind

## React Native Expo :

**To create a new Expo project, run the following in your terminal :**

    npx create-expo-app@latest

**Install Watchman**

    `brew update`

	`brew install watchman`

## Nativewind :

**1.  Install nativewind and its dependencies.**

    npm install nativewind
    npm install --save-dev tailwindcss
    npx tailwindcss init

**2.  Replace the existing code in `tailwind.config.js` file with the code given below.**

    content: ['./app/**/*.{js,jsx,ts,tsx}', './components/**/*.{js,jsx,ts,tsx}', ],

**3.  In your `babel.config.js` add this line**

    plugins: ["nativewind/babel"],

**4.  Use process(css).then(cb) to work with async plugins**

    npm install --save-dev tailwindcss@3.3.2

** 5. In the root of the project create a file called global.d.ts and add the code given below **

    /// <reference types="nativewind/types" />

**6.  Run the command to run and clean the cache :**

    npx expo start -c



