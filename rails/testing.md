# RSpec

## Timecop

[timecop](https://github.com/travisjeffery/timecop)

* When dealing with relative times, i.e. `1.month.ago` or `Time.now + 1.day`, it's possible that part of the code will break when the current day reaches beyond a hard-coded or database-backed date, i.e. sometime in the next year. To avoid this, use relative dates wrapped in a Timecop block.
