# The Odin Project
## Sub Strings

This repo contains my implementation of the Sub Strings project as described in The Odin Project.

The documentation says to: 

  ```Implement a method #substrings that takes a word as the first argument and then an array of valid substrings (your dictionary) as the second argument. It should return a hash listing each substring (case-insensitive) that was found in the original string and how many times it was found.```
  
and gives these examples:

single word support

```ruby
  > dictionary = ["below","down","go","going","horn","how","howdy","it","i","low","own","part","partner","sit"]
  => ["below","down","go","going","horn","how","howdy","it","i","low","own","part","partner","sit"]
  > substrings("below", dictionary)
  => { "below" => 1, "low" => 1 }
```
Mulitple word support

```ruby
  > substrings("Howdy partner, sit down! How's it going?", dictionary)
  => { "down" => 1, "go" => 1, "going" => 1, "how" => 2, "howdy" => 1, "it" => 2, "i" => 3, "own" => 1, "part" => 1, "partner" => 1, "sit" => 1 }
```

## substrings.rb

I decided to create a method that first initializes a new hash to count all the words then it loops through each word inside the passed dictionary, For each word in the dictionary it checks to see if that word is included in the string and if it is then scans for the number of times that word is inside the string finally returning the original hash with all the words and associated counts.

[Source](https://www.theodinproject.com/lessons/ruby-sub-strings)
