# Rails Template

Application template used for creating new Rails only applications. For API only applications, see [Rails API Template](https://github.com/ayrt-n/rails-api-template) repo.

The template it based off of the template provided in "The Complete Guide to Rails Testing" by Jason Swett.

To use the template when creating a new rails application, you must append "-m https://raw.githubusercontent.com/ayrt-n/rails-template/main/application_template.rb" to the end of your call to rails new, like so:

```
rails new new_rails_api -d=postgresql -T -m https://raw.githubusercontent.com/ayrt-n/rails-api-template/main/application_template.rb
```

## Application Template Details

The application_template automagically adds a number of rails related testing gems (including rspec-rails).

The template will create a generators.rb config file to turn off the creation of view and controller specs, when generating new rails models/controllers.

Lastly, it will bundle install all gems and then set rspec up by ```running rails generate rspec:install```