# RailsCasts Episode #115: Model Caching (revised)

http://railscasts.com/episodes/115-model-caching-revised

Requires Ruby 1.9.2 or higher.


### Commands used in rails console

```
Rails.cache.write('date', Date.today)
Rails.cache.read('date')
Rails.cache.fetch('time') { Time.now }
Rails.cache.class
article = Article.first
article.cache_key
article.touch
Rails.cache.fetch([article, "foo"]) { 123 }
```
