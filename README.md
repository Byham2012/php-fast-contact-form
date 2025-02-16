# Fast & Secure PHP Form with reCAPTCHA v3

## Overview
This is a lightweight, fast-loading contact form built with PHP and Google reCAPTCHA v3 for spam protection. It securely sends user submissions to an email address and can be easily customized.

## Features
- Fast-loading (No bloated frameworks)
- Secure (reCAPTCHA v3 anti-spam protection)
- Easy Setup (Works with PHP mail function)
- Customizable (Modify fields, styles, and actions)

## Files Included
- `index.php` → The form page
- `send_email.php` → Handles form submission & sends email
- `styles.css` → Optional styling for form layout
- `thank-you.html` → Confirmation page after successful submission

## Setup Instructions
### 1. Clone the Repository
```sh
 git clone https://github.com/Byham2012/php-fast-contact-form.git
```

### 2. Upload Files to Your Server
Place all files inside your `public_html/` or a subdirectory (e.g., `contact-form/`).

### 3. Update Your reCAPTCHA Keys
- Get your Google reCAPTCHA v3 keys from [Google reCAPTCHA](https://www.google.com/recaptcha/admin)
- Open `index.php` and replace `your-recaptcha-site-key` with your actual Site Key:
```html
<script src="https://www.google.com/recaptcha/api.js?render=your-recaptcha-site-key"></script>
```
- Open `send_email.php` and replace `your-recaptcha-secret-key`:
```php
$recaptcha_secret = "your-recaptcha-secret-key";
```

### 4. Configure Your Email
In `send_email.php`, update the recipient email address:
```php
$to = "your-email@example.com"; // Change this to your email
```

### 5. Test Your Form
- Open `index.php` in your browser
- Fill out the form & submit
- Check if you receive the email at your configured address

## License
MIT License - Free to use and modify.

## Contributing
If you'd like to contribute or improve the project, feel free to submit a pull request.

## Credits
Developed by [Tanzi Bee] (https://webhoney.digital). Inspired by the need for fast-loading, secure contact forms.

---
### Live Demo & Tutorial
- Demo: https://webhoney.digital/logo-initial-consultation-discovery/
- Tutorial on Dev.to: [Read Here] (https://dev.to/tanzi_bee/)
