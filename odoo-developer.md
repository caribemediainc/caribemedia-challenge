# Odoo Developer Challenge

The assignment is designed to check your coding and problem-solving.

Things we require your work to have:

- Code organization (modularity, dependencies between modules, etc)
- Clean and readable code
- No unused code or unused file in the custom modules

## Introduction

Caribe Media needs a software that allows the management of the internal tasks as well as the sales management. For this purpose, the company has chosen to use an Open Source solution: **Odoo**.

### Odoo

Odoo is a suite of open source business apps that cover all your company needs: CRM, eCommerce, accounting, inventory, point of sale, project management, etc. Odoo's unique value proposition is to be at the same time very easy to use and fully integrated.

## Requirements

Your job as an Odoo Developer is to create and maintain odoo modules that helps Caribe Media reach its goals. You should be able to listen to problems and figure out how to solve them in a efficient way.

### Tasks

You should get your Odoo V15.0 instance up and running by yourself in any way of your preference.

> we recommend using [VSCode](https://code.visualstudio.com/) as a lightweight code editor, [Dockerdoo](https://github.com/iterativo-git/dockerdoo) as a nice and easy way to get odoo running in docker and [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension to build and run dockerdoo faster.

1. Create a DB with Country: Dominican Republic and Language: English
2. Create a submodule for Sales App (sale_management):

   - Add a "sale_type" relational field (with its maintenance so the users can handle it by their own).
   - In a sale, if the selected value for this sale_type field is "Recorded", the "Call ID" field must show up as required to save the sale (new field). If the selected values is "Signed", the Call ID field must not be visible or required.
   - The logic for the Call ID field to be visible or not must be controlled from the Sale Type maintenance. This means that the users must be able to choose if they want the Call ID field to show up whenever a sale is marked as "Recorded" or any other Sale Type they create.

3. Create a submodule for Contacts App (contacts):

   - Add any needed field to manage multiple phone numbers (dinamically) by client.
   - These fields must be stored on DB and be visible only if the client is a Company.
   - Aside of the phone number, you must store the raw phone (without parenthesis, hyphen, etc), a field to check if it is active and a field to check if it is the main phone (only one main phone by client).
   - Access Rights:
     - Everyone can read/see all of the phones inside the contact.
     - Only the Admin (administration/settings) will be able to see and fully manage all of the additional phones.
     - A new group named "Phone Management" will be able to read, add and modify the additional phones, but won't be able to delete them.

4. Create a submodule for Stock App (stock):

   - Create a new search filter on the search bar that allows the users to search by sale price. Ex: all of the products with a sale price of 10.

5. Create a submodule for the next two actions:
   - Create a server action for Contacts app that adds the "Prospects" tag to the selected contact.
     - The action must be available when the contact is selected.
   - Create a schedule action for Contacts app that updates the "Notes" field of every contact with the text "Updated on {Day/Month/Year Hour:Minutes:Seconds}".
     - The schedule action must execute by itself a couple of times until every contact have been updated.
     - The schedule action must execute every 1 minute.
     - The schedule action must never repeat the same contact.
     - The schedule action must update only 2 contacts on every execution.

> Note: we do not need you to do all of the tasks, but more than you do, more we know your skills.

## Deliverables

1. Github repository with each module inside.

## References

- [What is Odoo?](https://www.odoo.com/)
- [Docker and Odoo](https://hub.docker.com/_/odoo)
- [Odoo Runbot](https://runbot.odoo.com/)
- [Dockerdoo](https://github.com/iterativo-git/dockerdoo)
- [Dev Container Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
