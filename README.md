# Training Exercises

The purpose of these exercises is to evaluate the candidate or apprentice's designing and development
abilities. We expect the code to be published publicly in a [Github](http://github.com/) or [Bitbucket](https://bitbucket.org/)
repository. You can use any technology with which you you feel proficient. We suggest using [Django](https://www.djangoproject.com/)
for the Backend, [React](https://reactjs.org/) for the frontend, and [PostgreSQL](http://postgresql.org/)
for the database.

## Excercise

We have the following exercises available:

- [Ticket System](./ticketing-system.md)
- [Car Rental System](./car-rental-system.md)
- [Stock System](./stock-system.md)

## Optional Requirements

If you feel inclined and you have extra time, consider also completing the following activities related
to code quality, testing and deployment.

### Code Quality

- Improve the code using Sophilabs' *[Guidelines](https://sophilabs.co/guidelines/)*.
- *[Unit Test](https://en.wikipedia.org/wiki/Unit_testing)* coverage above 90% both frontend and backend.

### Deployment

![Diagram of containers for the project](containers.png)

- Use [containerization](https://en.wikipedia.org/wiki/Operating-system-level_virtualization) through
  [Docker](https://www.docker.com/) to isolate your web server and database.  A good starting point
  could be having 3 containers:
  - A Frontend Server, which hosts a [Single Page Application](https://www.kirupa.com/react/creating_single_page_app_react_using_react_router.htm)
    and makes calls to a Backend Server to do any operation with the system.
  - A Backend Server, which exposes an API for operating with the system. It can contain the Admin
    Site to approve users.
  - A Database Server to store persistent data, using PostgreSQL or another database engine of your choice.
- *Deploy* your project to be available publicly on [Amazon Web Services](http://aws.amazon.com/),
  [Heroku](https://www.heroku.com/) or a similar service.

**Good luck!**
