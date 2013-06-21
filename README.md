DSSG Fellows Python Data Dictionary
============

A dictionary to describe DSSG's fellows and how awesome they are. Each fellow interviews the others as an (extremely nerdy) ice-breaker. May lead to visualizations and analyses.

Steps to play along:

**1) Create a file which contains your dictionary.**

`<first_name>_<last_name>.json`

Suggested format for the dictionary is

(see `example.json`)

```
{
  "name1" : "answer",
  "name2" : "answer2"
  //etc 
}
```

or

```
{
  "name1" : {
    "question_tag1": "answer1-1",
    "question_tag2": "answer1-2"
  },
  "name2" : {
    "question_tag1": "answer2-1",
    "question_tag2": "answer2-2"
  }
  //etc
}
```

**2) Document your name and question in this `README.md` file.

How to Save and Load JSON files
====

Read from a JSON file

```
import json

f = open('example.json')

# Read input file to JSON. Python might explode if your JSON is poorly formatted!
d = json.load(f)

#   d ->
#   {u'Adam Fishman': u'',
#   ...
#   u'Zahra Ashktorab': u''}
```

```
import json

# Create Python dictionary
d = { "key":"value" }

# Convert dictionary to JSON
my_json = json.dumps(d)

# Write JSON to file
new_file = open('new.json', 'w')
new_file.write(my_json)
new_file.close()
```

Names and questions
====

- Nathan Leiby - What is your favorite character from a book, play, movie, etc?
- <person 2> - <question(s)>
- ...



