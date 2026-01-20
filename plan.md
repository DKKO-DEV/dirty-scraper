###DIRTY WEB SCRAPER

The plan is to scrap the web [BooksToScrape](https://books.toscrape.com/), getting and storing in a csv file the following data:

*Title -> STR
*Price -> FLOAT, no currency symbols.
*Star Rating -> INT
*Avaliability -> BOOL

To track this data embbeded in the web, I'll need to target specific CSS selectors. I haven't touched front-end dev at all, but from looking at the internet and inspecting the .html pages my initial belief (21/01/2026 - 0:41h CET) is that i can get all the info that I want from the following selectors respectively:

*.product_pod h3 (.product_pod is the general selector where all info for each book is at, I believe.)
*.product_price
*.reviewrating OR .star-rating (.One/.Two/.Three...)
*.avaliability (.instock/.outofstock)