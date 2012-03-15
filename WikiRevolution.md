Wiki Revolution
================================================================================

tl;dr
--------------------------------------------------------------------------------
Google Sites sucks; let's switch to a GitHub wiki pronto.


Declaration of Indisposition
--------------------------------------------------------------------------------
When in the course of software development it becomes necessary for one team to
dissolve the bit-rotted links that have connected them with a deficient
documentation system and to assume among the powers of organization the
capability to reasonably manage their critical information infrastructure, a
decent respect to the opinions of managers and colleagues requires that they
should declare the causes which impel them to the separation.

We hold these truths to be self-evident, that documentation is at least equal
in importance to code, that it is required in order for them to remain useful
that certain essential characteristics inhere in those docs, that among these
are easy emendation, decent version control, and the use of one's preferred
editor. That to secure these characteristics, tools are continually invented
and reinvented among programmers for their mutual benefit. But when inept,
unwieldy, poorly-designed tools result in otherwise stalwart programmers
invariably muddling through the exact same problems their peers just did not
too long ago, it is their right, it is their duty, to throw off such hacky
kludges, and to provide new tools to secure their collective knowledge. Such
has been the patient sufferance of this team; and such is now the necessity
which constrains them to alter their former systems of documentation
management. The history of the present Google Sites is a history of repeated
injuries and usurpations, all having in indirect consequence great frustrations
and impediments to efficiency, taxed morale, and many a late-night
troubleshooting session ill-informed by anecdotal misremembrances. To prove
this, let Facts be submitted as a pull request to a candid repository.


Arguments Against Google Sites
--------------------------------------------------------------------------------

When the tools used to maintain documentation create friction above and beyond
the already difficult task of writing documentation in the first place, the
documentation so maintained tends to stagnate and fall into disuse. Google
Sites is a clumsy, half-baked, neglected stepchild of a webapp that discourages
the making of substantial revisions, hampers culling and reorganizing entries,
and dampens even the most enthusiastic intentions of keeping content
up-to-date.

*   Editing Google Sites pages in a web browser is tedious, slow, and error
    prone. Doing anything more complicated than writing unadorned blocks of
    text requires editing raw html in order to get acceptable results.

*   Futhermore, Google Site's use of html as the base document format is a gross
    violation of the fundamental principles of encapsulation and separation of
    data from presentation that we hold dear as responsible software designers. And
    this violation is especially grievous when the tools provided for WYSIWIG editing
    generate beneath the rendered façade an increasingly mangled mess of tag soup
    that makes subsequent revision ever more onerous.

*   Google Sites version history is awkward, unwieldy, inefficient, unclear,
    and inaccessible to existing diff tools.

*   Creating and maintaining links between pages is laborious, painstaking work.

*   Essentially, Google Sites is not a even a genuine wiki, missing some of the
    most essential features of a wiki: fast, easy, simple shared editing; pages
    created and linked automatically with WikiWords alone.

*   Google can change and has changed the interface without warning or any
    means of appeal.

*   All external links are wrapped in a Google redirection URL.

*   Do I really need to make this case? Have you used it?

    ____

    __Google Sites Counterpoint__

*   We do already have a fair amount of documentation in Google Sites. Moving it
    to another system would take time and effort (though we would likely wind
    up cleaning it up and improving it significantly in the process).

*   Google Sites pages are more widely available to everyone in the company,
    rather than only those with a GitHub account.

*   Google Sites does have an API and sample code libraries with which we could
    possibly cobble together something more usable. (Of course `API + libraries !=
    working application`. And arguably, the best use of these APIs might be to mirror
    select GitHub wiki pages on Google Sites.)


Arguments In Favor of GitHub Wiki
--------------------------------------------------------------------------------

Our documentation is arguably as important as our code. We should treat it that
way. We should each be able to use the tools we are already most familiar and
comfortable with&mdash;and which are much better suited to the task&mdash;to
edit our documentation as well. A GitHub wiki makes this very easy.

*   Using GitHub for documentation further consolidates our work management
    toolset. We are already using GitHub for our code and code reviews.

*   Yet it also leverages the flexibility and breadth of all of the great
    features of a text-based distributed version control system by virtue of
    its git underpinnings, including:

    * Contents accessible with the entire arsenal of tools already at our
      fingertips for editing, search, and replace.

    * Great diffing, version history, merging, branching, and confict
      resolution facilities.

    * Much less chance of mistaken deletions or undetected edits.

    * Offline access.

*   Nearly all of the tools that drive the wiki engine are open source
    projects that accept and even encourage contributions via pull requests.

*   Multiple markup formats are available, and can even be mixed and matched,
    if so desired.

*   We could script updates to documentation in a clean, controlled way to
    keep it in sync with our related code changes automatically.

    ____

    __GitHub Wiki Counterpoint__

*   Access is limited to those with GitHub accounts in our organization, with
    access rights to the documentation repository. But switching development
    documentation to GitHub is not mutually exclusive of keeping select documents
    in Google Sites. It's no more difficult to link between GitHub wiki pages and a
    Google Sites pages than it is between Google Sites pages.

*   What other drawbacks? Help me out here.
