## Flask Application Design

### HTML Files

**index.html**
- This will be the main page of the application, responsible for displaying the recent news articles.
- It will contain HTML elements to showcase the articles, such as a list with article titles and links.

**article.html**
- This page will show the full content of a specific news article when a user clicks on its title.
- It will retrieve the article's content from the database or another data source and display it within the HTML structure.

### Routes

**@app.route('/index')**
- This route will handle the display of the index page (index.html).
- It will query the database or other data source to retrieve the recent news articles and pass them to the index.html template for rendering.

**@app.route('/article/<int:article_id>')**
- This route will handle the display of the full article based on its ID (article_id).
- It will retrieve the article's content from the database or another data source and pass it to the article.html template for rendering.