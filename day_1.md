# Day 1: April 22

## Keynote: David Heinemeier Hansson

* Code/poetry similarity
* TDD: most successful software diet
* James Coplien "Why Most Unit Testing is Waste"

## Ultra Light and Maintainable Rails Wizards - Sean Marcia

* Computers should be better than paper
* Highest goal is ease of use for user
* Wizard == Builder Design Pattern
* Each step gets a presenter
  * Runs its validations
* Step 1 is #create of Model - every other is #edit of ModelPart
* Each step inherits from Model
* Wicked gem

## Rack::Attack: Protect your app with this one weird gem! - Aaron Suggs

*@ktheory*

* *github.com/kickstarter/rack-attack*
* Blocking & throttling middleware
* kicksniper.py
* `obj.presence`
* Restrict trolls to GET requests
  * Support team bans IPs
  * They also deploy the yaml update
* Code, easyness, notifications better than nginx
* Integration testable

## Lightning Fast Deployment of Your Rails-backed JavaScript app - Luke Melia

* `heroku labs:enable preboot`
  * Switches to new code after 3 minutes
* Make both old versions and new versions available for a few minutes after a deploy
  * Prevents asset 404s
* Deploy js and css to non-app code servers
* Deploy html to redis server, serve from there through rails controllers
  * Get manifest hash
  * Preview any manifest
  * Can also AB test
* Deploying to s3
  * Keep manifest file, only deploy what is different
* Gives you flexibility with how to build JS
* split gem: AB test tool

## Real-time Rails with Sync - Mike Moore

* *github.com/chrismccord/sync*

## Mutation Testing with Mutant - Erik Michaels-Ober

* *github.com/mbj/mutant*
* Computer History Museum, Mountain View CA
* Mutation Testing: changes code at runtime
  * Tests should fail with mutation
* `bundle exec mutant ...`

## Keynote: Farrah Bostic

* "I didn't Build That"
