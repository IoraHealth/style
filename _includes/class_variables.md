{% highlight ruby %}
class Cat
  @@capable_of_purring = true

  def self.purr
    puts "prrrrrrrrrr" if @@capable_of_purring
  end
end

class Lion < Cat
  @@capable_of_purring = false
end

Cat.purr # => prints nothing :(
{% endhighlight %}
