Code author: Mustafa Mustafa
Code reviewer: Drew Hoek

Hey Mustafa,

Good work here! The post is not working because you are attempting to send an array of individual objects for each piece of feedback. You need to be sending an object at the very end not an array. Everything else works intended though and your values are displayed correctly. Just one little change to make with your reducers and payloads.

---

| Functional Requirements                                                | Complete? |
| ---------------------------------------------------------------------- | :-------: |
| Multi page form with client side routing and navigation (next button)  |    yes    |
| Data stored in Redux when navigating from page to page                 |    yes    |
| User is notified when trying to leave a blank score                    |    yes    |
| Review Component displays scores and comments from current redux state |    yes    |
| Submit button sends data to the server via Axios                       |    no     |
| Confirmation Page displays after data is POSTed to the server          |    no     |
| Button on Confirmation Page clears Redux and starts a new survey       |    no     |
| Views are broken down into components                                  |    yes    |

---

### Notes:

Everything works great besides the post request. Tweak the reducer as well as add a confirmation page and then it'll work great!

---

| General Items                                                | Complete? |
| ------------------------------------------------------------ | :-------: |
| More than 15 git commits                                     |    no     |
| Commits are descriptive of the changes made or feature added |    yes    |
| Readme file updated                                          |    no     |
| Appropriate amount of code comments                          |    no     |
| Code is consistently formatted                               |    yes    |
| Server code organized with router & module files             |    yes    |

---

### Notes:

Code is formatted well and is easy to follow but make sure you update your README and add a few more comments in the code!
