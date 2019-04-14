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


## generate static pages:
```bash
rails generate controller StaticPages about help --no-test-framework
rails destroy controller StaticPages home help
```
## resources:
+ https://ruby-china.org/topics/3313
