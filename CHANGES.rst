Changelog
=========

4.0.2 (2017-06-11)
------------------

- Mark as compatible with Python 2 and 3.

4.0.1 (2016-08-30)
------------------

- Fix version number of ZCatalog requirement to be PEP compliant.

4.0 (2016-08-28)
----------------

- Move code into ZCatalog distribution.

- Implement new `IQueryIndex` interface.

- Require at least Zope and ZCatalog 4.0.

3.0 (2016-07-18)
----------------

- Replace stopper and okascore C implementations with pure-Python.

- Remove HelpSys pages.

- Remove various internal test helper modules.

- Remove old-style interface modules, use the interfaces module instead.

- Update to ZODB 4.x as direct dependency. Which drops ZODB3 support.

2.13.5 (2014-02-19)
-------------------

- Add `getIndexQueryNames` method to index to comply with extended interface.

2.13.4 (2012-12-03)
-------------------

- Fixed problem where the index was not reindexed if the new value was an empty
  string leading to inconsistence between the object attribute (that is empty)
  and the index that still contains the old indexed value.

2.13.3 (2011-07-28)
-------------------

- Fixed problem in reindex document optimization, which could lead to negative
  document counts when reindexing unchanged documents.

2.13.2 (2011-05-04)
-------------------

- Avoid changing data, if the indexed values stayed the same.

2.13.1 (2010-10-02)
-------------------

- Changed word id creation algorithm in Lexicon. Instead of relying on an
  increasing length counter, we use a number from a randomized range. This
  avoids conflict errors while adding new words in multiple parallel
  transactions. Inspired by code from ``enfold.fixes``.

- Lexicon: Added clear method.

- Lexicon: Removed BBB code for instances created with Zope < 2.6.2.

- Added missing namespace_packages declaration to setup.py.

2.13.0 (2010-06-19)
-------------------

- Released as separate package.
