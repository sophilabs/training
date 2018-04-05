# Car Rental System

## Project Information

This project consists of building a car rental web system where users can upload new clients and
rent their cars. The system manages three types of entities: Users, Clients, and Cars. The system knows
the following information about the users: their email, their password (which should be stored securely
in the database), and their full name.
For the clients, the system stores: their name, their drivers license number, and a phone number.
For the cars, the system stores: the model, the year, the number of km, and its status (which
can be either *rented* or *available*). When a car is rented, it is important to store which client
has rented the car, which user made the rental, the date of the rental and the return date.

### Registration and Approval

Users have to submit a request to register with the site. A system administrator then has to approve
their registration request for them to use the site.

### Dashboard and Rental anagement

When the user logs in they are redirected to their Dashboard, which shows a list of rentals made by that
user. The rentals that are overdue, with a return date prior to the current date, should be marked. In
the dashboard, the user can also add a new client, rent a car to a client (the car shouldn't be rented),
and return a rental. When a rental is returned it must disappear off the list. The dashboard should
allow displaying all tickets, including closed ones.

## Pages

We propose a site structure like the picture below, creating a separate site for using the rental system,
and another special page for administrators for the purpose of approving users.

![Rent car system sitemap](rent-car-system-sitemap.png)

You can adapt the schema, as long as the site provides the following pages:

- Registration Page where users can register. (They will have to wait until an administrator authorizes
 their account to enter again.)
- Login page to enter the Dashboard
- Dashboard page containing a rental list plus the following features:
  - Filters: by car and client
  - Sort: by return date
  - Individual actions: Make a new rental, return a rental
- Make a rental page with following characteristics and features:
  - User can edit the car, client, and return dates (editable)
  - The system should suggest only *available* cars
  - Creation date is read only and set to the browser date.
  - Rental's User is read only and is set to the logged in user.
- Create client page, where the user can create new clients
- Client details page, where the user can see/edit the client information. It will be very useful if
 you can show a list of cars rented by these clients.

### Hints

- If you use Django, you can use the built in [Admin Site](https://docs.djangoproject.com/en/2.0/ref/contrib/admin/)
  page. For implementing this in another framework, consider using an Admin Site instead of crafting
  a page specifically for this.

- You can include a log in form on the landing page rather than creating a dedicated login page.
