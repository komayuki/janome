=======
Janome
=======

.. image:: https://travis-ci.org/mocobeta/janome.svg?branch=master
    :target: https://travis-ci.org/mocobeta/janome

.. image:: https://coveralls.io/repos/github/mocobeta/janome/badge.svg?branch=master
    :target: https://coveralls.io/github/mocobeta/janome?branch=master

Janome is a Japanese morphological analysis engine written in pure Python.

General documentation:

http://mocobeta.github.io/janome/en/ (English)

http://mocobeta.github.io/janome/ (Japanese)

Requirements
=============

Python 2.7.x or 3.3+ is required.

Install
========

[Note] This consumes about 500 MB memory for building.

.. code:: bash

  (venv) $ python setup.py install

Run
====

.. code:: bash

  (env) $ python
  >>> from janome.tokenizer import Tokenizer
  >>> t = Tokenizer()
  >>> for token in t.tokenize(u'すもももももももものうち'):
  ...     print(token)
  ...
  すもも 名詞,一般,*,*,*,*,すもも,スモモ,スモモ
  も    助詞,係助詞,*,*,*,*,も,モ,モ
  もも  名詞,一般,*,*,*,*,もも,モモ,モモ
  も    助詞,係助詞,*,*,*,*,も,モ,モ
  もも  名詞,一般,*,*,*,*,もも,モモ,モモ
  の    助詞,連体化,*,*,*,*,の,ノ,ノ
  うち  名詞,非自立,副詞可能,*,*,*,うち,ウチ,ウチ

License
========

Licensed under Apache License 2.0 and uses the MeCab-IPADIC dictionary/statistical model.

See LICENSE.txt and NOTICE.txt for license details.

Acknowledgement
================

Special thanks to @ikawaha and @takuya_a.

Copyright
==========

Copyright(C) 2015-2017, moco_beta. All rights reserved.
