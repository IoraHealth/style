{% highlight ruby %}
# Too much going on
result = number % 2 == 0 ? number % 4 : number / 3

# Just enough going on
result = if number % 2 == 0
  number % 4
else
  number / 4
end
{% endhighlight %}
