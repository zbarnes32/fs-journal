Date: June 4th

HTML & CSS

Some notes in separate VSCode file named PetCare (pasted down below).


--Copied from VSCode--

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport"
    content="width-device-width, initial-scale-1.0">
    
    <link rel="stylesheet" href="style.css">

    <title>Document</title>
</head>

<body>
    <!-- Header just creates a block, it's value is in the semantic nature of the tags names -->
    <header>
        <!-- Div is a simple division, creates a box -->
        <div>
            <span class="logo">
            Pet.Care
        </span>
            <a href="">Home</a>
            <a href="">About</a>
            <a href="">Product</a>
            <a href="">Service</a>
            <a href="">Trainers</a>
        </div>
            <button>Sign Up</button>
    </header>

    <main>
        <!-- Main, also creates just a block on the page, but the semantic nature is good practice -->
        <div>
            Left
        
        </div>
        <div>
            Right
            <!--<img src="">Image of a dog -->
        </div>
    </main>
</body>


</html>

-- End of HTML Copy --

-- Start of CSS Copy --

/* Debug styles */

main *{
    /* this rule will target ALL elements within the main */
    outline: 1px red dashed;
}


body{
    
}

/* Trying to layout elements should not be done with margin OR padding, those ... */
span {
    
}

button {
    
}

header {
    font-size: 20px;
    display: flex;
    justify-content: space-between;
    border-bottom: 1px black solid;
    padding-bottom: .75em;
    /* em, is a multiple of the font-size of the element, standard font size is 16px, so .75 times 16px is 12. */
}

main {
    display: flex;
}

.logo {
    /* pixels are absolute measurements and CAN cause issues when certain things like screen size or text size change */
    margin-right: 30px;
}

-- End of CSS copy --

Images will default to actual px size of the picture. A way to fix this is to add styles to it.
Create a class to specialize styles. 

##HTML Semantic Hierarchy

<html>

<head>
<style></style>
</head>

<body>
<header></header>
<main>
</main>
<footer>
</footer>
</body>

</html>

holding 'alt' while selecting HTML tags allows you to edit multiple tags at once.

to get suggestions back in VSCode, hit control + space ??

Creating specialty classes can help save time as apposed to styling each element type.

background-color: unset; -- removes the background color of the button itself.

If you hover over the css selector in VSCode, you can view the specificity.

!important should not be used to overwrite rules.

in CSS, hv is a percentage of the view height. 
for example height: 100hv; -- would allow the screen height be the full screen height
that paired with "flex-grow" in the body section fills the full webpage, allowing the body section to grow instead of whitespace under the footer. 

overflow-y: scroll; would allow a scrollable body instead of a scrollable page. 