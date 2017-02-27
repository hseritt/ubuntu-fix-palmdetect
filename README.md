# Fix your Ubuntu Laptop's Palm Detection

Are you having a problem with your Ubuntu laptop where your mouse cursor jumps everywhere while you're trying to type? If so, create a script called 'fixtouchpad', put it in ~/bin and make it exectuable.

Inside the file, put:

```
#!/usr/bin/env bash

pkill syndaemon
syndaemon -i 1 -KRd
```

Save it. Done.

On startup, you can run:

# fixtouchpad

And then the palm detection problem is now fixed. Mostly. Try it and let me know if you have any problems with it.
