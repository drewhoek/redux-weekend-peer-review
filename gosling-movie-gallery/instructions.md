
# Instructions for peer review

1. Add a file in this folder. Name it `parterName-yourName-projectName.md`. So if I am grading Mary's movie gallery weekend project, the filename could be `mary-blaine-redux-feedback-form.md`;
2. Make sure your filename ends in `.md` for markdown format
3. Paste in the ruberic, use the 'preview' functionality, save the file (on GitHub website is fine, or clone it down and push).

# Weekend 12 Challenge - Redux Saga Movies

## Overview

### Part 1

A weekend challenge in which students display a list of provide movie data, make requests via Sagas, and utilize a junction table and join select for a detail view. Allows editing of title and description for a single movie.

- Student is provided with a Movie List Page and Route. It displays all movies on the DOM.
- Student is provided with full data tables and starter data

### Part 2

SQL Challenges. See [other rubric](./weekend12-sql-challenge.md)


## Links

> Sagas, SQL junction table and joins

- Starting repo: [repo](https://github.com/PrimeAcademy/weekend-movie-sagas)
- Live Solve Starter: [repo] TODO
- Solution: TODO
    

## Movies Page

- Student is provided with a Movie List Page and Route. It displays all movies on the DOM.
- [ ] View has ability to click on a single movie
- [ ] Clicking on single movie goes to movie details view at `/details`

## Details Page

- [ ] Detail view should show all detail data include all the genres for the given movie
- [ ] Has Back to List which goes back to the Home Page

## Add Movie Page

- at own route similar to `/add`
- an input field (for the movie title)
- an input field (for the movie poster image URL)
- a textarea (for the movie description)
- a dropdown (for the genres)
- Cancel button, which should bring the user to the Home/List Page
- Save button, which should update the title and description in the database and bring the user to the Home/List Page (which now has the new movie)

### Add Movie POST/INSERT

Requires two inserts: first for the movie data and second into the movies_genres junction table. Much of this was provided in the starting repo. Students will need to match whatever they used for junction column names in that INSERT query.

**Base functionality does not require being able to select more than one genre for a new movie**



## General Tasks

- [ ] Use Sagas for API requests to the server
- [ ] Use cards or grid for nice movie listing presentation
- [ ] Should have at least 15+ commits. 
- [ ] Use branches for features.
- [ ] Comment your code.
- [ ] Update this README to include a description of the project in your own words.

## Stretch Goals

> NOTE: Copy/pasted from instructions


### Edit Page

- [ ] View at route `/edit`
- [ ] Assumes the selected movie id is in Redux
- [ ] Display an input field for changing the movie title
- [ ] Displays a textarea for changing the movie description
- [ ] Cancel button, which should bring the user to the Details Page
- [ ] Save button, which should update the title and description in the database and bring the user to the Details Page

### OTHER STRETCH GOALS
- [ ] Display the current values in the input (title) and textarea (description) on the Edit Page
- [ ] Display all genres on movie list page. Research array_agg to make this possible.
- [ ] Move sagas and reducers out of your index.js and into separate files (ideally in src/redux/reducers and src/redux/sagas folders).
- [ ] Allow the user to refresh the details or edit page. The url for the details page would be something like /details/1 for movie with id of 1. Research react router params.
- [ ] Allow the user to add a genre to a movie.
- [ ] Allow the user to remove a genre from a movie.
- [ ] Only display the top 10 movies, and allow the user to search for movie titles with a search bar on the home page (you can do this on the client side or the server side, server side is a bigger stretch, but good practice).
- [ ] Create an Admin page. Add a link from the Home page to the Admin page. The page should initially display a login form (an input for username and an input for password). When the user enters the correct username (camera) and password (action), the page should display a form to add genres to the database, and a list of all of the genres with an x to remove them from the database. 

## Junction Table

Junction Table and full starter data is provided.


## Genre Join for a specific movie

```sql
-- expected join without array_agg()
-- we only need the genre names for Base Mode, so skip the movie stuff
SELECT genres.name FROM movies
JOIN <junction_table_name> ON movies.id = <junction_table_name>.movies_id
JOIN genres ON genres.id = <junction_table_name>.genres_id
WHERE movies.id = 1; -- Avatar's id
```


## Portal-ready Markdown

```

---
| Functional Requirements | Complete? |
| --- | :---: |
| Movies can be clicked on to go to a detail page | no |
| Movie Detail Page displays movie image, title, description | no |
| Movie Detail Page displays all genres for this movie | no |
| Add Movie Page allows the movie title, image URL, description to be added | no |
| Add Movie Page allows user to select 1 genre | no |
| Add Movie POST/INSERT stores movie data | no |
| Add Movie POST/INSERT stores genre junction data | no |
| Sagas used for calls to server | no |

---
### Notes:

Notes on items above.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no |
| Code broken down into Components | no |
| Commits are descriptive of the changes made or feature added | no |
| Readme file updated | no |
| Appropriate amount of code comments | no |
| Code is consistently formatted | no |
| Good use of Redux (where appropriate) | na/yes/no |
---

### Notes:



```
