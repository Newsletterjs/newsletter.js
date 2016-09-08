# Newsletter web application

Opensource newsletter application build with node.js

## Features:

- Multiple Newsletter
- Categories in every newsletter
- Email builder
- User subscribe and unsubscribe
- SPA Administration


## How to run

### First clone the code:

Clone and load subrepositories with:

Clone:

```sh
git clone https://github.com/videoteca/videoteca.git
```

Enter in project folder:

```sh
cd videoteca
```

Load all submodules (admin and api):

```sh
git submodule update --init --recursive
```

### With local installation

### With docker compose

```
docker-compose up -d
```


## Roadmap:

- API
  - Implement the email template load and email template file structure
    - Email template need:
      - settings file (index.js) 
        - this file need to return one instance of EmailTemplate class 
      - instance of EmailTemplate class (new)
        - create method
        - update method
        - delete method
      - html form (form.hbs) 
      - preview image (preview.png)
      - email files (see email-templates npm module):
        - html.{ext}
        - text.{ext}
        - style.less
  - Add suport for send emails with cron and max send per run (we.js commands + we.js cron features)
- Client / site
  - Add one for each newslleter with newslleter data and subscription form or unsubscribe form
  - Login form
- Admin
  - add an authentication strategy (JSON web tokens or Oauth password grant method)
  - Create pages with:
    - logged in user email templates
    - all logged in user newslleters
    - create email with email tempalte form
    - edit email
    - preview email (may be in edit email ...)
    - Send email action

## Stack

- We.js - server side api
- Ember.js - admin
- git - versionamento

# License:

The MIT License (MIT)

Copyright (c) 2016-2017 Alberto Souza

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.