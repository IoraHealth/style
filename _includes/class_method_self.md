{% highlight ruby %}
class Ninja
  # apparently string replacement is hard here
  def Ninja.create_with_claw
    Ninja.new Claw.new('doris')
  end
end

class Ninja
  # so much more resilient
  def self.create_with_claw
    Ninja.new Claw.new('doris')
  end
end
{% endhighlight %}
