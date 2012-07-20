{% highlight ruby %}
# vertical space following variable assignment
def allowed_in_restaurant?
  shirt = true
  pants = false
  shoes = true

  shirt && pants && shoes
end

# vertical space following multi-line block
def rock
  1..12.each do |hour|
    ready_to_rock?
 end

 rock_around_the_clock_tonight
end
{% endhighlight %}
