# useful-regexs
This is a place to put any useful regular expressions I find. Feel free to submit pull requests with your own!

# Java
Match everything before the hour in an iso date:

```
s/^[0-9]{4}-[0-9]2-[0-9]2T//

```
e.g. 
string: '2015-12-22T20:05:00'
matches '2015-12-22T'
ignores everything not following

Match everything after the hour in an iso date:
```
s/[0-9]{2}:[0-9]{2}$//
```

e.g. 
string: '2015-12-22T20:05:00'
matches '05:00'
ignores everything before it


# Javascript
Find all instances where there is a comma without a trailing space.

```
,[^\s]
```

e.g.
string: '_.findWhere(schema,{ 'name': action.sourceColumn } );'
matches: ',{'
useful for finding those pesky code style faux pas.
