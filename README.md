# NewsletterApp_Using_Mailchimp_API
Newsletter subscription frontend that connects to expressJs backend and uses Mailchimp API to add to your subscription list and then\
you can send them your spams anytime

## Try it out
Test by Clisking [HERE](https://chambray-shrub-composer.glitch.me/)

## Usage
Its pretty simple, can make it fit your own need, just follow the step

```bash
npm i
```
It will install the following modules: Express, Body-parser, request and nodemon\

## Navigate the proj
Index.js is the main run file\
.html files are explained as by their names and what they do (The template is from bootstrap examples)\
public folder contains the image and css file so they can be GET successfully\
You can change the image, placeholders and links in html files

## Use your api key

```js
var options = {
    url: "https://us21.api.mailchimp.com/3.0/lists/" + process.env.LIST_CODE,
    method: "POST",
    headers: {
      Authorization: `auth ${process.env.AUTH_KEY}`,
    },
    body: jsonData,
  };
```
create .env file and declare it there by: AUTH_KEY and LIST_CODE\
generate your own mailchimp api key and place it in .env file by the name AUTH_KEY or place direclty in index.js\
same goes for you own LIST_CODE

THATS ALL
