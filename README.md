## doctrine/orm v2.8.1 fork with manyToOne associations support in Embeddable

Surprisingly I found out that doctrine [doesn't](https://github.com/doctrine/orm/issues/4291)
[support](https://github.com/doctrine/orm/issues/4747) [relations](https://github.com/doctrine/orm/issues/4546)
in embeddable and [silently ignores them](https://github.com/doctrine/orm/pull/5809).
This fork adds support of manyToOne associations and is based on the following PRs: https://github.com/doctrine/orm/pull/1502 https://github.com/doctrine/orm/pull/5962

Add this to your project's root composer.json:
```
{
    "repositories": [
        {
            "type": "git",
            "url": "git@github.com:karser/doctrine-orm.git"
        }
    ],
    "require": {
        "doctrine/orm": "dev-embeddable-relations-2.8 as 2.8.1",
    }
}
```


Doctrine 2 is an object-relational mapper (ORM) for PHP 7.1+ that provides transparent persistence
for PHP objects. It sits on top of a powerful database abstraction layer (DBAL). One of its key features
is the option to write database queries in a proprietary object oriented SQL dialect called Doctrine Query Language (DQL),
inspired by Hibernate's HQL. This provides developers with a powerful alternative to SQL that maintains flexibility
without requiring unnecessary code duplication.


## More resources:

* [Website](http://www.doctrine-project.org)
* [Documentation](https://www.doctrine-project.org/projects/doctrine-orm/en/latest/index.html)


  [Master image]: https://img.shields.io/travis/doctrine/orm/master.svg?style=flat-square
  [Master]: https://travis-ci.org/doctrine/orm
  [Master coverage image]: https://codecov.io/gh/doctrine/orm/branch/master/graph/badge.svg
  [Master coverage]: https://codecov.io/gh/doctrine/orm/branch/master
  [2.8 image]: https://img.shields.io/travis/doctrine/orm/2.8.svg?style=flat-square
  [2.8]: https://github.com/doctrine/orm/tree/2.8
  [2.8 coverage image]: https://codecov.io/gh/doctrine/orm/branch/2.8/graph/badge.svg
  [2.8 coverage]: https://codecov.io/gh/doctrine/orm/branch/2.8
