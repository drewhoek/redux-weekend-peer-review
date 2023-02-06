-David-

---
| Functional Requirements | Complete? |
| --- | :---: |
| Movies can be clicked on to go to a detail page | Yes |
| Movie Detail Page displays movie image, title, description | no | -object returns undefined so nothing is displayed
| Movie Detail Page displays all genres for this movie | no | -object returns undefined so nothing is displayed
| Add Movie Page allows the movie title, image URL, description to be added | no | -page displays an error message it is trying to grab the genre but it is undefined crashing the rest of the page
| Add Movie Page allows user to select 1 genre | no | -genres are displayed but where they are referenced as part of the object are un defined "gen"
| Add Movie POST/INSERT stores movie data | no | -the code does not get this far as per the previous state not going through
| Add Movie POST/INSERT stores genre junction data | no | -the code does not get this far as per the previous state not going through
| Sagas used for calls to server | yes | -The get saga for the movies list is working

---
### Notes:

Notes on items above.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no | -3 commits, a good idea to get more commits, generally each time you finish a functional part, or something similar
| Code broken down into Components | yes |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | no | -remember to do the readme
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Good use of Redux (where appropriate) | na/yes/no | -redux used but not fully working yet
---

### Notes:

So there are a few things that you will need to work on, the details page and the add movie page are currently not working fully. Overall you have most of the large pieces that you need but you still
need to get them all connected together. Youre on the right track.
