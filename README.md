# Newsletter Sign-Up

This is a simple newsletter sign-up application built with Node.js and Express. It allows users to sign up for a newsletter by providing their first name, last name, and email address. The application then sends this data to Mailchimp for managing the mailing list.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Files](#files)
- [Contribution](#contribution)


## Installation
1. Clone the repository:
```bash
git clone https://github.com/Ashish-Chokhani/Newsletter-Sign-Up.git
```
2. Navigate to the project directory:
```bash
cd Newsletter-Sign-Up
```

3. Install dependencies:
```bash
npm install
```

4. Set up your Mailchimp API key and List ID:
- Replace 'YOUR_API_KEY' and 'YOUR_LIST_ID' in app.js with your Mailchimp API key and list ID.

```bash
let options = {
    url: 'https://usX.api.mailchimp.com/3.0/lists/YOUR_LIST_ID',
    method: 'POST',
    headers: {
        "Authorization": "anystring YOUR_API_KEY"
    },
    body: jsonData
}
```

5. Start the application:
```bash
node app.js
```

6.Open your browser and navigate to http://localhost:3000.

## Usage
- Fill in the sign-up form with your first name, last name, and email address.
- Click the "Sign in" button.
- If the sign-up is successful, you will be redirected to the success page.
- If there is an error, you will be redirected to the failure page where you can try again.


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

## Files
**app.js**
This is the main file that sets up the Express server and handles the routes.

**failure.html**
This file contains the HTML for the failure page which is shown when there is an error during sign-up.

**signup.html**
This file contains the HTML for the sign-up page where users can enter their details.

**success.html**
This file contains the HTML for the success page which is shown when the sign-up is successful.

**public/css/styles.css**
This file contains the custom styles for the sign-up form.

## Contribution
We welcome contributions! Feel free to fork the repository, make changes, and submit a pull request.

