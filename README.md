# relational_rails
## Mod2 Solo Project #1

### Learning Goals
- Design a one-to-many relationship using a schema designer.
- Write migrations to create tables with columns of varying data types and foreign keys.
- Use Rails to create web pages that allow users to CRUD resources.
- Create instance and class methods on a Rails model that use ActiveRecord methods and helpers.
- Write model and feature tests that fully cover data logic and user behavior.

### Requirements
- must use Rails 5.2.x
- must use PostgreSQL
- must “handroll” all routes (no use of resources syntax)

### Permission
- If there is a specific gem you’d like to use in this project that is not mentioned on this project page, you must get permission from your instructors first.

### Setup
- Students should create their own new Rails app for this project. Students can reference the [Task Manager](https://backend.turing.edu/module2/projects/relational_rails/#:~:text=Task%20Manager%20tutorial%20app) tutorial app for how to set up a new Rails project.
- Students must host their code in a new repository on GitHub.

### Evaluation
- [Peer code share](https://backend.turing.edu/module2/projects/relational_rails/#:~:text=Evaluation-,Peer%20code%20share,-%2C%20evaluation%2C%20and%20rubric), evaluation, and rubric information can be found [here](https://backend.turing.edu/module2/projects/relational_rails/evaluation).

### Relationships
#### Design your database
Read this [lesson plan](https://backend.turing.edu/module2/lessons/one_to_many_relationships) and use it as a reference when designing your database.

Each student will come up with their own one-to-many relationship. This should represent a real world example of your choice.

Do not use “Parent”/”Child” as your relationship.

You can create as many columns on each table as you would like, but we need a few columns represented on each table:
- One string column for a ‘name’
- One boolean column
- One numeric column
- Two DateTime columns: created_at and updated_at

A couple of things to keep in mind as you’re designing your schema:
- Foreign Keys do not count as an integer column.
- You should not create columns that duplicate data. For example, in Parent/Child, a Parent should not store a “child_count” column since the count of Children can also be found by counting the number of associated children.

### User Stories
A user story is a concise description of functionality that a specific user should experience while using your application. In these stories, we will refer to the “one” side of the relationship as the “parent” and the “many” side of the relationship as the “children/child”.

Each user story will focus on one of the following:
- ActiveRecord
- CRUD Functionality
- Usability: Users should be able to use the site easily. This means making sure there are links/buttons to reach all parts of the site and the styling/layout is sensible.

Note: When writing code for each user story, it is important to go in numerical order; don’t jump around. You may notice some later user stories “overwriting” earlier stories - this is intentional and mimics what you may experience on the job when working with real clients.