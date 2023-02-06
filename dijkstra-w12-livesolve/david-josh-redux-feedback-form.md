## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [x] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [x] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [x] Thank you page takes you back to the first view
    - [x] Old Data is cleared on form completion

- Client code:
  - [x]  Individual components for each form part
  - [x]  Redux setup complete
    - [x] Store linked to react with `<Provider>`
    - [x] Store setup with reducer(s) and logger middleware 
  - [x] Reducers & Actions Working
    - [x] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [x] Actions have a `type` key, and `payload` if sending data
    - [x] Reducers are returning a new state, or the old state (not mutating)
    - [ ] Reducers are using spread correctly (to keep old data, while adding new)
  - [x] Review Component shows at all times with current redux state
  - [x] React-Redux Working
    - [x] `connect`ing components correctly & dispatching Actions onClick
    - [x] `mapStateToProps` when data is needed from Redux for submission
  - [x] Axios POST request to add feedback


- Server code:   
  - [x] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [x] Multiple git commits showing incremental progress
  - [x] Commits are descriptive of the changes made or feature added 
  - [x] Has .gitignore with node_modules
  - [ ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [x] Appropriate amount of code comments
  - [x] Code is consistently formatted
- Client
  - [x] Appropriate use of HTML tags
  - [ ] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of _5 - Exceeds Expectations_

- Previous Steps
  - [x] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [x] user can upate their score for a step
    - [x] new score is validated to not be empty
    - [x] redux is updated with new score
  - [x] user can continue on to review page and submit as in Base Mode


- Admin View
  - [x] All entries are visible with correct data from inputs
    - [x] Most recent is at the top
  - [x] Can Delete an entry
    - [ ] User is prompted before deleting
  - [x] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [x] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku

## Comments
I do like how clicking on the name of a field in Review will redirect you to the page to edit. I would recommend using CSS to change the cursor to a pointer to make it obvious to users that it is a clickable field, otherwise misclicks could happen more easily.
A nice trick to only allow the numbers 1 - 5 would be to add min=1 max=5 to your input, then you will not need to use an if statement to check if the field's value is a different number.
When 'delete' is clicked in the admin page you are using an alert. A confirm should be used here instead, as an alert has only one option to choose from and thus even if you misclicked the only option on the pop-up will lead to deletion. A confirm has two options, thus can work as the condition of an if statement.

Good job with getting the stretch goals done. I see the function and router made for the PUT request, so it looks like if you had more time you could have gotten all the stretch goals completed.
I like how you used props in a way to allow you to reuse the Form.jsx for all the pages, though it did prevent the ability to leave comments empty.

Overall, I think you did a great job. Definitely gives me some ideas on how to improve my own code.
