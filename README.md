# Building Project Manage App using Rails and Vue.js

## STEPS

# VIDEO 1

## 1. Create the app
## 2. modified:   Gemfile and modified:   README.md
## 3. Added vue: $ yarn add vue-turbolinks
## 4. Add vue: $ yarn add vue-resource
## 5. Added mailcatcher
## 6. Git: added 3-5
        modified:   README.md
        modified:   config/environments/development.rb
        modified:   package.json
        modified:   yarn.lock
## 7. Add gem devise
## 8. Create controller home index
## 9. Add home route
## 10. Modified app layout
## 11. Use guard : > guard init livereload ; > bundle exec guard
        new file:   Guardfile
        new file:   GuardfileX
        new file:   app/assets/javascripts/home.coffee
        renamed:    app/assets/stylesheets/application.css -> app/assets/stylesheets/application.css.scss
        new file:   app/assets/stylesheets/home.scss
        new file:   app/controllers/home_controller.rb
        new file:   app/helpers/home_helper.rb
        new file:   app/views/devise/confirmations/new.html.erb
        new file:   app/views/devise/mailer/confirmation_instructions.html.erb
        new file:   app/views/devise/mailer/email_changed.html.erb
        new file:   app/views/devise/mailer/password_change.html.erb
        new file:   app/views/devise/mailer/reset_password_instructions.html.erb
        new file:   app/views/devise/mailer/unlock_instructions.html.erb
        new file:   app/views/devise/passwords/edit.html.erb
        new file:   app/views/devise/passwords/new.html.erb
        new file:   app/views/devise/registrations/edit.html.erb
        new file:   app/views/devise/registrations/new.html.erb
        new file:   app/views/devise/sessions/new.html.erb
        new file:   app/views/devise/shared/_error_messages.html.erb
        new file:   app/views/devise/shared/_links.html.erb
        new file:   app/views/devise/unlocks/new.html.erb
        new file:   app/views/home/index.html.erb
        modified:   app/views/layouts/application.html.erb
        modified:   config/environments/development.rb
        new file:   config/initializers/devise.rb
        new file:   config/initializers/simple_form.rb
        new file:   config/locales/devise.en.yml
        new file:   config/locales/simple_form.en.yml
        modified:   config/routes.rb
        new file:   lib/templates/erb/scaffold/_form.html.erb
        new file:   test/controllers/home_controller_test.rb

# 12.  Create User model:

        $ rails g devise User;
        $ rails db:migrate
        $ rails g migration AddNameToUsers name:string
        $ rails db:migrate
        $ rails g migration AddTeamIdToUsers team_id:integer
        $ rails db:migrate

        $ git status
        new file:   app/controllers/confirmations_controller.rb
        new file:   app/controllers/registrations_controller.rb
        new file:   app/models/concerns/log_validation_errors.rb
        new file:   app/models/user.rb
        modified:   app/views/devise/confirmations/new.html.erb
        new file:   app/views/devise/confirmations/show.html.erb
        modified:   app/views/devise/mailer/confirmation_instructions.html.erb
        modified:   app/views/devise/mailer/email_changed.html.erb
        modified:   app/views/devise/mailer/password_change.html.erb
        modified:   app/views/devise/mailer/reset_password_instructions.html.erb
        modified:   app/views/devise/mailer/unlock_instructions.html.erb
        modified:   app/views/devise/passwords/edit.html.erb
        modified:   app/views/devise/passwords/new.html.erb
        modified:   app/views/devise/registrations/edit.html.erb
        modified:   app/views/devise/registrations/new.html.erb
        modified:   app/views/devise/sessions/new.html.erb
        deleted:    app/views/devise/shared/_error_messages.html.erb
        modified:   app/views/devise/shared/_links.html.erb
        modified:   app/views/devise/unlocks/new.html.erb
        modified:   app/views/layouts/application.html.erb
        modified:   config/initializers/devise.rb
        modified:   config/routes.rb
        new file:   db/migrate/20190918152155_devise_create_users.rb
        new file:   db/migrate/20190918155447_add_name_to_users.rb
        new file:   db/migrate/20190918155650_add_team_id_to_users.rb
        new file:   db/schema.rb
        new file:   test/fixtures/users.yml
        new file:   test/models/user_test.rb







