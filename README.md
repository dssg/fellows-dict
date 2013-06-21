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
- Jette Henderson - 1. What is your spirit animal? 2. Do you prefer to read fiction or non-fiction?
- Emily Rowe - Where do you fall in your family's birth order (position)? How many children are in your family? Example: Someone whose position is 2 and number of children is 3 is the second of three children.
- Adam Fishman - What is your favorite question?
- Joe Walsh - If you could do any experiment, what experiment would you do? 
- Breanna Miller - What is your favorite pasta shape?
- Kwang-Sung Jun - For laptop keyboard, there are weird layouts for insert, delete, home, end, page up, and page down keys. Which one do you prefer? Choices are do-not-care, six-pack, in-a-row, fn-key-with-arrow. null value was used to denote "did not ask".
- <person 5> - <question(s)>
- ...



