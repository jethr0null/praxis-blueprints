# praxis-blueprints changelog

## next 

## 1.3.0

* Added `include_nil` option to `View` for refining the rendering of nil values. 
  * This can be set when defining the view with `Blueprint.view`, and defaults to false. For example: `view :default, include_nil: true { ... }`.
* Fixed `Blueprint.describe` to output the proper `:id`. That is: the 'id` from the Class name, rather than the internal Struct attribute.
* Fixed `Blueprint.dump(nil)` raising a `NoMethodError`
* Fixed `Blueprint.load(nil)` to properly support the `recurse` option.

## 1.2.0

* `Blueprint` readers now always `load` the value for an attribute before returning it.

## 1.1.0

* Added CollectionView, a special type of view that renders an array of objects with another view.


## 1.0.1

* Relaxed ActiveSupport version dependency (from 4 to >=3)


## 1.0

Initial release!