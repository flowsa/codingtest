# Flow API (Laravel) Developer Test

This is a test to review knowledge and understanding of basic API principles.

Click "use this template" and "create a new repository" in Github to get started

![image](https://user-images.githubusercontent.com/17523844/218440440-760e900a-8676-4f98-8b64-5e041dc09e8f.png)


## Brief

This is an API for a todo list application, but we've a couple issues we need to resolve. 

We have a test suite but some of the tests are failing due to some bugs we've intentionally added.

**Look through the application logic and fix it so that the tests pass. Do not edit the tests!**

1) Tests\Feature\TodoListTest::test_todos_list_can_only_be_updated_by_owner
2) Tests\Feature\TodoListTest::test_todos_list_can_only_be_deleted_by_owner
3) Tests\Feature\TodoListTest::test_deleting_a_todo_list_deletes_all_todos
4) Tests\Feature\TodoListTest::test_get_all_todo_lists
5) Tests\Feature\TodoListTest::test_todo_lists_search
6) Tests\Feature\TodoTest::test_update_todos_to_complete_updates_list_status
7) Tests\Feature\TodoTest::test_adding_todo_to_complete_list_updates_list_status
8) Tests\Feature\UserTest::test_user_register

And then secondly, some of the clients that are integrating into this often forget to include the correct headers, so then we're finding that they're being returned redirects and HTML when they hit a route thats unauthorised etc.

Can you please set this to only return `JSON` regardless of headers for all API routes? Can you also please add a test so we don't accidently run into this again.

To run the tests use `php artisan test` to run the PHPUnit test suite.

### Working Environment
You are welcome to use your own PHP development environment.
Typically this would include
1. Cloning the repository
2. Running `composer install`
3. Running `php artisan key:generate`
4. Running `php artisan migrate:fresh`
5. Running `php artisan serve`

There is also a DDEV setup. If you have DDEV installed, simply run `ddev start`. 

### Testing
There is a Postman test suite and enviroment, to use please point the `baseUrl` variable to eg `http://127.0.0.1:8000` or wherever you are serving the application from.

NB: This collection has been setup to test userflow so has been designed to run as a collection, individual tests may fail based on environment variables being set in previous tests.


### Submission
Click "use this template" and "create a new repository" in Github and commit your work to this new repo. Please then update this `Readme` with details of how to get the application standing and or details of where this is staged if you are serving it yourself.

Please update the Postman Environment to match any variable criteria (eg, `baseUrl` etc)

Please remember to allow the Github user `richardfrankza` to have access to this repo in order for us to review.

Good luck!
