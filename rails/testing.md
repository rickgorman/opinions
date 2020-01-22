# RSpec

## Timecop

[timecop](https://github.com/travisjeffery/timecop)

* When dealing with relative times, i.e. `1.month.ago` or `Time.now + 1.day`, it's possible that part of the code will break when the current day reaches beyond a hard-coded or database-backed date, i.e. sometime in the next year. To avoid this, use relative dates wrapped in a Timecop block.

# Associations

## block-style invocation

[has_many](https://apidock.com/rails/ActiveRecord/Associations/ClassMethods/has_many)
* You can pass a block into an association. On one hand I love this, because it allows model+association-specific behavior to exist, i.e. a scope that relies on the base model, and on the other hand, I dislike this, because it creates a potential scenario for code duplication, i.e. when a piece of behavior needs to be defined in two different associations in two different models, not to mention tight-coupling between models.
