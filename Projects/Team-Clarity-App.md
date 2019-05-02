# Team Clarity

**Tier:** 3-Advanced

An important aspect of Agile teams is everyone on the team is encouraged to
have and express opinions when it comes to decisions. While this is valuable
for both team morale and the quality of the resulting decision it's not always
easy to identify team differences and concensus. It's also all too easy for
discussions to end in decision making by "groupthink".

The objective of the Team Clarity app is to quantify team member opinions on
a particular subject and to vote on a particular solution or determine that
a hybrid solution necessary.

It does this by allowing team members to 

1. Propose solutions along with pros and cons for each
2. Rate pros and cons for each proposal
3. Rank the three solutions they like the best in numerical order

Once voting is complete metrics are provide to highlight a clear winner among
the proposed solutions or to focus additional team discussion around the
leaders.

### Constraints

Users have different responsibilities which means the app must provide 
functionality only to the users of a given role. This means the app must
identify users in order to determine what functionality can be delivered to
each. These roles are `team lead` and `team member`. 

This project must support not just a single user, but all members of the team,
some of who might be remote developers. Users should also have the opportunity 
to prepare prior to any discussion. This means this app must collect and
deliver information to the user through a frontend application, but since data
is shared by the team it must reside in a server and must be concurrently
accessible.

Because of this complexity the initial set of User Stories is based on a series
of _mocked_ functionality which can be added later by implementation of 
Bonus features that replace the mocks with actual functionality. In addition,
only one decision can be worked on at any point in time.

## User Stories

### Page Layout
-   [ ] User can see a navigation bar at the top of the page containing
    - User name and role name. These will be blank if user has not yet
logged in.
    - Application name
    - A "hamburger" menu with these options:
       - Define Issue (available only to users with the `team lead` role)
       - Evaluate Issue (available to all `team members`)
       - Results (available to all users)
-   [ ] User can see a content area that will contain information for the 
option selected in the hamburger menu.
-   [ ] User can see a Footer Bar at the bottom of each page containing an
About link

### User Authentication
-   [ ] User can see a mock authentication panel containing a user name 
input field, a password input field, and a 'Login' button.
-   [ ] Developer will define valid user names and passwords and their roles
in the app for its inital release.
-   [ ] User can enter a valid combination of user name and password into the
input fields.
-   [ ] User can click the Login button.
-   [ ] User can see an error message if either the user name or password fields
are empty or if the combination of the two is invalid.
-   [ ] User can see the users role name (`team lead` or `team member`)
displayed in the 

### Define Issue Page
-   [ ] Users with the `team lead` role can see the Define Issue page
containing the issue description input text field and 'Cancel' and 'Add' 
buttons.
-   [ ] User can enter a short description of the issue a solution is to be 
decided on.
-   [ ] User can click the 'Add' button to add the issue.
-   [ ] User can see and error message if the description text box is empty.
-   [ ] User will see a confirmation message following an 'Add' operation.

### Evaluate Issue Page
*_TBD_* Process based on team members defining solutions, assigning pros and cons and ranking them
by importance, then ranking solutions.

### Results Page
*_TBD_* Process based on displaying results of member ranking and voting in descending order.

### About Page
-   [ ] User can click the About link in the Footer Bar to display information
about the Developer.
-   [ ] User can see links to the Developers GitHub and social media accounts 
including social media icons (like the Twitter icon).

## Bonus features

### User Authentication
-   [ ] Developer will implement a true authentication protocol that allows
the user to be validated using an app login screen.

### Issues List Page
-   [ ] User can see an Issues List option that replaces the Define Issue
option in the hamburger menu. 
-   [ ] User can see a list of open and closed issues on the Issues List page
as well as a 'New Issue' button.
-   [ ] User can see a row for each issue containing an 'Open' button, it's
status ('Open' or 'Closed'), the date it was created, and the first 50
characters of its description.
-   [ ] User can click the 'New Issue' button to display an empty Define Issue page.
-   [ ] User can click the 'Open Issue' button to display the Define Issue page
prefilled with that issues data.
-   [ ] User can see new buttons to 'Delete' and 'Modify' on the Define Issue 
page opened from the Issues List page.
-   [ ] User can click the 'Delete' button to delete an issue in the open
status.
-   [ ] User can modify the issue description and click the 'Modify' button
to update it.
-   [ ] User can see a confirmation message for 'Delete' and 'Modify'
operations.

## Useful links and resources

- [GroupThink](https://www.psychologytoday.com/us/basics/groupthink)
- [Quantitative Pros and Cons](https://www.mindtools.com/pages/article/newTED_05.htm)

## Example projects

[TriCider](https://www.tricider.com/)
