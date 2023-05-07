# flask-blog-page-with-api
This code creates a simple blog web application using the Flask framework. The application defines two URL routes: / and /post/<int:index>.

The get_all_posts() function is called when the / route is accessed. It renders the index.html template and passes all the blog posts to the template using the render_template() function.

The show_post(index) function is called when the /post/<int:index> route is accessed. It retrieves the requested post by searching for the post with the given index in the list of blog posts. Once the requested post is found, it renders the post.html template and passes the requested post to the template using the render_template() function.

Additionally, the statement app.run(debug=True) runs the Flask application in debug mode, which allows detailed error messages to be displayed during the development process.

The application also depends on a separate file named post.py. This file contains the Post class, which represents the blog posts and allows the creation of objects to represent individual posts. The Post class has properties such as post ID, title, subtitle, and body.

With this setup, you can run your Flask blog application and view the blog posts in your web browser.
