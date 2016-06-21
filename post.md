```
This is the first of at least an 8 part serious I'm excited to share. The rough plan over the next 8-12 weeks is looking like:

- p2: BIG Schema, SMALL Payloads: MongoDB & Express Data Patterns
- p3: ES6 on NodeJS
- p4: Semantic Middleware
- p5: Lazy Loading Requires for SPPPEEED
- p6: Browserify & Packaging For Distribution
- p7: Hyrid Client-Server Template Techniques
- p8: Analytics & (airpair.com's) Real-Time "God View"
```

Follow @AirPair to stay up to date and tweet me at @hackerpreneur if you'd like to pair sometime, or one day work with me on AirPair's code base.

## 1 Why is testing MEAN-Stack Hard?

JavaScript man! Before I started AirPair, I'd worked with Backbone.js for about 12 months. But AirPair.com is my firt ever NodeJS app... Everytime someone new says to me "Yeah I bet I can get into testing JS in a couple of weeks" I cringe.

JavaScript is so simple at first glance... then a few days later you realize how f@!#$kin retarted and quirty (inset "WAT" here) this language is all about.

Complexity as an app like AirPair grows is HARD to manage. Users with old accounts... migrations, differnt login systems (you used to only be able to login with google).

## 2 What makes a good test suite?

### 2.1 Readability
 
### 2.2 Speed

Bootstrapping your requires. I'm not talking about a few files, but hundreds.

They say it's best practices to require up the top. 
They say it's best practices not to use globals.

*** But ... ***

Sometimes you need to break some rules. Just don't do it often.
 
### 2.3 TDD vs Coverage
 
Sometimes I do. Mostly I dont.


## 2 MACS-stack: The Serious MEAN-stack Test Stack

**2.0 DISCLAIMER**

1. I'm not the best dev in the world, these are my ideas that I've come up with and I know they could be evolved and polished way beyond what's presented here.

2. This post is only about Server-Side Testing. Truthfully, I've completely 100% neglected testing AirPair's front-end. Maybe soon :).

3. I know there are loads of bits and pieces that could be swapped out... hey we could go as far as replace express probably. This post isn't trying to present the faster and most effecient everything, it's trying trying to strike a balance of maintaining something BIG... in this case my experience with AirPiar, coding it out by myself.

### 2.1 Mocha on Air (MA)

**Mocha you SHOULD know**

This is an advanced post, so I'm not going to call a lot of assumed stuff out. Rather just share some of the newer things I learned over the last few months that made my life easier.

npm test
.only


**Mocha on ES6 and Coffee**

COFFEE!!!! SERIOUSLY WHY OH WHY?

Ok purist, I get it. I honor what you have to say, we can't have an abomination fragmenting the community... But for tests that will not be
used by other people, I'm going to save myself the headaches of finding
closing brackes and braces... when there are SO F#@!kin many in test suites that I would have a constant head ache and dream of the AirPair logo.

**Super Agent**

**MongoDB Helpers**

**Timelapse**



### 2.1 Sinon & Chai (SC)

** SETUP.stubs **

## 3. Identity 

> How do I test scenarios involving multiple uses logging in?

## 4. Data 

### 4.0 Static vs Seed data and helper functions

### 4.1 Static Files

Better to use javascript, as my old app got really slow compiling coffee.

### 4.2 BSON Import

### 4.3 Mongoose vs MongoDB

It wasn't until I dived really deep during iteration two of AirPair that I realized how big of a gap there is between Mongoose and Mongo.

#### 4.4 MongoDB Patterns (with challenge of running against more than one codebase - v0, v1, vExp)

#### Mongoose abstractions and schema behavior

#### Migration Strategies + Nesting schemas + Only point of splitting by collection is for querying and indexing ... (See Mongo Patterns post)

#### Sneaky ObjectId nuances between mongoose vs Model.collection



** What you see is NOT what you get **

Consider this schema

```

```

##  When to run tests (Pre-push) Poor man's CI


##  Patterns

To maintain huge code bases, you need clean beautiful and consistent code. 
It's even hard to devote to this end in a test suite than normal code.

### Stories



