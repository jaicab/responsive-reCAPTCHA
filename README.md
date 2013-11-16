#responsive reCAPTCHA

A responsive theme for <a href="https://www.google.com/recaptcha">reCAPTCHA</a>. I needed a reCAPTCHA for a responsive web site and the default theme didn't fit on screens smaller than 300px. So I decided to build a mobile-first, icon-free theme.

<img src="https://raw.github.com/jaicab/responsive-reCAPTCHA/master/example.jpg" alt="example">

Supported in all modern browsers and:
* Internet Explorer 8.0+
* Firefox 2.0+
* Chrome 4.0+
* Safari 3.1+
* Opera 9.6+

##How-to
Before copy-pasting this, please remember that you'll need a public and private key to make reCAPTCHA work. In this case you'll see this URL two times at the end of the code: `http://www.google.com/recaptcha/api/challenge?k=YOUR_PUBLIC_KEY`

You'll have to replace YOUR_PUBLIC_KEY with the one you'll get at <a href="https://www.google.com/recaptcha/admin/create">reCAPTCHA's site</a>.
Also, you'll have to consider that:
- You must include this before the `form` opening tag.

```html
 <script type="text/javascript">
 var RecaptchaOptions = {
    theme : 'custom',
    custom_theme_widget: 'responsive_recaptcha'
 };
 </script>
 ```
- You must include all the HTML and CSS. But don't worry, all the CSS is specified by `#responsive_recaptcha` id so copy&paste won't be a problem.
- If you want a fallback, you may want to leave the `noscript` where it is.

##Customising
I built this using LESS so it would be easy to customise if you wanted to. All the colors and margins depend on the variables at the top of the LESS file.
Also you can change the text in the HTML if for example, you want to translate it. But I don't recommend changing the HTML code if you want it to stay responsive.

##License
responsive reCAPTCHA by Jaime Caballero is licensed under a Creative Commons Attribution 3.0 Unported License. http://creativecommons.org/licenses/by/3.0/