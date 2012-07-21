{%highlight ruby %}
# Checking equality
if pants_off_dance_off == Time.now
  take_pants_off
end

# Assigning a value and checking equality
if (pants_off_dance_off = Party.party_o_clock) == Time.now
  PartyQueue.enqueue pants_off_dance_off
end
{% endhighlight %}
