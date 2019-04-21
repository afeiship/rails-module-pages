# rails-module-pages
> Rails module for pages(like about/help/contact...).

## rails
~~~
$ ./bin/rails -v
Rails 5.2.3
~~~

## initialize:
```bash
cd ~/github/rails-module-pages
rails new .
bundle install
```

## rails s
```shell
# mv Gemfile / .ruby-version: 2.6.1
./bin/rails s
```


## migrate rails_pages
1. Add rails_pages gem
   ```rb
   gem 'rails_pages', git: 'https://github.com/afeiship/rails_pages'
   ```
2. Initial config file
   ```shell
   # initilal
   ./bin/rails g rails_pages:initializer
   # eidit: ./config/initializers/rails_pages.rb
   config.pages = ["help", "about"]
   ``` 
3. Installl pages
   ```shell
   ./bin/rails g rails_pages:install
   ```
4. preview
   http://localhost:3000/rails_pages/help
   http://localhost:3000/rails_pages/about

5. Or you can modify the mounted_at
   ```rb
   # ./config/routes.rb
   Rails.application.routes.draw do
    mount RailsPages::Engine => "/rails_pages"
    # For details on the DSL available within this file, see http://guides.rubyonrails.org/routing.html
   end
   ```

## resources:
+ https://ruby-china.org/topics/3313
