# Welcome to Library Loops!

You have a massive collection of books; many you've read, many you have not! You've read so many, it's been hard to keep track of the information about these books. In order to keep track of all of your books, you've decided to catalogue them all, keeping track of specific data about each book.

Now you have your collection, minified to an array called library. This array contains hashes that represent each book, keeping track of the book's title, author, genres, publication year, number of pages, and whether or not you've completed reading the book. Though all this data is great, it's unwieldy, and hard to understand or navigate through. You give yourself another challenge: write some ruby methods to interpret the data! Here are the methods you have in mind...

## Deliverables

* `all_pages`: `all_pages` takes in your library as an argument, and outputs how many pages are in all of your books in your library! (Bonus: try to complete this method using the `.reduce` method)

Example
```ruby
all_pages(library)

12406
```
---
* `all_pages_read`: `all_pages_read` takes in your library as an argument, and outputs how many pages are in all the books that you've read! (Bonus: try to complete this method using the `.reduce` method)

Example
```ruby
all_pages_read(library)

781
```
---
* `all_genres`: `all_genres` takes in your library as an argument, and outputs an array. This array should contain all of the genres that you have in your library. Try to make it display only unique strings; no duplicates!

Example
```ruby
all_genres(library)

["Fantasy", "Horror", "Science Fiction"]
```
---
* `num_books_read`: `num_books_read` takes in your library as an argument, and outputs an array of all of the books that you have completed.

Example
```ruby
num_books_read(library)

[{title: "Dracula", author: "Bram Stoker", genres: ["Horror", "Gothic"], pages: 418, publication_year: 1897, completed: true}, {title: "Mastering the Art of French Cooking", author: "Simone Beck, Louisette Bertholie, Julia Child", genres: ["Cooking", "Non-Fiction"], pages: 726, publication_year: 1961, completed: true}]
```
---
* `completed_books_detail`: `completed_books_detail` takes in your library as an argument, and outputs a string that lists how many books you've read, and how many pages you've read.

Example
```ruby
completed_books_detail(library)

"I've read 5 books, totaling at 1074 pages."
```
---
* `books_in_library`: `books_in_library` takes in your library as an argument, and outputs an array of strings, where each string is each book of your library, but only their name and author

Example
```ruby
books_in_library(library)

["Inferno by Dante Alighieri", "Mastering the Art of French Cooking by Simone Beck, Louisette Bertholie, Julia Child", "Animal Farm by George Orwell"]
```
---
* `books_by_year`: `books_by_year` takes in your library as an argument, and outputs an array of strings (just like the previous method). However, the books should be ordered by what year they were published.

Example
```ruby
books_by_year(library)

["Inferno by Dante Alighieri", "Animal Farm by George Orwell", "Mastering the Art of French Cooking by Simone Beck, Louisette Bertholie, Julia Child"]
```
---
* `books_with_subtitles`: `books_with_subtitles` takes in your library as an argument, and outputs an array of book hashes that have titles that have a subtitle.

Example
```ruby
books_with_subtitles(library)

[{title: "Frankenstein; or, the Modern Prometheus", author: "Mary Shelley", genres: ["Gothic", "Horror", "Science Fiction"], pages: 280, publication_year: 1818, completed: true}]
```
---
* `books_primary_title`: `books_primary_title` takes in your library as an argument, and outputs an array of book title strings. If the book title has a subtitle, only output the primary title.

Example
```ruby
books_primary_title(library)

["Dracula", "Frankenstein", "Circe", "Animal Farm"]
```
---
* `highest_page_count`: `highest_page_count` takes in your library as an argument, and outputs the longest book. (Bonus: try to complete this method using the `.reduce` method)

Example
```ruby
highest_page_count(library)

{title: "War and Peace", author: "Leo Tolstoy", genres: ["Historical Fiction"], pages: 1225, publication_year: 1869, completed: false}
```
---
---
## BONUS Deliverables

* `recommended_books`: `recommended_books` takes in your library and a number in as arguments, and outputs an array of strings. The number of strings in the array should be equal to the number argument. The strings are about books you are recommending from your entire library, organized by fewest page count to longest page count. e.g., If the number argument is 4, you should output the 4 shortest books.

Example
```ruby
recommended_books(library, 3)

["You should read Animal Farm by George Orwell; it's only 112 pages long!", "You should read Circe by Madeline Miller; it's only 385 pages long!", "You should War and Peace by Leo Tolstoy; it's only 1225 pages long!"]
```
---
* `recommended_books_by_genre`: `recommended_books_by_genre` takes in your library and two strings in as arguments, and outputs an array of strings. The first string argument should be a genre that is preferred, and the second string argeument should be a genre that is not preferred. The array should a list of recommendations, listing the preferred genres first, followed by the the other books in your library. The books with the genres that are not preferred should not be in the array.

Example
```ruby
recommended_books_by_genre(library, "Historical Fiction", "Science Fiction")

["Since you like Historical Fiction, you should read Circe by Madeline Miller!", "Since you like Historical Fiction, you should read War and Peace by Leo Tolstoy!", "I also recommend Animal Farm by George Orwell.", "I also recommend Mastering the Art of French Cooking by Simone Beck, Louisette Bertholie, Julia Child.", "I also recommend Dracula by Bram Stoker."]
```
