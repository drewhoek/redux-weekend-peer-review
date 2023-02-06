# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [X] Able to add feedback
    - [X] Data collected on individual pages & components
    - [X] Click on next takes you to the next page in sequence
    - [X] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [X] Thank you page takes you back to the first view
    - [X] Old Data is cleared on form completion

- Client code:
  - [X]  Individual components for each form part
  - [X]  Redux setup complete
    - [X] Store linked to react with `<Provider>`
    - [X] Store setup with reducer(s) and logger middleware 
  - [ ] Reducers & Actions Working
    - [X] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [X] Actions have a `type` key, and `payload` if sending data
    - [X] Reducers are returning a new state, or the old state (not mutating)
    - [X] Reducers are using spread correctly (to keep old data, while adding new)
  - [X] Review Component shows at all times with current redux state
  - [X] React-Redux Working
    - [X] `connect`ing components correctly & dispatching Actions onClick
    - [X] `mapStateToProps` when data is needed from Redux for submission
  - [X] Axios POST request to add feedback


- Server code:   
  - [X] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [X] Multiple git commits showing incremental progress
  - [X] Commits are descriptive of the changes made or feature added 
  - [X] Has .gitignore with node_modules
  - [X] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [X] Appropriate amount of code comments
  - [X] Code is consistently formatted
- Client
  - [X] Appropriate use of HTML tags
  - [X] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of _5 - Exceeds Expectations_

- Previous Steps
  - [X] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [X] user can upate their score for a step
    - [X] new score is validated to not be empty
    - [X] redux is updated with new score
  - [X] user can continue on to review page and submit as in Base Mode


- Admin View
  - [X] All entries are visible with correct data from inputs
    - [X] Most recent is at the top
  - [X] Can Delete an entry
    - [X] User is prompted before deleting
  - [X] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ ] Styling with Material UI
- [X] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey David,

General Feedback.

---
| Functional Requirements | Complete |
| Multi page form with client side routing and navigation (next button) | Yes |
| Data stored in Redux when navigating from page to page | Yes |
| User is notified when trying to leave a blank score | Yes |
| Review Component displays scores and comments from current redux state | Yes |
| Submit button sends data to the server via Axios | Yes |
| Confirmation Page displays after data is POSTed to the server | Yes |
| Button on Confirmation Page clears Redux and starts a new survey | Yes |
| Views are broken down into components | Yes |

---
### Notes:

Project looks awesome!  Love the custom background, and the pages are consistent and nicely laid out.  Great use of the sweet alerts for your confirmations!

One thing to keep in mind is what data you are working with, you use a Number() conversion multiple times on the same data between the client and database. While this project doesn't strictly need number vs string, its good to be aware of what your data is at all times!

---
| General Items | Complete |
| More than 15 git commits | Yes |
| Commits are descriptive of the changes made or feature added | Yes |
| Readme file updated | Yes |
| Appropriate amount of code comments | Yes |
| Code is consistently formatted | Yes |
| Server code organized with router & module files | Yes |

---
### Notes

Great work overall!  You have a great amount of commits and everything looks well documented and clean.  It may be worth looking at a formatter that helps with tab whitespace, as the big nested SWAL stuff gets pretty bulky with 4 spaces on each indent.

The notes are just minor things to keep in the back of your head:

1. May want to be a little more detailed about commit messages.  If you ever need to go back to a commit, but it just says "added image" you don't know which image commit you are going back to if there are multiple images.

2. Run the readme through a spellcheck.  Some people never notice typos, but some are very attuned to them, and small/repeated spelling things can affect overall view of a project.

3. <th> tags should only be used in a <thead> tag for accessability issues with browsers.  In your admin page you don't have a <thead> at all, but then have <th> used in your <tr>'s.

```
