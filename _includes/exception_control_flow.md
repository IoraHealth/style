{% highlight ruby %}
# bad
begin
  n / d
rescue ZeroDivisionError
  puts 'Cannot divide by 0!'
end

# good
if d.zero?
  puts 'Cannot divide by 0!'
else
  n / d
end
{% endhighlight %}
