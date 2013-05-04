class methods
========================

Classes are cookie cutters for types of things. Imagine you're playing God: You have your model for dogs, and your model for people, and your model for trees. People are capable of abstract thought and computer programming and dogs are capable of running long distances and charming the pants off of anyone and trees are capable of photosynethsis and winning most blinking contests. So it goes.

When you use your people model, you make an instance of a person. They have the essential characteristics of a person. Unless they don't. Because every person can learn new things and acquire new skills (methods, to use the Ruby term), and they can change the characteristics they already have and have all sorts of genetic differences.

The beauty of classes is the ability to make a bunch of the same thing from a common archetype, and then to only discuss the differences between the individual instances of those things. That way when you're playing God, you don't have to say "I create Rob and he has two legs," and "I create Brett and he has two legs," and "I create Xavier and he has two legs, too." You just say, "People have two legs unless I define a specific person with more or less legs." Much easier.

Class methods are all the verbs that things starting from a common archetype can do. VCRs (if you're old enough to remember such things) could play tapes and rewind tapes and eat tapes and blink 12:00 indefinitely. Those were all the things a VCR could do, unless you hacked it to give it some new capabilities that were unique to your VCR. You could even remove those other capabilities, so that you VCR-like thing no longer much resembled a VCR. But that's a story for another day, grandson.

The class block defines all those verbs. The class block is flagged using the class keyword, then the name of the archetypal thing (VCR), and then, optionally, another thing to inherit characteristics from. This is (in Ruby) how evolution works: You base homo erectus off of homo habilis; homo erectus inherits all the capabilities of homo habilis and then begins to diverge and take on a life of its own. VCRs aren't inheriting from other things though, so we'll just define a VCR, which inherits intrinsically from object without us needing to specify it explicitly (VCRs are objects, after all).

```
  class VCR

    def play_tape(tape)
      if tape.is_in && play._is_pressed
        for frame in tape
          print frame
        end
      else
        blink_1200_forever_and_ever()
      end
    end
```

[Instance methods](https://github.com/brettshollenberger/codecabulary/blob/master/ruby/instance_methods.md) are the new things that individual VCRs learn to do when you hack them. They're also just examples of an individual performing a class method. For instance, if bretts_vcr.eats_tape, eats_tape is an instance method, since my VCR did the eating. For the most part, in practice, you'll call methods on particular instances of classes, since instances are the ones doing most of the stuff. Very rarely, in code or reality, do our gods make the "idea" of people "sleep talk," or whatever, but I suppose it could be done.
