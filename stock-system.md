# Stock System

## Project information

This project consists in building a web stock system, where users can upload new products and
administrates it stock. The system manages two types of entities: Users, Product. For the users,
the system knows about, their email, their password, which should be stored securely in the database
and their full name.
For the products, the systems stores their name, category (a predefined list), prices, creation date
and stock.

### Registration and approval

Users have to request to register to the site. Upon request, a system administrator has to approve
their request for them to use the site.

### Dashboard and product management

When the user logs in they are redirected to their Dashboard, which shows a list of products.
The products with stock lower than a configurable value should be marked.
In the dashboard the user can also add a new product.

## Pages

We propose a site structure the picture below, having a separate site for using the rent system, and
another special page for administrators for the purpose of approving users.

![Stock system sitemap](stock-system-sitemap.png)

You can adapt the schema, as long as the site provides following pages:

- Register Page, where users can register. They have to wait until an administrator authorizes them
  to enter again.
- Login page to enter the Dashboard
- Dashboard page containing a product list and
  - Filters: by category
  - Sort: by name, stock
  - Individual actions: create a new product, edit a product
- Create a product, where the user can enter the following information
  - Category, name, and stock are editable
  - The systems should suggest the categories from a combobox for example.
  - Creation date is read only and set to the browser date.
  - Rent's User is read only and is set to the logged in user.
  - Stock can't be lower than 0
- Edit/Detail product:
  - Name is not editable

### Hints

- If you use Django, you can use the built in [Admin site](https://docs.djangoproject.com/en/2.0/ref/contrib/admin/)
  page for implementing this in another framework consider using an Admin Site for this instead of crafting
  a page specifically for this.

- The landing page can have a log in form included instead of a dedicated login page.
