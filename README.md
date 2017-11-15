# Contact form without backend

It's a responsive modal, activated on button and validated by Javascript. Error messages are displayed if something is wrong.
It uses [formspree.io](https://formspree.io/) for sending emails. All you need is HTML, Javascript and JQuery.

See it [here](https://c0deboy.github.io/contact-form-no-backend/).

Steps to get it working:

1. Copy JS and CSS file to your project.

2. Include all elements from `index.html` (from both `<body>` and `<head>` sections).

3. Translate text and messages if needed.

4. Specify your email adress in HTML form at `action` attribute:
``` HTML
<form class="emailForm" method="POST" action="https://formspree.io/your.email@example.com">
```

5. Get your [reCAPTCHA V2](https://www.google.com/recaptcha/admin) site key nad copy paste it at `data-sitekey` attribute.
``` HTML
<div class="g-recaptcha" tabindex="-1" data-sitekey="6Lc9_xMUAAAAAFPVNhvDKb9lMXHGI4o7-zhqkTgL"
                 data-callback="recaptchaClearErr"></div>
```

6. Send first email to yourself. You'll get email from formspree.io where you can confirm, that you want receive emails from this site.

7. Done
