# Data Description

There are five tables, as follows:

`books` Contains data on books:

- `book_id`
- `author_id`
- `title`
- `num_pages` — number of pages
- `publication_date`
- `publisher_id`

`authors` Contains data on authors:

- `author_id`
- `author`

`publishers` Contains data on publishers:

- `publisher_id`
- `publisher`

`ratings` Contains data on user ratings:

- `rating_id`
- `book_id`
- `username` — the name of the user who rated the book
- `rating`

`reviews` Contains data on customer reviews:

- `review_id`
- `book_id`
- `username` — the name of the user who reviewed the book
- `text` — the text of the review

# Purposes
- To generate a value proposition for a new product (books) based on a database of one of the services competing in the market of startups that rushed to develop new apps for book lovers.
        
# Libraries
*pandas, numpy, sqlalchemy* 
