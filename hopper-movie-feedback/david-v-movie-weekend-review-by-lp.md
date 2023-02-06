| Functional Requirements | Complete! |
| --- | :---: |
| Movies can be clicked on to go to a detail page | Yes |
| Movie Detail Page displays movie image, title, description | Yes |
| Movie Detail Page displays all genres for this movie | Yes |
| Add Movie Page allows the movie title, image URL, description to be added | Yes |
| Add Movie Page allows user to select 1 genre | Yes |
| Add Movie POST/INSERT stores movie data | Yes |
| Add Movie POST/INSERT stores genre junction data | Yes |
| Sagas used for calls to server | Yes |

---
### Notes:

Base functionality looks great! 

---
| General Items | Complete! |
| --- | :---: |
| More than 15 git commits | Yes |
| Code broken down into Components | Yes |
| Commits are descriptive of the changes made or feature added | Yes |
| Readme file updated | Yes |
| Appropriate amount of code comments | Yes |
| Code is consistently formatted | Yes |
| Good use of Redux (where appropriate) | Yes |
---

### Notes:

Project looks great overall!  I like the use of a different font, which can be easy to forget, but adds a lot!
Also, I love the scroll buttons to move between detail pages! I'd be careful using a <p> as a button though.  It will cause issues with accessability readers.

Couple of things to think about:
You may want to set min/max or just a set width on your cards on the movie list.  Without this you end up with situations where some cards are very wide and some are small based on their title.  For example, one of the titles is "Harry Potter and the Philosopher's Stone" this title made whatever column it was in very wide even when one below it was "Gone Girl".

On the movieList page, i'd recommend thinking about putting the onClick to the container <div> not the image.  At first I couldn't get into the details page because I was clicking on the card all over and nothing was happening, even though the curser was set to a pointer.

When in your details page and editing a movie, if you remove all genres you get an error and can no longer see the movie at all.  You probably want to make it so the user can't delete the last genre or (better option) still display the movie even with no genres

One last minor suggestion, when doing your final push, i'd suggest cleaning up some of your console.logs and comments.  Remove some of the "testing" comments from when you were working on things and/or comment out the console.log's so when loading it doesn't show a ton of "random" info to the user.
