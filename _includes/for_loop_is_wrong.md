{% highlight ruby %}
for num in [1..12] do
  puts num % 2
end

# This is just plain wrong.
puts num # => 12

[1..12].each { |num| puts num % 2 }

puts num # => NoMethodError

{% endhighlight %}
