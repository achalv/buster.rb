![buster.rb](http://i.imgur.com/WmfSP9S.png?2) buster.rb
=========

## **About**

Buster is a cachebuster plugin for the Jekyll static site generator which works with the Liquid templating engine.

Every time you run `jekyll serve` or `jekyll build`, buster will append a new hash to the end of all your static assets - scripts, stylesheets, images - whatever you want. This tricks the browser into thinking that you're loading an entirely new resource, and so it doesn't just load the asset from your cache – it'll fetch it like it's new.

## **Usage**

Add buster.rb to the `_plugins/` folder in your Jekyll site. Then, in your code, you can use the liquid tag `{% buster %}` wherever you want buster to add a hash.

## **Example**

Using {% buster %} with app.js like such...
```
<script src="/js/app.js{% buster %}"></script>
```
would give us this result when Jekyll generates our markup –
```
<script src="/js/app.js?dfc274b88222920b4d89006fde43c19f"></script>
```
***That's it!***

## **Need help?**

Please open an issue if you have any problems with buster. 

[**License - MIT**](https://github.com/achalv/buster.rb/blob/master/LICENSE)

> Dog designed by <a href="http://www.thenounproject.com/ilikemetomuch">Philip Glenn</a> from the <a href="http://www.thenounproject.com">Noun Project</a>
