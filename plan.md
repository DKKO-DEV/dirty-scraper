### DIRTY WEB SCRAPER

The plan is to scrap the web [BooksToScrape](https://books.toscrape.com/), getting and storing in a csv file the following data:

* Title -> STR
* Price -> FLOAT, no currency symbols.
* Star Rating -> INT
* Availability -> BOOL

To track this data embbeded in the web, I'll need to target specific CSS selectors. I haven't touched front-end dev at all, but from looking at the internet and inspecting the .html pages my initial belief is that i can get all the info that I want from the following selectors respectively:

* a -> <a title="'>
* .price_color
* .star-rating (.One/.Two/.Three...)
* .availability (.instock/.outofstock)
