
Hey AJ,

General Feedback.

Really great job on this.  Code was clean and all the compenents were really well organized.  I had a few errors come up and I think all you needed was setting the default in the useState. This would have allowed your alerts for empty fields to come up and solve the undefined thing.  Styling was all consistent and easy to read / navigate.

I had some nesting parent/child nesting errors that would show on the review page, but it didn't impact anything as far as the form or moving to next page.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | yes |
| Data stored in Redux when navigating from page to page | yes |
| User is notified when trying to leave a blank score | no |
| Review Component displays scores and comments from current redux state | yes |
| Submit button sends data to the server via Axios | yes |
| Confirmaion Page displays after data is POSTed to the server | yes |
| Button on Confirmation Page clears Redux and starts a new survey | yes / no | reset dispatch was on review page
| Views are broken down into components | yes |

---
### Notes:

Notes on the above Functional Requirements.

I noticed you had the 'required' set on the drop-down, so I think that would have worked, if the undefined useState didn't throw the error.

Then I just noticed that your dispatch to reset was on your button on the review page, and it could be on the button on the submit page.  Great job.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes |
| Commits are descriptive of the changes made or feature added | yes |
| Readme file updated | no |
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:

Notes on General Items

Really great job on commenting and descriptions within your Git commits.  Again code was really clean and easy to follow.  The only thing I noticed the README wasn't updated.  Easy fix and I know you were in a time crunch.

Only other nit picky thing (just a for me thing) was maybe including a res.sendStatus on the axios POST so you can tell it was accepted on submission.  No big deal, I could tell it submitted in the table.  Just an extra.

```


