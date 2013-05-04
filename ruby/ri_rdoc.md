ri and RDoc
========================

ri (Ruby Index) and RDoc (Ruby Documentation) provide documentation about Ruby programs. Both include command-line tools that can be installed using [Ruby Version Manager](http://github.com/rvmlink). You can check out our RVM page for info on installing RVM.

```
  #> rvm docs generate
```

Once ri is installed, you can use it to request information about Ruby. Let's say you just saw string.upcase used in a StackExchange article. You can quickly look up info on the .upcase method by typing:

```
ri String#upcase
```

The call to ri will return documentation, like this:


