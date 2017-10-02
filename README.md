# Ticketing System

## Purpose

The purpose of this assignment is to evaluate the candidate’s designing and development abilities.

## Deliverable

Code published on Github or Bitbucket.

Deadline is 7 days after assignment is sent to the candidate.

## Requirements

- Build a web based ticketing system.
- Administrator validate users.
- Users login to the system and go to their dashboard.
- The dashboard shows a list of tickets assigned to the user.
- Tickets can be created, edited and closed.
- They can also be assigned to another user.
- If the ticket is closed, it will no longer appear in the dashboard by default.
- If the ticket is assigned, it will show only to the assigned user by default.
- The dashboard will allow to show all tickets including closed ones.

## Models

- User

  - email
  - password
  - name

- Ticket

  - title
  - body
  - status (open, closed)
  - author (User)
  - assignee (User)
  - created (date)

## Pages

- Register

- Login

- Dashboard

  - filters: title, status
  - actions: create tickets, edit tickets, delete ticket

- Ticket: create

  - title, body, status and assignee are editable
  - status is open by default
  - dates read only and self by default
  - author is read only and self by default
  - assignee self by default but you can change it from a list of users

- Ticket: edit

  - title, body, status and assignee are editable

## Optional

- Use Sophilabs' guidelines to improve the code.
- Unit test coverage above 90%.
- Deploy your project on heroku or similar.

**Good luck!**
