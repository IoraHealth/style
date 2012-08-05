{% highlight ruby %}
string = "line ending\nusername"
string[/^username$/]   # matches
string[/\Ausername\Z/] # does not match
{% endhighlight %}
