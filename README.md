# Luvotels - Full-stack hiring test

## Foreword

Hi, this is the tech team at Luvotels, welcome to our Full-stack practical test!

You should have gotten here during our hiring process but if you got there *by chance* and you find the idea fun please send us an email at hello@luvotels.com!

The idea here is to use the same test case for any level (apprentice/junior/mid/senior) but judge it according to your level. So don't be afraid if you're an apprentice or a junior, just do your best!

## How-to

1. Create a fork of this project
2. Do your thing
3. Use the README.md file to explain what you did
4. Send us an email to hello@luvotels.com when you have finished!

Number 3 is **really important**, there are plenty of ways of solving this challenge and we want to understand why you chose to do it like that.
Imagine you have to explain to:
* our real hotel clients why your solution is good
* our tech team why your code is organized like that

We advise you document your choices as you go because it's easy to forget!

The README should also contain any specific information on how to run the project.

And, last but not least, some todo/critics/comments/leads on your code is highly welcome. We do not believe in a quest to write perfect code but believe we need to always improve. So that's okay if your code is not perfect as long as you are aware of the flaws and can explain them :wink:

There is no time limit although we generally leave 1 week to complete the test (because that's what happens in real life) and you should have a working solution in about 12/16 hours.

### Help?!

If you have any question you can:
* Browse the issues https://github.com/luvotels/fs-hiring-test/issues and/or create one
* Send an email to hello@luvotels.com

## The challenge

You will build a bookings report page for the motels owners.

The real case scenario : each motel owner has a private access to a special area to administrate their data. They need to be able to quickly access the bookings that were made through the platform and their revenue share.

You **don't** have to build any admin area but you should be able to login different users (ie, motel owners) and show only their own reports.
Additional information about users and motels can be found in issue #1

### The data

We have put online a simple API. Here's the doc.

#### https://luvotels-hiring-api.herokuapp.com/motels.json

Will return the list of motels in our system, for every motel you'll get:
```json
{
  "id": 42,
  "name": "The motel name",
  "logo": "http://something.xxx/logo.jpg"
}
```

#### https://luvotels-hiring-api.herokuapp.com/motels/:motel_id:/rooms.json

Will return the list of rooms for the specified motel, for every room you'll get:
```json
{
  "id": 42,
  "motel_id": 42,
  "name": "Best room ever",
  "picture": "http://something.xxx/picture.jpg"
}
```

#### https://luvotels-hiring-api.herokuapp.com/motels/:motel_id:/bookings.json

Will return the list of bookings for the specified motel, for every booking you'll get:

```javascript
{
  "id": 42,
  "motel_id": 42,
  "room_id": 42,
  "amount_centavos": 9900, // how much the client paid in cents
  "fee_percentage": 12, // the part that goes to Luvotels in percents
  "booking_period": "2 hours - Week",
  "created_at": "2017-12-05T18:43:09.528Z",
  "paid_at": "2017-12-05T18:53:09.528Z",
  "booking_code": "XOPFJW" // unique code the client present to the reception
}
```

### What we are expecting

* The project to be done using Rails
* Clean code (whether it's ruby/js/css/html)
* Using Twitter boostrap
* Mobile first (and of course, responsive)
* Having the project run on Heroku

#### What would be great

* Tests!
* Using a different templating syntax (we use slim)

#### What would be amazing

* A layer between our API and your page so you don't overcharge the API.

#### What we do NOT want

* Discover you did not do the test by yourself
* See ugly commits

### What we will look at

* your commit history
* your README
* your code quality, its structure and how you implemented your design choices
* if the provided solution... resolves the problem!
* how it looks on mobile and on desktop

Hope you have fun, any doubts please feel free to contact us hello@luvotels.com

## Thanks

The structure of this README is greatly inspired by the Frontend challenge of Intellipost. GG! https://github.com/intelipost/job-frontend-developer
