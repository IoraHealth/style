{% highlight ruby %}
module Smurf
  class Papa
    attr_accessor :hat
    @hat = 'red'
  end

  class Nerdy
    attr_accessor :glasses
    @glasses = true
  end
end

Smurf::Papa.new.hat # => 'red'
Smurf::Nerdy.new.glasses # => true
{% endhighlight %}
