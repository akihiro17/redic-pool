1.0.1 - 2015-04-06
==================

* Fixed a critical issue that prevented `Redic::Pool` objects from being used
  across Ohm models. See https://github.com/soveran/ohm/issues/184.

1.0.0 - 2013-12-27
==================

* Changed API to make a `Redic::Pool` object interchangeable with `Redic`. This
  makes `Redic::Pool` compatible with Ohm out of the box, so you can do:

        Ohm.redis = Redic::Pool.new(ENV["REDIS_URL"], size: 10)

0.1.0 - 2013-12-18
==================

* First release.
