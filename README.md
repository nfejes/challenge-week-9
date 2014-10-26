# Name

Niklas Fejes

# How many points have you earned?

100/100


# How many hours have you spent on this?

6 hours

# When did you first start working on this week's learning challenges?

Saturday (25/10/14)

# What is the most difficult part about this week's challenge?

Nothing was outstandingly difficult, but if something the review of how to use mongodb.

# Show and tell (8 points)

## Link (2 points)

[Big Data Digest: Rise of the think-bots](http://www.pcworld.com/article/2839092/big-data-digest-rise-of-the-thinkbots.html)

## Discuss how you may apply the machine learning technique mentioned in this article to another interesting problem (6 points).

The article talks about a API service that can be used by companies to get its data automatically analyzed with machine learning
on the cloud. The same technique could be used to detect anomalies in the data flow from logs or user data to automatically detect
and alert the company about possible bugs or events they may otherwise not notice.

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

![terminal output of mongodb query](screenshots/mongodb/checkpoint2.png?raw=true)

## Challenge 1 (4 points x 10 = 40 points)

### 1 (4 points)

`> db.course_events.findOne({'actor.login' : 'doubleshow' });`

![screenshot](screenshots/mongodb/challenge1.png?raw=true)

### 2 (4 points)

`> db.course_events.findOne({ 'actor.login' : 'doubleshow' }, { actor : 1 });`

![screenshot](screenshots/mongodb/challenge2.png?raw=true)

### 3 (4 points)

`> db.course_events.find({'actor.login' : {$in : ['doubleshow','chrisbopp']}},{'actor.login':1,created_at:1});`

![screenshot](screenshots/mongodb/challenge3.png?raw=true)

### 4 (4 points)

`> db.course_events.findOne({'type' : 'PushEvent' });`

![screenshot](screenshots/mongodb/challenge4.png?raw=true)

### 5 (4 points)

`db.course_events.find({'type' : 'PushEvent' }, {'payload.commits.author.name' : 1});`

![screenshot](screenshots/mongodb/challenge5.png?raw=true)

### 6 (4 points)

`db.course_events.findOne({'type' : 'IssuesEvent' }, {payload : 1});`

![screenshot](screenshots/mongodb/challenge6.png?raw=true)

### 7 (4 points)

`> db.course_events.find({'type' : 'IssuesEvent' }, { 'payload.issue.user.login' : 1});`

![screenshot](screenshots/mongodb/challenge7.png?raw=true)

### 8 (4 points)

`> db.course_events.find({'type':'IssuesEvent','payload.issue.state':'closed'}, {'payload.issue.id':1,'payload.issue.state':1});`

![screenshot](screenshots/mongodb/challenge8.png?raw=true)

### 9 (4 points)

`> db.course_events.find({'type':'IssuesEvent','payload.issue.state':'open'}, {'payload.issue.user.login':1,'payload.issue.state':1});`

![screenshot](screenshots/mongodb/challenge9.png?raw=true)

### 10 (4 points)

`> db.course_events.find({type:'IssuesEvent','payload.issue.comments':{$gt:0}}, {'payload.issue.user.login':1,'payload.issue.comments':1});`

![screenshot](screenshots/mongodb/challenge10.png?raw=true)


## Challenge 2 (8 points x 2 = 16 points) 

### 1 (8 points)

When were pull requests made?

`> db.course_events.find({type : 'PullRequestEvent'},{'actor.login':1,created_at:1});`

![screenshot](screenshots/mongodb/challenge11.png?raw=true)

### 2 (8 points)

How many files were changed in the pull requests?

`> db.course_events.find({type : 'PullRequestEvent'},{'payload.pull_request.changed_files':1,'actor.login':1});`

![screenshot](screenshots/mongodb/challenge12.png?raw=true)
