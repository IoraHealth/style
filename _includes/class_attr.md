{% highlight ruby %}
class Cat
  class << self
    attr_reader :capable_of_purring
  end
  @capable_of_purring = true

  def purr
    pust "prrrrr" if @capable_of_purring
  end
end

class Lion < Cat
  @capable_of_purring = false
end

Cat.purr # => "prrrr"
Lion.purr # => outputs nothing! yay.
{% endhighlight %}
