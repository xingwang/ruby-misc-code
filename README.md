# ruby-misc-code

Just a couple notes for quick referencing in the future in case I forget.

1) Use %Q to add double quotes around a string for cleaner looking strings that require double quotes.

```ruby
puts %Q|{"message":"Malformed url #{image[:uri]}", "_id": "#{@test["_id"]}", "field_name": "#{image[:description]}"}|
```
A pretty good read up can be found [here](https://simpleror.wordpress.com/2009/03/15/q-q-w-w-x-r-s/)

2) When including a class, the main class gets access to all the included class's methods. The included class also gets access to the main class's instance variables.

```ruby
class First
  include Second
  def initialize
    @monkey = "wont do"
  end
end

class Second
  def what_about_the_monkey
    puts @monkey #prints out "wont do"
  end
end
```

3) In Ruby, valid JSON **requires double quotes** unlike Javascript where the preferred way is with single quotes.

4) In Ruby, the **&** does way too much. Good read found [here](http://www.skorks.com/2013/04/ruby-ampersand-parameter-demystified/)
