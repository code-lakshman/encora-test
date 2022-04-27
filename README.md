# Encora Code Assignment
A custom module as assignment 

## Module structure/Installation
Dependencies
- Address
- Better Exposed Filters

Drupal 9 Compatible

All config files are in the `config/install` folder

# How this works on Pantheon site 

- Live Demo : https://dev-encora-test.pantheonsite.io/user

- Username: admin
- Password: admin

# Setup a Drupal system with custom content types based on Organization departments
## Sales CT
- Fields
https://dev-encora-test.pantheonsite.io/admin/structure/types/manage/sales/fields
- Example Node
https://dev-encora-test.pantheonsite.io/node/1

## Production CT
- Fields
https://dev-encora-test.pantheonsite.io/admin/structure/types/manage/production/fields
- Example Node
https://dev-encora-test.pantheonsite.io/node/2

## Delivery CT
- Fields
https://dev-encora-test.pantheonsite.io/admin/structure/types/manage/delivery/fields
- Example Node
https://dev-encora-test.pantheonsite.io/node/3

# Create views for all the above content types where records can be listed with option to sort by creation date, name, price etc. Add a range filter to drill down records created between certain dates and a category filter for the Production list view page.

## Sales data
- View Link
https://dev-encora-test.pantheonsite.io/admin/structure/views/view/sales_data/edit/sales_data
- Page
https://dev-encora-test.pantheonsite.io/sales-data

## Production Data
- View Link
https://dev-encora-test.pantheonsite.io/admin/structure/views/view/sales_data/edit/production_data
- Page
https://dev-encora-test.pantheonsite.io/production-data

## Delivery Data
- View Link
https://dev-encora-test.pantheonsite.io/admin/structure/views/view/sales_data/edit/delivery_data
- Page
https://dev-encora-test.pantheonsite.io/delivery-data

## Create roles and attach to content types such that, no one can edit/delete other departments' data, the view can be public.
New roles created
- Sales Team
- Production Team
- Delivery Team
- Sales Head

- Permissions page
https://dev-encora-test.pantheonsite.io/admin/people/permissions 

- Public views
- https://dev-encora-test.pantheonsite.io/node/1
- https://dev-encora-test.pantheonsite.io/node/2
- https://dev-encora-test.pantheonsite.io/node/3


## Add-on: create a workflow for sending emails to the sales head when a new quote is generated from sales team.
- Sales Head 
https://dev-encora-test.pantheonsite.io/user/2
- In `.module` file we have `hook_mail` implementation to send an email when sales team creates any sales node
- Screenshot here 
https://github.com/code-lakshman/encora-test/blob/main/Screenshot%202022-04-27%20at%2022.41.04.png 
- A message appears after you add a sales node


