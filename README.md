# Welcome to Microblog-Verify!

This is the example application featured in my [Flask Mega-Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world), to which I've added support for two-factor authentication via the [Twilio Verify API](https://www.twilio.com/docs/verify/api).

## How To Run This Application

Microblog is fairly complex application that is developed over the 23 chapters of the tutorial referenced above. Below you can see how to start the basic application using a local SQLite database, and without including support for emails, full-text search and background tasks. This is enough to demonstrate how to add two-factor authentication.

1. Create a Python virtual environment and activate it:

    *For Unix and Mac computers:*

    ```
    $ python3 -m venv venv
    $ source venv/bin/activate
    (venv) $ _
    ```

    *For Windows computers:*

    ```
    $ python3 -m venv venv
    $ venv\bin\activate
    (venv) $ _
    ```

2. Import the Python dependencies into the virtual environment:

    ```
    (venv) $ pip install -r requirements
    ```

3. Create a local database:

    ```
    (venv) $ flask db upgrade
    ```

4. Start the development web server:

    ```
    (venv) $ flask run
    ```

5. Access the application on your web browser at `http://localhost:5000`

Interested in learning more about this application besides two-factor authentication? The [actual tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world) is the best reference!
