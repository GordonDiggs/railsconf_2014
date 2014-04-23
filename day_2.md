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

## Technical Onboarding, Training, and Mentoring - Kate Heddleston

* Confidence affects how well people perform
* Let new devs learn and play in your environment
* Set boundaries and then move them out as they progress
* Onboarding Categories
  1. Technical Knowldege
  2. Company Knowledge & Process
  3. Personal Development

#### Sample Plan

* Week 1
  * Dev Env Setup
    * Use the last person who started at the company
    * Have a timing goal
  * Shipping
    * Start small (like a config file)
  * Journaling
    * Give a central place to talk about what they're learning
    * Helps alleviate confusions
  * Social Event
* Week 2
  * History of company
    * Who are the founders, who was hired a long time ago
    * Team map: pictures and names
  * Code Labs / Shadowing
    * Code lab: talk to someone about code, answer any questions
    * Shadowing: watch someone work for a specific amount of time
* Week 3
  * 1 on 1s
    * Solicit feedback, ask about what they learned
  * Goal setting
    * What do they want to do next?
  * Give feeback early and often
  * Presentations
* Week 4
  * Review Concepts
  * 1 on 1s
  * Elective Shadowing
  * Co-piloting a larger project
* github.com/heddle317/onboarding

## Authorization in a Service-Oriented Environment - Alan Cohen

* Application code is loosely coupled to authorization
* IronHide gem
