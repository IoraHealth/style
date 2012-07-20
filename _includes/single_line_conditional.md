{% highlight ruby %}
# Not the greatest
def send_tweet(message)
  if message.length <= 140
    TwitterStream.enqueue message
  end
end

# Better
def send_tweet(message)
  TwitterStream.enqueue(message) if message.length <= 140
end

# Bettererer
def send_tweet(message)
  TwitterStrem.enqueue(message) if message.usable_on_twitter?
end

{% endhighlight %}
