```

---
| Functional Requirements | Complete? |
| --- | :---: |
| Movies can be clicked on to go to a detail page | yes |
| Movie Detail Page displays movie image, title, description | yes |
| Movie Detail Page displays all genres for this movie | yes |
| Add Movie Page allows the movie title, image URL, description to be added | yes |
| Add Movie Page allows user to select 1 genre | yes |
| Add Movie POST/INSERT stores movie data | yes |
| Add Movie POST/INSERT stores genre junction data | yes |
| Sagas used for calls to server | yes |

---
### Notes:

Notes on items above.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes |
| Code broken down into Components | yes |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | yes |
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Good use of Redux (where appropriate) | yes |
---

### Notes:

- I noticed when clicking a movie card that the cursor does not change. Changing the css for that to cursor: pointer; can help indicate that that is an item that can be clicked on.

- I love how you implemented adding multiple genres to a movie on the add movie page and the use of check boxes.

- The check boxes on the edit page already checked for the genres of the movie on load is super neat!

- I like how you incorporated different renders on the details page so when the edit button is clicked you have it conditionally render the EditDetails component, again super neat!

- I am assuming some of those whack long class names are for tailwind? Pretty cool!

```
