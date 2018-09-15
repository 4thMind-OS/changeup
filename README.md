# changeup
...

### Things for Alex to take on
- [ ] look into https://auth0.com/docs/quickstart/spa

### Things to consider 
- code breakout....we want a monorepo-ish code architecture
    - lerna
    - mgit
    - ...
    - _see 
- we need Auth to include the following Roles
    - User (general)
    - Account Manager
    - Admin
    - SysAdmin
- We'll want at least 2 apps
    - A mobile app for 
        - Users to look at and take action on their day's ChangeUp challenges/tasks.  (They may also be able to see a week view eventually, but the single day view comes first.)
        - Users and Account Owners to capture quick summary of challenges/tasks for the future ("inbox" style).
    - A web app for 
        - Account owners (people who manage tasks for one or more Users) to enter and organize/manage a Users challenges/tasks over time.
        - More detailed table and chart views
## Branching
 - All work must be done in branches and must be submitted with a PR
 - Branch naming convention: {your_name}/{ticket_number}-descriptive_name
