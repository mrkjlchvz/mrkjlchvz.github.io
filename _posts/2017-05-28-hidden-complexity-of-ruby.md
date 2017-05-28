---
layout: post
title: The Hidden Complexity of Ruby
---

Ruby's simplicity has reached a whole new level. It has given developers a new approach to writing code. For me, coding
should be fun and that's what Ruby has always been. It has enabled us to not think about code too much but focus
more on how we can give values to our customers.

Why am I saying this?

Because once a developer has focused on the customer, it keeps them happy and we get to keep our jobs. More value means success.

To demonstrate how simple this language is, let me show you a block of code.

```ruby
list_of_characters = Character.all

list_of_characters.each do |character|
  puts character.name
  puts "List of weapons:"

  character.weapons.each do |weapon|
    puts weapon.name
  end
end
```

The above code is simple, and easy to understand. But this is something that has a hidden cost. In the context of Rails,
we call this the `N+1` problem. This article is not going to discuss the `N+1` problem but conceptually, it means more
unnecessary database calls and performance issues.

What I am trying to say is that developers new to Ruby or Rails may have abused the simplicity that `ruby` offers. This is just one of the many problems that `ruby` developers has to be aware of. No wonder that there are a lot of `Ruby on Rails is dead.` and `Ruby on Rails does not scale.` articles showing up on the web and it really creeps me up.

It's about time to step up and stop blaming `ruby` for whatever problems that we have. Because it is a language that scales and performs very well just like any other languages.

We can start by understanding how Ruby's GC works. Or learn how to benchmark effectively. Let's know when and when not to
use `ActiveRecord` for our queries and many more!

Make it simple.