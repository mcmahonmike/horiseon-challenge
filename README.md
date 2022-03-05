# Horiseon Code Refractor Challenge

An overview of all the changes made to the HTML and CSS stylesheet for the Horiseon website. 
These changes include adding semantic HTML to the existing code, adding alt attributes to the images, creating a logical title for the website as well as consolidating the CSS Styles in the style sheet.

## HTML Changes

Starting from the top elements down, I updated the `<title>` element in the head to read as **Horiseon** to better reflect the name of the website. Followed by adding semantic elements to the `<div class="header">` replaced as  `<header>` as well as repalcing the following `<div>` element with a `<nav>` element.
Other semantic elements that were updated are as follows:
*  `<div class="hero">` to `<section class="hero">`
*  `<div class="benefits">` to `<aside class="benefits>`
*  `<div class="footer">` to  `<footer>`

Next I consolidated class atributes to reduce repetion throughout the page and to better consolidate the CSS stylesheet. 
The class attributes that were consolidated are as follows:

**Within the Hero Section**

*  `class="search-engine-optimization"` `class="online-reputation-management"` `class="social-media-marketing"` consolidated to `class="cell"`

**Within the Aside Section**

*  `class="benefit-lead"` `class="benefit-brand"` `class="benefit-cost"` consolidated to `class="benefit"`

The last updates to HTML were adding alt attributes to all the images within the Horiseon website.
The alt attributes that were added are as follows:

**Within the Hero Section**

* `<img src="./assets/images/search-engine-optimization.jpg"` added alt attribute 
`alt="a notepad with SEO written on it as well as a cup of coffee and a laptop resting on a wooden surface"`
* `<img src="./assets/images/online-reputation-management.jpg"` added alt attribute `alt=" a person working on a laptop which on it has a bar graph and the word reputation on the screen"`
* `<img src="./assets/images/social-media-marketing.jpg"` added alt attribute `alt="a team of six working at a large table with colorful stickers with social media buzz words"`

**Within the Aside Section**

* `<img src="./assets/images/lead-generation.png"` added alt attribute `alt="a gear being funneled into a coin with a dollar sign, and an arrow on the funnel pointing from the gear to the coin "`
* `<img src="./assets/images/brand-awareness.png"` added alt attribute `alt=" a person in a suit with a lightbulb for a head with wave signals emulating from the lightbulb"`
* `<img src="./assets/images/cost-management.png"` added alt attribute `alt="a gear with three coins postioned in front of it with each coin having a dollar sign on it"`


That completes all the changes made to the HTML (index.html)


## CSS Changes
Again starting from the top down the changes to the CSS are as follows: all .header styles were updated to be header, removing the "." since the class="header" was removed from the HTML.
All "div" children were replaced with "nav" within header styles. In .content `position: relative;` and `top: 825px;` was added too move the .content section down to the bottom of the page to be inline with the aside.
In the .benefits added `position: static;` to move the aside section to the bottom of the page, inline with the .content.
Then consolidated styles to match the added classes inputed into the HTML.
* `.benefit-lead` `.benefit-brand` `.benefit-cost` styles consolidated into one `.benefit` style
* as well as their children styles `h3` and `img` consolidated into `.benefits h3` and `.benefits img`
* `.search-engine-optimization` `.online-reputation-management` `.social-media-marketing` styles consolidated into one `.cell` style
* as well as their children styles `img` and `h2` consolidated into `.cell img` and `.cell h2`
And finally the ".footer" style was updated to "footer"

That completes the style changes added to the CSS (style.css)
