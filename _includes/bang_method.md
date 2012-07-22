{% highlight ruby %}
class Array
  def flatten_once!
    res = []
    each do |e|
      [*e].each {|f| res << f }
    end
    replace(res)
  end

  def flatten_once
    dup.flatten_once!
  end
end
{% endhighlight %}
