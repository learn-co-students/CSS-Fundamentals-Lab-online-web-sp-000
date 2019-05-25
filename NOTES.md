# *CSS* FUNDAMENTALS

1. adding style to our index.html page by linking an external CSS file.
```html

<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Exceptional Realty Group - Luxury Homes - About</title>

        <!-- Don't forget to link your CSS file! -->
        <link rel="stylesheet" href="relative path to CSS file">

    </head>
    <body>
        <header>
        <!-- logo -->
        <h1>Exceptional Realty Group</h1>

        <nav>
            <a href="index.html">About</a> <a href="new-properties.html">New Properties</a> <a href="real-estate-listings.html">Listings</a> <a href="market-report.html">Market Report</a> <a href="contact.html">Contact</a> <a href="http://hud.gov" target="_blank">H.U.D.</a>
        </nav>
        </header>

    </body>
</html>

```
Links to stylesheets should go at the end of the <head> section! Make sure you provide a relative path to the stylesheet.

What is a relative path?
You could write href="style.css" and the content of style.css
would change your index.html file.

#But we want to teach you to require external resources
#(*CSS or JavaScript*) by using relative paths.

*Relative paths* make it crystal clear which file is being used.

Relative paths start with './' which means:
"from the directory I am currently in."

When using links to associate a stylesheet, href="./style.css" refers to:
"From the directory in which I, the index.html file live"

look for a file called style.css and use it.

This pattern will help you and other developers remove any possible confusion.

# *Hint*: Try adding the following temporarily to your style.css file to test if your linked CSS is working:
```css

    h1 {
        color: red;
    }

```
