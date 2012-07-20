{% highlight ruby %}
# Future arrest pending
pants_on = false

def can_go_outside?(pants_status)
  pants_status ||= true

  pants_status
end

can_go_outside? pants_on # => true

# Safety from prosecution
def can_go_outside?(pants_status)
  pants_status = true if pants_status.nil?

  pants_status
end

can_go_outside? pants_on # => false
{% endhighlight ruby %}
