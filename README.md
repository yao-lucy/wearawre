## Description
First, my program iterates through the input data and aggregates the data using dictionaries. Then, it deletes any existing data and inserts the new aggregated data into the given Notion database using the Notion API. Run the program by running the `notion_exercise.py` file and entering the input data file path.

## Short Answers
**Was there anything you got stuck on, and if so what did you do to resolve it?**

I was not sure what the best way to aggregate the input data was. I was debating between (1) keeping a running ratings sum, ratings count, and favorites count for each book or (2) calculating the average rating and favorites count at the end. The performance of both would be similar as it does not increase time or space complexity by any order, but I felt like there should be a more "correct" option. I ended up going with option (1) because I felt like it could be more efficient if the program expanded features though it might be less readable.

Other areas to consider include handling edge cases (considered in the comments), adding asynchronous compatibility, and writing log statements for debugging.

**Do you have any suggestions for improving the API documentation to make it clearer or easier to use?**

I thought the API documentation was pretty clear and easy to use once I got over the initial learning curve. Once I realized that database rows were treated as pages, everything started to click. While there are a few Python examples, it could also be nice to include some more examples in Python rather than just JavaScript.

## Resources
- https://stackoverflow.com/questions/71918703/visual-studio-code-pylance-report-missing-imports
- https://github.com/ramnes/notion-sdk-py
- https://developers.notion.com/docs/create-a-notion-integration
- https://developers.notion.com/reference/post-database-query
- https://developers.notion.com/reference/archive-a-page
- https://developers.notion.com/docs/working-with-databases#adding-pages-to-a-database

## Libraries
N/A
