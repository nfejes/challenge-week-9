# Name

Niklas Fejes

# How many points have you earned?

100/100


# How many hours have you spent on this?

6 hours

# When did you first start working on this week's learning challenges?

Saturday (25/10/14)

# What is the most difficult part about this week's challenge?

fill-in-your-answer

# Show and tell (8 points)

## Link (2 points)

[title-of-the-article](http://link-to-an-article-about-machine-learning-use-for-big-data)

## Discuss how you may apply the machine learning technique mentioned in this article to another interesting problem (6 points).

fill-in-your-answer

# D3 IV

## Checkpoints (3 points x 4 = 12 points)

# 1. (3 points)

![image](screenshots/d3/checkpoint1.png?raw=true)

[checkpoint](html/checkpoint1.html)

# 2. (3 points)

![image](screenshots/d3/checkpoint2.png?raw=true)

[checkpoint](html/checkpoint2.html)

# 3. (3 points)

![image](screenshots/d3/checkpoint3.png?raw=true)

[checkpoint](html/checkpoint3.html)

# 4. (3 points)

![image](screenshots/d3/checkpoint4.png?raw=true)

[checkpoint](html/checkpoint4.html)

## Challenges (4 points x 3 = 12 points)

# 1. (4 points)

![image](screenshots/d3/challenge1.png?raw=true)

# 2. (4 points)

![image](screenshots/d3/challenge2.png?raw=true)

# 3. (4 points)

![image](screenshots/d3/challenge3.png?raw=true)

[challenge3](html/challenge3.html)



# MongoDB II

## Checkpoints (6 points x 2 = 12 points)

### 1 (6 points)

[mongodb js code collecting github events about our course](mongodb-github.js)

### 2 (6 points)

![terminal output of mongodb query](screenshot.png?raw=true)

## Challenge 1 (4 points x 10 = 40 points)

### 1 (4 points)

`> db.course_events.findOne({'actor.login' : 'doubleshow' });`

![screenshot](screenshot.png?raw=true)

### 2 (4 points)

`> db.course_events.findOne({ 'actor.login' : 'doubleshow' }, { actor : 1 });`

![screenshot](screenshot.png?raw=true)

### 3 (4 points)

`> db.course_events.find({'actor.login' : {$in : ['doubleshow','chrisbopp']}},{'actor.login':1,created_at:1});`

![screenshot](screenshot.png?raw=true)

### 4 (4 points)

`> db.course_events.findOne({'type' : 'PushEvent' });`

![screenshot](screenshot.png?raw=true)

### 5 (4 points)

`db.course_events.find({'type' : 'PushEvent' }, {'payload.commits.author.name' : 1});`

![screenshot](screenshot.png?raw=true)

### 6 (4 points)

`db.course_events.findOne({'type' : 'IssuesEvent' }, {payload : 1});`

![screenshot](screenshot.png?raw=true)

### 7 (4 points)

`> db.course_events.find({'type' : 'IssuesEvent' }, { 'payload.issue.user.login' : 1});`

![screenshot](screenshot.png?raw=true)

### 8 (4 points)

`> db.course_events.find({'type':'IssuesEvent','payload.issue.state':'closed'}, {'payload.issue.id':1,'payload.issue.state':1});`

![screenshot](screenshot.png?raw=true)

### 9 (4 points)

`> db.course_events.find({'type':'IssuesEvent','payload.issue.state':'open'}, {'payload.issue.user.login':1,'payload.issue.state':1});`

![screenshot](screenshot.png?raw=true)

### 10 (4 points)

`> db.course_events.find({type:'IssuesEvent','payload.issue.comments':{$gt:0}}, {'payload.issue.user.login':1,'payload.issue.comments':1});`

![screenshot](screenshot.png?raw=true)


## Challenge 2 (8 points x 2 = 16 points) 

### 1 (8 points)

{question-in-plain-English}

> db.course_events.[complete this query]

![screenshot](screenshot.png?raw=true)

### 2 (8 points)

{question-in-plain-English}

> db.course_events.[complete this query]

![screenshot](screenshot.png?raw=true)
