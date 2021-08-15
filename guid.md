<!-- To Build tailwind css in desire folder -->

"scripts": {
"build-css":"tailwindcss build src/styles.css -o public/styles.css"
},

<!-- to get full tailwind css config file -->

=> npx tailwindcss init --full

<!-- for only simple config file -->

=> npx tailwindcss init

<!-- custom font -->

To add custom font we have to add font import link in styles.css file inside srt folder ,Not public folder. after have to add name and font name in config file...

<!--  @apply -->

Use @apply to inline any existing utility classes into your own custom CSS.

here, we can write plain css and tailwind class with @apply method
ex:
.btn {
transform: translateY(-1px);
@apply bg-black;
}

/_ Output _/
.btn {
background-color: #000;
transform: translateY(-1px);
}

<!-- problem -->

@apply directice doesn't work
