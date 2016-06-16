# ruby-misc-code

Just a couple notes for quick referencing in the future in case I forget.

1) Use %Q to add double quotes around a string for cleaner looking strings that require double quotes.

```ruby
puts %Q|{"message":"Malformed url #{image[:uri]}", "_id": "#{@test["_id"]}", "field_name": "#{image[:description]}"}|
```
A pretty good read up can be found [here](https://simpleror.wordpress.com/2009/03/15/q-q-w-w-x-r-s/)
