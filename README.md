# Genre Identification

Instructions on running this project
------

### If you do not have Ruby set up on your computer, please set up now
Instructions can be found (here)[https://www.ruby-lang.org/en/documentation/installation/]

### Either clone this repository using the HTTP or SSH protocol or download a a zip file

HTTPS: ```git clone https://github.com/genagain/genre_identification.git```

SSH: ```git clone git@github.com:genagain/genre_identification.git```

To download a zip file please click the "Download Zip" button on the right hand side of the screen.

### Run the following command at the root of this project in your terminal
```ruby run_this.rb```

Edge cases
------
I encountered an interesting edge case when a keyword has more than one genre associated with it. I encountered this edge case when I was finishing with writing the program. Because of this when generating the keywords data structure in the ```generate_keywords``` method in the lib/genre_identifier.rb, I thought it would be okay to have the keys be the keywords. 

Because "distant future" appears twice in samples/sample_genre_keyword_value.csv, I should have counted it twice when generating the keywords data structure. Because I did not, this made the resulting values for genre-fit incorrect. However when a keyword only has one genre associated with it, the genre-fit scores are correct.

### This took me about 4.5 hours
If I had more time, I would have accounted for this edge case. I also would have programmed the logic to print genres with a genre-fit scores of 0 when a book is catagorized in one or two genres. Finally, I would have added logic to sort the genres by genre-fit score before being printed out. 
