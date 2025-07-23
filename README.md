# TailwindCSS-Learning
This repository contain all steps of learning Tailwind from zero to production.

## How to install Tailwind in Vs Code

### Steps
1. Create Folder for your project.
2. Inside of your project folder create other two folders :
    A. public, it will contain your input files 
            For Example: index.html , styles.css
    B. output, it will contain your output files. 
3. You need to search for Tailwind Documention on Tailwind CLI but first you have
                     to check if you have node in your pc if not install it then preceed by Install Tailwind CSS
                    Install tailwindcss and @tailwindcss/cli via npm.

4. Import Tailwind in your Css by Add the @import "tailwindcss"; import to your main CSS file. 
                In this project, I imported it in styles.css from public folder.
5. Start the Tailwind CLI build process:
        Run the CLI tool to scan your source files for classes and build your CSS.
        By using this command npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
        but here i have changed this command by changinging folder for input from src to public and input.css to styles.css as it's in my project and also for output I changed also src to ouput as name of folder in this project. Then I runned it in terminal.
    
6. In your html file from public folder in head section link your output css file in ouput folder.
7. You must install Tailwind plugin before proceeding with the project which is (Tailwind CSS IntelliSense).
8. Proceeding with your project start designing.
9. Final step: Create a name for the script that will run everytime you open Vs Code instead of  
        copying and  pasting the whole the whole CLI command. like this 
        "scripts": {
            "tailwind:run":"npx @tailwindcss/cli -i ./public/styles.css -o ./output/output.css --watch"
        }