.bash_profile
========================

The .bash_profile is executed for login shells, meaning any Mac OSX Terminal Window by default. Most other graphic user interfaces (GUIs) that emulate terminals tend to use .bashrc instead.

Since it can be a hassle to maintain two separate configuration files for login and non-login shells, you can source .bashrc from your .bash_profile by adding the following lines to your .bash_profile:

```
if [ -f ~/.bashrc ]; then
   source ~/.bashrc
fi
```

And then storing common settings in .bashrc. This change will automatically call .bashrc when you open a console instead of .bash_profile.



