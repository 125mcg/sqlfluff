.. _vision:

Vision for SQLfluff
===================

SQLfluff has a few components:

1. A generic parser for SQL which aims to be able to unify SQL written
   in different dialects into a comparable format. The *parser*.
2. A mechanism for measuring written SQL against a set of rules, with
   the added ability to fix any violations found. The *linter*.
3. An opinionated set of guidelines for how SQL should be structured
   and formatted. The *rules*.

The core vision [#f1]_ for sqlfluff is to be really good at being the *linter*.
The reasoning for this is outlined in :ref:`realworldref`.

Most of the codebase for SQlfluff is the *parser*, mostly because at
the point of developing SQLfluff, there didn't appear to be a good
option for a whitespace-aware parser that could be used instead.

With regards to the *rules*, SQLfluff aims to be opinionated but it
also accepts that many organisations and groups have pre-existing
strong conventions around how to write SQL and so ultimately SQLfluff
should be flexible enough to support whichever rule set a user wishes
to.

.. rubric:: Notes

.. [#f1] Credit to `this article`_ for highlighting the importance of a
   good vision.

.. _`this article`: https://opensource.com/business/16/6/bad-practice-foss-projects-management
