# Training Exercises

The purpose of this exercise is to evaluate the candidate and apprentice designing and development abilities.
We expect the code published on public [Github](http://github.com/) or [Bitbucket](https://bitbucket.org/)
repository.
You can use any technology you feel proficient with. We propose using [Django](https://www.djangoproject.com/)
for the Backend, [React](https://reactjs.org/) for the frontend, and [PostgreSQL](http://postgresql.org/)
for the database.

## Excercise

The abailable excercises we have are the following:

- [Ticket System](./ticketing-system.md)
- [Car rental system](./car-rental-system.md)
- [Stock system](./stock-system.md)

## Optional Requirements

If you feel so and you have time consider doing the following activities related to code quality, testing and deployment.

### Code Quality

- Use Sophilabs' *[guidelines](https://sophilabs.co/guidelines/)* to improve the code.
- *[Unit Test](https://en.wikipedia.org/wiki/Unit_testing)* coverage above 90% both frontend and backend.

### Deployment

![Diagram of containers for the project](containers.png)

- Use [containerization](https://en.wikipedia.org/wiki/Operating-system-level_virtualization) through
  [Docker](https://www.docker.com/) to isolate your web server and database.  A good starting point
  can be having 3 containers:
  - A Frontend Server, which hosts a [Single Page Application](https://www.kirupa.com/react/creating_single_page_app_react_using_react_router.htm) and makes calls to a Backend Server to do any operation with the system.
  - A Backend Server, which exposes an API for operating with the system. It can contain the Admin Site to approve users.
  - A Database Server to store persistent data, using PostgreSQL or another database engine of your choice.
- *Deploy* your project to be available publicly on [Amazon Web Services](http://aws.amazon.com/), [Heroku](https://www.heroku.com/) or a similar service.

**Good luck!**
