1. $ rails new todo

2. $ rails generate model Item title:string description:text

3. $ rake db:migrate

4. $ rake routes

5. $ rails generate controller Items

6. add simple_form && bootstrap-sass to Gemfile

7. $ bundle install

8. configure bootstrap-sass

9. configure simple_form

10. add resources :items to routes.rb

11. add index, new and _form __ partial in views/items

12. add index and new actions to items_controller.rb

13. add show action to items_controller.rb

14. add show.html.erb to views/items

15. add edit, update && destroy actions to items_controller.rb

16. create views/items/edit.html.erb

17. add devise to Gemfile

18. configure devise
    - $ rails generate devise:install
    - add to config/environments/development.rb:
       config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }
    - add to app/views/layouts/application.html.erb.
       <p class="notice"><%= notice %></p>
       <p class="alert"><%= alert %></p>
    - $ rails g devise:views

19. $ rails generate devise User

20. $ rake db:migrate

21. restart the server

22. add navbar to application.html.erb

23. create Associations between User && Items
    - item belongs to a user
    - user has many items
    - $ rails generate migration add_user_id_to_items user_id:integer
    - $ rake db:migrate
