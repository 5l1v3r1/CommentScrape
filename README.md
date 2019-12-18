# CommentScrape
Scraping comments out of web pages / apps for enumeration purposes. One can often find clues during enumeration in code comments.
## Usage
Simply run the Python application against the test file, like so:

```
root@demon:~/Code/CommentScrape# ./comment_scrape.py http://127.0.0.1/testcomments.html

Fetching: http://127.0.0.1/testcomments.html

Line 5: 		/* THIS IS A SINGLE LINE COMMENT */
Line 6: 		// This is a single-line comment
Line 8: 		/*
Line 9: 			This is a multi-line
Line 10: 			JS
Line 11: 			comment
Line 12: 			multi-
Line 13: 			line.
Line 14: 		*/
Line 17: 	<body><!-- This is an in-line body element comment -->
Line 18: 		<!-- This is an HTML comment  -->
Line 20: 		<!--
Line 21: 	  		This
Line 22: 			is a multi line
Line 23: 			HTML
Line 24: 			comment
Line 25: 		-->

root@demon:~/Code/CommentScrape# 
```
