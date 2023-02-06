Hey _Hassin__,

General Feedback.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | yes |
| Review Component displays scores and comments from current redux state | no |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | no |
| Button on Confirmation Page clears Redux and starts a new survey | no |
| Views are broken down into components | yes |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | no |
| Commits are descriptive of the changes made or feature added | no |
| Readme file updated | no |
| Appropriate amount of code comments | no |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Just a few things to note.  It looks like you have the input validation set up correctly.  However, you are using the history.push even if they have not 
filled out anything for the inputs, so it goes to the next page no matter what.  Also, in the Feedback.jsx file, you are bringing in the store but the names
of your reducers do not match up with the names you are referring to in the file. This results in no data being displayed, and the data being sent to the backend does not exist,
so the application throws a server error when the user trys to submit.
