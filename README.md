# adam-css-funtime

<h2>About the Enviroment</h2>
- No node.js > No Require syntax or npm. Scripts are called above the last ```<body>``` tag, need to call jquery library direct via CDN
- No babel > No ES6 syntax
- No SASS > No ```@import``` css -- call it in the head <link rel="stylesheet" type="text/css" href="mystyle.css">
- No bootstrap > No col-3 or fluid container
- No Grunt > test locally with ```ruby -r un -e httpd . -p 7165```
- No Github cheatery...(better make sure you're not on master)
- Naked AF repo...back to basics

Mantras....
- Biggest Squares first!!!!!!!!
- Put a boarder on it (or a background-color)
- Mind your overflows
- (Groups of things that might move together belong in their own box)

<h3>Block vs Inline `&` Positioning</h3>
(demo block and inline elements , default styles > reset)
Floats n Clears
- Take element out of normal flow/order of nodes
- Overflow vs empty clear div (throw in clipping mask with hidden)
- What's a clearfix? (demo nav + 2 column + footer layout)
- Refer to Lynda video
  http://cssmojo.com/latest_new_clearfix_so_far/

Absolute vs relative


<h3>Selectors vs Psuedo Selectors</h3>
CSS Sushi Selector game: http://flukeout.github.io/
List of Selectors: http://www.w3schools.com/cssref/css_selectors.asp
Child Selector Game: https://css-tricks.com/examples/nth-child-tester/
Research specificity on your own (see the calculator) https://specificity.keegan.st/
Psuedos and Jquery? DOM load order?


<h3>Responsive Elements + Layout:</h3>
(demo fixed widths vs percentages vs viewport heights/widths)

img {
    width: 100%;
    height: auto;
}

Same as...

div {
  width: 100%;
  padding-bottom: 100%;
}

Same as...

div {
  width: 100vw;
  height: 100vh;
}

<h3>Media Queries:</h3>
Design for Orientation -- Landscape or Portrait
Take a look at desktop > mobile design transitions...what do you see? (When do we stack shit?)
http://mediaqueri.es/

No need for complete perfection...Only 4 major browser widths!
Bootstraps major break points: https://v4-alpha.getbootstrap.com/layout/overview/

Do mobile/break up CSS in 2 ways:
  1.) Break it up by device: Call 4 seperate style sheets for major device widths
  2.) Break it up by feature + media quieries within style sheet

Example:
  1.) <link rel="stylesheet" media="(max-width: 800px)" href="example.css" />

  2.)

<style>
  @media (max-width: 600px) {
    .facet_sidebar {
      display: none;
    }
  }
</style>

Mobile First....?
http://www.w3schools.com/css/css_rwd_mediaqueries.asp

Control Landscape:
@media only screen and (orientation: landscape) {
    body {
        background-color: lightblue;
    }
}

Why doesn't my site resize on my phone?
https://akadane87.github.io/portfolio/
https://akadane87.github.io/dojo/
<!--<meta name="viewport" content="width=device-width, initial-scale=1"> -->
https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag
http://www.kylejlarson.com/blog/iphone-6-screen-size-web-design-tips/


<h3> Mobile Nav in strictly CSS (why doe?)</h3>


<h3>Challenge: Rebuild this page...</h3>
http://millennium-consulting.com/

How is the nav broken up/ where is there style repitition amongst element relationships?
What are the break points?
What kind of font are they using?
Can I use their logo?
What other assets can I steal? (make a folder)

(Next coding challenge brand it to the company. That much closer to a company project)


<h3>SVG and GreenSockAnimationPlatform Demo:</h3>
CSS vs Jquery animations: https://css-tricks.com/myth-busting-css-animations-vs-javascript/
20x faster than jquery  https://greensock.com/get-started-js
Pluggin https://greensock.com/draggable
