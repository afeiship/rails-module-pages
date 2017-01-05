#rails-module-pages
> Rails module for pages(like about/help/contact...).

## initialize:
```bash
cd ~/github/rails-module-pages
rails new .
bundle install
```

## generate static pages:
```bash
rails generate controller StaticPages about help --no-test-framework
rails destroy controller StaticPages home help
```
## resources:
+ https://ruby-china.org/topics/3313
