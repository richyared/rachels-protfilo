# Rahel — Personal Portfolio

This package keeps the original portfolio's main sections and PHP/MySQL message-form idea, updated with:
- Name: **Rahel**
- Soft water-blue and pink theme
- Email: **rahelyared30@gmail.com**
- GitHub: **https://github.com/rahelyared**
- A password-protected `messages.php` inbox

## Files
- `index.php` — main portfolio page and contact form
- `messages.php` — private inbox for submitted messages
- `style.css` — responsive water-blue/pink styling
- `config.example.php` — sample local database and inbox settings
- `.gitignore` — keeps your real `config.php` out of Git

## Important: PHP hosting is required
GitHub Pages only publishes static files; it does not execute PHP or connect to MySQL. This portfolio needs a PHP host with MySQL support. You can test it locally with XAMPP.

## Run locally with XAMPP
1. Copy this folder into `xampp/htdocs/rahel-portfolio/`.
2. Make a copy of `config.example.php` named `config.php`.
3. Open `config.php`. Set your database username/password and replace the inbox password with a long private password.
4. Start **Apache** and **MySQL** in XAMPP.
5. Visit `http://localhost/rahel-portfolio/`.
6. Open `http://localhost/rahel-portfolio/messages.php` to sign in to your private inbox.

The PHP pages create the database and messages table on first use, provided the database account has permission to create databases. Otherwise, create a database named `rahel_portfolio` in phpMyAdmin first.

## Before publishing
- Keep `config.php` private and never upload it to a public repository.
- Use a unique inbox password. Do not reuse your GitHub password.
- The email address appears publicly on the portfolio, as requested.
- Test the contact form and inbox on your PHP host before sharing the site.
- If you use a hosting provider, enter its database details in `config.php`.

## About the template
The available GitHub commit snapshot showed the original PHP page and inbox source, but did not include the original CSS diff. The stylesheet in this package is a recreated matching stylesheet for the same page structure, with the requested blue/pink palette; it is not a byte-for-byte copy of the unavailable original CSS.


## Publish a static preview with GitHub Pages
The repository also includes `index.html`, a static preview for GitHub Pages. It preserves the portfolio layout and uses email/GitHub contact links. The PHP contact form and private inbox require PHP/MySQL hosting and will not run on GitHub Pages.

To publish the preview: open the repository on GitHub, go to **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/(root)**, then save. Wait for GitHub Pages to publish and use the URL shown in the Pages section.
