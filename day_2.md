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

## What the cache?! - Simon Kröger

## Artisans and Apprentices

## Building kick-ass internal education programs (for large and small budgets)

## Technical Onboarding, Training, and Mentoring

## Authorization in a Service-Oriented Environment - Ballroom 1-3
