### Adding posts

Create a file in the _posts/(category ID) directory for the category you want it to appear in.

Name the file (year)-(month)-(day)-(post-name-with-dashes).md, e.g. *2015-01-01-my-example-coin.md*

This is the example code, make sure you change the category to match the one you put it in:

    ---
    layout: page
    category: coins
    title: My Example Coin
    image: https://placekitten.com/g/200/300
    ---

    Example coin goes here

It will be put in the right places on the site. Posts are sorted by most recent first by default.

### Adding categories

This is a bit more involved.

Create a file in _data/categories, called (categoryid).yml, using this template fill in the data:

    name: Coins
    image: https://placekitten.com/g/200/300
    description: Take a look at my coin collection!

Then, create a directory called the category ID then make an index.html file in it with the following template (make sure you change the id to match):

    ---
    layout: category
    id: coins
    ---

Then make a folder with the category ID in the _posts directory, and create a post using the instructions above using your new category ID.