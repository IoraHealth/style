{% highlight ruby %}
def format_party_time(start_time, end_time)
  start_hour = start_time.strftime '%h'
  end_hour   = end_time.strftime '%h'

  # Calculate party things here.
end
{% endhighlight %}
