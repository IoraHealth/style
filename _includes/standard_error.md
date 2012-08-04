{% highlight ruby %}
# Please don't let this method eat your children
def will_eat_your_children
  exit
rescue Exception
  puts 'Mission Accomplished!'
end

# We have avoided children eating on this day
def will_eat_your_children
  exit
rescue => e
  puts 'DAG'
end

# You can even be very explicit
def will_eat_your_children
  exit
rescue StandardError => e
  puts 'DAG AGAIN'
end
{% endhighlight %}
