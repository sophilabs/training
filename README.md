# Ticketing System

![A ticket system icon](icon.png)

## Purpose

The purpose of this assignment is to evaluate the candidate/apprentice designing and development abilities.

## Deliverable

Code published on public [Github](http://github.com/) or [Bitbucket](https://bitbucket.org/) repository. Deadline is 7 days after assignment is sent to the candidate.

## Technologies

You can use any technology you feel proficient with. We propose using [Django](https://www.djangoproject.com/) for the Backend, [React](https://reactjs.org/) for the frontend, and [PostgreSQL](http://postgresql.org/) for the database.

## Project information

This project consist in building a web based ticketing system, where users can upload tickets and distribute work among project teammates.

The system manages two types of entities: Users and Tickets.

For the users the system knows about, their email, their password, which should be stored securely in the database and their full name.

For the tickets the system stores their title, the description , it's status (which can be either *open* or *closed*), the creation date. Also for each ticket the system stores the Author and the Assignee both of them are User entities.

## Specific requirements

### Registration and approval
Users have to request to register to the site. Upon request, a system administrator have to approve their request for them to be able to use the site.

### Dashboard and ticket management

When the user log in they are redirected to their Dashboard, which shows a list of tickets assigned to that user. Tickets can be created, edited, closed or assigned to another user. If the ticket is closed, it will no longer appear in the dashboard by default. If the ticket is assigned, it will show only to the assigned user. The dashboard will allow to show all tickets including closed ones.

## Pages

We propose a site structure the picture below, having a separate site for using the Ticket system, and another special page for admistrators for the purpose of approving users.

![Ticket system sitemap](sitemap.png)

You can adapt the schema, as long as the site provides following pages:

- Register Page, where users can register. They have to wait until an admisitrator authorizes them to enter again.
- Login page to enter the Dashboard
- Dashboard page containing a ticket list and
  - Filters: by title and status
  - Individual actions: Create a ticket, edit a ticket, and delete a ticket
- Ticket creation page, where the user can enter the following information
  - Title, body, status and assignee are editable.
  - Status is open by default.
  - Creation date is read only and set to the browser date.
  - Author is read only and is set to the logged in user.
  - Assignee is the logged in user by default but you can change it selecting from a list of users.
- Ticket details page, where the user can see and edit the ticket status, body and title.

### Hints

* If you use Django, you can use the built in [Admin site](https://docs.djangoproject.com/en/2.0/ref/contrib/admin/) page for implementing this in another framewoerk consider using an Admin Site for this instead of crafting a page specifically for this.
* The landing page can have the login page included.

## Optional Requirements

- Use Sophilabs' *[guidelines](https://sophilabs.co/guidelines/)* to improve the code.
- *[Unit Test](https://en.wikipedia.org/wiki/Unit_testing)* coverage above 90% both frontend and backend.
- Use [containerization](https://en.wikipedia.org/wiki/Operating-system-level_virtualization) through [Docker](https://www.docker.com/) to isolate your web server and database.
- *Deploy* your project on [Amazon Web Services](http://aws.amazon.com/), [Heroku](https://www.heroku.com/) or a similar service.


**Good luck!**
