{% highlight ruby %}
# I hate unecessary code
def wasted_code_is_awesome
  begin
    do_something_error_prone
  rescue StandardError => e
    p 'I GOBBLE UP ALL THE ERRORS!'
  rescue IOError => e
    p 'I am the lonliest error block'
  end
end

# now we're talking
def every_line_of_code_is_a_liability
  begin
    do_something_error_prone
  rescue IOError => e
    p 'NOW ITS MY TIME TO SHINE'
  rescue StandardError => e
    p 'I miss all the IOErrors :('
  end
end
{% endhighlight %}
