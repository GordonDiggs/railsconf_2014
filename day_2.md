# Day 2: April 23

## Keynote - Yehuda Katz

* Cognitive Depletion
* Experimentation merged into shared solutions

## Tricks that Rails didn't tell you about - Carlos Antonio da Silva

* `change_column_null` - change null constraint
* `change_column_default`
* Relation merge: `.joins(:articles).merge(Article.draft)`
* `group(:status, :category).count`
* `where.not status: 'draft'`
* `Item.pluck(:title, :artist)` or `Item.distinct.pluck(:title, :artist)`

```ruby
class Article < ...
  to_param :title
end
```

* `ActiveRecord::Base.benchmark 'description' { Article.foo }`
  * Can use `benchmark` helper in views too
* ActiveModel::Model
  * Lets you use rails helpers with other classes
  * Can validate stuff
* `render(...) || content_tag(...)`
* `local_assigns` in partials instead of always passing variables
* `truncate` takes block ro have read more link
* `config.exceptions_route` to have custom error controller
* `app`, `helper` methods in console
* console helpers
* `rails c --sandbox` - everything gets rolled back
* Updating Rails
  * `rake rails:update`
* Rails talk mailing list
* https://speakerdeck.com/carlosantoniodasilva/tricks-that-rails-didnt-tell-you-about-at-railsconf-2014

## What the cache?! - Simon Kröger

* `:race_condition_ttl` config option
* Cache versioning - store version in cache as well
* bounded_cache gem

## Artisans and Apprentices - Coraline Ehmke

* Values-driven development
  * Don't have to compromise your values to be successful
* Amplify dissent
* Pass down your values

## Building kick-ass internal education programs (for large and small budgets) - Chuck Lauer Vose

* A good educator pushes people out of their comfort zone
* Turn to your neighbor and give a high five
* Lightning talks before lunch
  * People can continue the conversation through lunch
  * Bring food
* Mob refactoring / Code Review
  * Rewrite the code together, then throw it out
* Pair programming methods
  * Sneaky monitor: bring your monitor to their desk
  * Opt-in workshops: send out an invite
* Workshops
  * Choose a theme as a group
* Fishbowl discussions
  * Some people discuss a difficult problem
  * Others can listen
* On-boarding mentors
  * Point person for new hire's first 2-4 weeks
  * Sets aside time to answer all questions
* Ask team to review code - bring snacks

## Technical Onboarding, Training, and Mentoring

## Authorization in a Service-Oriented Environment - Ballroom 1-3
