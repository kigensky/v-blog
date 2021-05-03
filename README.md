##  V-BLOG
# Author

[victor-kigen](https://github.com/kigensky)

## Description
This is a flask application that allows writers to post blogs, edit and delete blogs. It also allows users who have signed up to comment on the blogs that has been posted by a writer. It also allows a person to subscribed to recieve email everytime a new blog is posted by a writer.

You can view the site at:[HEROKU](https://hakika2.herokuapp.com/)

# User Stories
These are the behaviours/features that the application implements for use by a user.

As a user I would like to:
* A user can view the most recent posts.
* View and comment the blog posts on the site.
* A user should an email alert when a new post is made by joining a subscription.
* Register to be allowed to log in to the application
* A user sees random quotes on the site
* A writer can create a blog from the application and update or delete blogs I have created.

# Specifications

## Specifications
| Behaviour | Input | Output |
| :---------------- | :---------------: | ------------------: |
| Load the page | **On page load** | Get all blogs, Select between signup and login|
| Select SignUp| **Email**,**Username**,**Password** | Redirect to login|
| Select Login | **Username** and **password** | Redirect to page with blogs that have been posted by writes and be able to subscribe to the blog|
| Select comment button | **Comment** | Form that you input your comment|
| Click on submit |  | Redirect to all comments tamplate with your comment and other comments|
|Subscription | **Email Address**| Flash message "Succesfully subsbribed to V-Blog"|


### Running the Application
To get the code..

1. Cloning the repository:
  ```bash
  https://github.com/kigensky/v-blog
  ```
2. Move to the folder and install requirements
  ```git
  cd V-Blog
  pip3 install -r requirements.txt
  ```
3. Exporting Configurations
  ```git
  export SQLALCHEMY_DATABASE_URI=postgresql+psycopg2://{User Name}:{password}@localhost/{database name}
  ```
4. Running the application
  ```git
  python3 manage.py server
  ```
5. Testing the application
  ```git
  python manage.py test
  ```
Open the application on your browser `127.0.0.1:5000`.


## Technologies Used

* [Python3.6](https://www.python.org/)

* [Flask](http://flask.pocoo.org/)

* [Heroku](https://heroku.com)

## known Bugs
* There are no known bugs currently but pull requests are allowed incase you spot a bug

## License
[MIT](https://choosealicense.com/licenses/mit/)

Copyright (c) 2021 victor kigen

