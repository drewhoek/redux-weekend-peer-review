X = checks out = pass.
? = I didn't understand the question.
- = objective incomplete.

Multi-Part Form:

X Able to add feedback
X Data collected on individual pages & components
X Click on next takes you to the next page in sequence
X Data saves in DB after all the parts are completed (not piecemeal)
X Thank you page takes you back to the first view
X Old Data is cleared on form completion

Client code:

X Individual components for each form part
X Redux setup complete
X Store linked to react with <Provider>
X Store setup with reducer(s) and logger middleware
X Reducers & Actions Working
X Actions are in SCREAMING_SNAKE_CASE and semantically named
X Actions have a type key, and payload if sending data
X Reducers are returning a new state, or the old state (not mutating)
X Reducers are using spread correctly (to keep old data, while adding new)
? Review Component shows at all times with current redux state
X React-Redux Working
X connecting components correctly & dispatching Actions onClick
X mapStateToProps when data is needed from Redux for submission
X Axios POST request to add feedback

Server code:

X Router made for GET, POST

General Items

Feedback should be provided for these items, but they do not impact scoring.

Git
X Multiple git commits showing incremental progress
X Commits are descriptive of the changes made or feature added
X Has .gitignore with node_modules
- Readme file updated (assuming this is previously discussed)

Code Style
"Nice work overall Lance.  We were supposed to be able to skip commenting, but everything else seems to be in order."

- Appropriate amount of code comments.    "No comments that I could see."
x Code is consistently formatted.  "very clean!"

Client
X Appropriate use of HTML tags
X Basic CSS styling with margins/padding

Stretch Goals
First must be complete for score of 5 - Exceeds Expectations

Previous Steps

- allows a user to go to a previous step, either directly or by cycling backward thru the steps
- user can upate their score for a step
X new score is validated to not be empty
X redux is updated with new score
? user can continue on to review page and submit as in Base Mode

Admin View

- All entries are visible with correct data from inputs
- Most recent is at the top
- Can Delete an entry
- User is prompted before deleting
- Axios GET request to get all feedback for /admin view in componentDidMount

Busywork Goals, consider removing or making more useful

- Styling with Material UI

- Ability to flag a feedback item on /admin for further review

- Deployed to Heroku

