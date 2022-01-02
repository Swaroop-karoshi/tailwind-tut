# tailwind css basic postcss files requried to build website

# TAILWINDCSS
A utility-first CSS framework for rapidly building custom user interfaces.
Tailwind css basic requriment file.

This files are very important coding for <a href="https://tailwindcss.com/">tailwindcss.</a>


<h2>You can install these files form Postcss from <a href="https://tailwindcss.com/docs/installation/using-postcss">tailwind website</a></h2>

Install Tailwind CSS
Install tailwindcss and its peer dependencies via npm, and create your tailwind.config.js file.

Terminal


npm install -D tailwindcss postcss autoprefixer

npx tailwindcss init

Add Tailwind to your PostCSS configuration

Add tailwindcss and autoprefixer to your postcss.config.js file, or wherever PostCSS is configured in your project.




postcss.config.js



module.exports = {

  plugins: {
  
    tailwindcss: {},
    
    autoprefixer: {},
    
  }
  
}




Configure your template paths

Add the paths to all of your template files in your tailwind.config.js file.

tailwind.config.js


module.exports = {

  content: ["./src/**/*.{html,js}"],
  
  theme: {
  
    extend: {},
    
  },
  
  plugins: [],
  
}




main.css

@tailwind base;

@tailwind components;

@tailwind utilities;


Start your build process
Run your build process with npm run dev or whatever command is configured in your package.json file.

Terminal

npm run dev


Start using Tailwind in your HTML
Make sure your compiled CSS is included in the <head> (your framework might handle this for you), then start using Tailwind’s utility classes to style your content.

