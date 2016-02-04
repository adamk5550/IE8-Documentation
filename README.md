# IE8-Documentation

## The Reality of Developing for IE8 in 2016 and beyond. :cry:

![alt text](IE8Memes/thisisfine.png?raw=true)

So you've found yourself on this page and your thinking oh but i need to support IE6 and/or IE7 as well? I'm sorry i can not help you, no one can help you...

Effective January 12, 2016, Internet Explorer 8 is no longer supported on any version of Windows. <strong> Rejoice </strong> :tada:


## HTML

<p>IE provides basically no support for HTML5 which is the most recent version of HTML and has been for the past 5 years. For example IE8 will not support such things as section, article, nav, header, footer, aside and canvas tags. This isn’t really to much of an issue because the tags mentioned above besides canvas are semantic elements and therefore don’t function to much differently than your standard div tag. IE8 and all other browsers should handle unknown elements as inline-elements so you can add some simple CSS to make them act like they should</p>

```CSS
header, section, footer, aside, nav , main, article, figure {
	Display: block;
}```

<p>You can also teach older browsers to handle HTML5 features and there is a full feature on how available at http://www.w3schools.com/html/html5_browsers.asp</p>

<p>Additionally, IE8 does not support SVG elements which means that you cant use popular graphical library’s such as D3.js</p>

<p>One of the tools which you should look into is modernizr.js library which will provide feature-detection letting you support IE8 easier. While there may be ways to hack around this it ultimately is not work the development effort.</p>


## CSS

<p>IE does not fully support CSS3 therefore if you want full CSS support you would have to use CSS2.1. </p>

<p>This means that you cannot key features such as :</p>
* Media Queries
* Keyframes
* Transform and Transition
* Nth of type or nth-child selectors

<p>There is a library you can use to try and patch some of these features called  http://selectivizr.com/ which may help</p>

<p>Additionally, you may come across some strange activity when using popular CSS frameworks, however the most successful CSS framework to use would be bootstrap. However, there are no guarantees that you will have full support.</p>

<p>IE8 is famous as the devil in browser form for many reasons one of these being to do with the CSS. God help you if something’s not correctly placed when it should be it will take over the next 3 days of your life… </p>

![alt text](IE8Memes/ie8.jpg?raw=true)

## JavaScript
