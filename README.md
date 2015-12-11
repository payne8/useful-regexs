# useful-regexs
This is a place to put any useful regular expressions I find. Feel free to submit pull requests with your own!

# Java
Match everything before the hour in an iso date:

```
s/^[0-9]{4}-[0-9]2-[0-9]2T//
```

Match everything after the hour in an iso date:
```
s/[0-9]{2}:[0-9]{2}$//
```
