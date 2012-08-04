{% highlight ruby %}
class Ninja
  include SilentWarrior

  ROCK_HARD_AWESOME = true

  attr_accessor :weapon

  def initialize(weapon)
    @weapon = weapon
  end

  def sneak_attack
    case @weapon
    when ThrowingStar
      attack_with_throwing_star
    else
      flip_out_and_stuff
    end
  end

  def attack_with_throwing_star
    "YOU'VE BEEN NINJADDDDDD"
  end

  def flip_out_and_stuff
    "YOU HAVE ALSO BEEN NINJADDDDD"
    disappear_into_darkness
  end

  def self.create_with_throwing_star(throwing_star_name = 'Pinkie Pie')
    weapon = ThrowingStar name: throwing_star_name

    Ninja.new weapon
  end

  private
  def disappear_into_darkness
    throw_powder #implemented in SilentWarrior
    "LOLOLOLOL INVISIBLE"
  end
end
{% endhighlight %}
