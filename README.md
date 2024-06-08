# Newsletter Sign-Up

This is a simple newsletter sign-up application built with Node.js and Express. It allows users to sign up for a newsletter by providing their first name, last name, and email address. The application then sends this data to Mailchimp for managing the mailing list.

## Directory Structure

```bash
Newsletter-Sign-Up
│   .DS_Store
│   .gitignore
│   app.js
│   date.js
│   failure.html
│   package-lock.json
│   package.json
│   signup.html
│   success.html
│
├───public
│   ├───css
│   │       styles.css
│   │
│   └───images
│           application.png
│
└───views
    ├───about.ejs
    ├───footer.ejs
    ├───header.ejs
    └───list.ejs
```

## Installation
1. Clone the repository:
```bash
git clone https://github.com/Ashish-Chokhani/newsletter-sign-up.git
cd newsletter-sign-up
```

Install dependencies:
bash
Copy code
npm install
Set up your Mailchimp API key and List ID:

Replace 'YOUR_API_KEY' and 'YOUR_LIST_ID' in app.js with your Mailchimp API key and list ID.
