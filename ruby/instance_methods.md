instance methods
========================

If classes are cookie cutters, instances are cookies. Cookie cutters define what individual cookies are like.

Class methods are the things that all instances of a particular class can do. All cookies can bake and be_delicious and go_stale and make_you_fat.

Instance methods are the individual cookies doing the things that all cookies can do (and sometimes things that not all cookies can do).

```
  bretts_cookie.make_you_fat
```

Will make Brett fat, since it's an instance of cookie that's being eaten by Brett. Brett is an instance of the Person class, and so bretts_cookie won't make Roger fat; Roger is another instance of the Person class that now his own attributes and methods that aren't affected by Brett's eating the cookie.

Check this link for a more detailed look at [Class Methods](https://github.com/brettshollenberger/codecabulary/blob/master/ruby/class_methods.md)
