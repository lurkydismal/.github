Contributing to this repository
===============================

_tl;dr: be [courteous](https://github.com/lurkydismal/.github/tree/main/CODE_OF_CONDUCT.md), follow the steps below to set up a development environment._


Welcome
-------

There are many ways to contribute, including writing code, filing issues on GitHub,
helping to triage, reproduce, or fix bugs that people have filed, adding to documentation,
doing outreach about this repository, or helping out in any other way.

I communicate primarily over GitHub.

Before you get started, I encourage you to read these documents which describe some of the norms:

1. [My code of conduct](https://github.com/lurkydismal/.github/tree/main/CODE_OF_CONDUCT.md), which stipulates explicitly
   that everyone must be gracious, respectful, and professional. This
   also documents my conflict resolution policy and encourages people
   to ask questions.

<!-- TODO: Add values -->
2. [Values](VALUES), which talks about what I care most about.


Helping out in the issue database
---------------------------------

Triage is the process of going through bug reports and determining if they are valid, finding out
how to reproduce them, catching duplicate reports, and generally making issues list
useful for me.

If you want to help us triage, you are very welcome to do so!

1. Read [my code of conduct](CODE_OF_CONDUCT.md), which stipulates explicitly
   that everyone must be respectful, and professional. If you're helping out
   with triage and you want to make sure to make a good impression!

2. Start by trying to reproduce the problem and asking for people to
   provide enough details that you can reproduce the problem, pointing out duplicates,
   and so on.

<!-- TODO: Add issue hygiene -->
3. Familiarize yourself with my [issue hygiene](Issue-hygiene), which covers
   the meanings of some important GitHub labels and milestones.


Quality Assurance
-----------------

One of the most useful tasks, closely related to triage, is finding and filing bug reports. Testing
beta releases, looking for regressions, creating test cases, adding to test suites, and
other work along these lines can really drive the quality of the product up. Creating tests
that increase test coverage, writing tests for issues others have filed, all these tasks
are really valuable contributions to open source projects.

If this interests you, you can jump in and submit bug reports without needing anyone's permission!
I am especially eager for QA testing when I announce a beta release.

If you want to contribute test cases, you can also submit PRs. See the next section
for how to set up your development environment.


Developing for this repository
------------------------------

If you would prefer to write code, you may wish to start with **good first contribution** issues.

To develop for this repository, you will eventually need to become familiar
with my processes and conventions. This section lists the documents
that describe these methodologies. The following list is ordered: you
are strongly recommended to go through these documents in the order
presented.

<!-- TODO: Add issue hygiene -->
1. [Setting up your app development environment](SETTING_UP_DEVELOPMENT).
   This project mainly uses latest C++ with GNU extensions.

<!-- TODO: Add tree hygiene -->
2. [Tree hygiene](TREE_HYGIENE), which covers how to land a PR, how to do code review, how to
   handle breaking changes, how to handle regressions, and how to
   handle post-commit test failures.

<!-- TODO: Add style guide -->
3. [My style guide](STYLE_GUIDE), which includes advice for designing APIs for this repository,
   and how to format code.

<!-- TODO: Add template -->
<!-- TODO: Add design documents -->
4. [Design document template](TEMPLATE), which should be used when proposing a new technical design.
   This is a good practice to do before coding more intricate changes.
   See also my [guidance for writing design docs](DESIGN_DOCUMENTS).


API documentation
-----------------

Another great area to contribute in is sample code and API documentation. As API docs are integrated into source code, see the
"developing for this repository" section above for a guide on how to set up your developer environment.

<!-- TODO: Add style guide -->
To contribute API documentation, an excellent command of the English language is particularly helpful, as is a careful attention to detail.
I have a [whole section in my style guide](STYLE_GUIDE#documentation-docs) that you should read before you write API documentation.
It includes notes on wording and grammar conventions.

In general, a really productive way to improve documentation is to use this repository and stop any time your have a question: find the answer, then
document the answer where you first looked for it.

I also keep a list of areas that need better API documentation with TODOs.
In many cases, I have written down what needs to be said in the relevant issue, I just haven't gotten around to doing it!

I am especially eager to add sample code and diagrams to my API documentation. It can be a lot of fun to create new diagrams for the API docs.


Releases
--------

If you are interested in participating in my release process, which may involve writing release notes and blog posts,
updating release tooling, and other work of that nature, then please contact [lurkydismal@duck.com](mailto:lurkydismal@duck.com).
