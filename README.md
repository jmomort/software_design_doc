# Software Design Documents: Thoughts and Template

Last Updated: Oct 30, 2019

Authors: Adam Fletcher, Jonathan Mortensen

Status: Approved

**The goal of a design document is to provide some
structure around thinking in depth about a complex problem that will be
solved in software before writing that software.**

The goal of a design document is NOT to:
  * Detail a schedule for the creation of software; it’s not the waterfall style specifications document.
  * Be 100% correct. No design doc has ever survived meeting reality, and that’s fine.
  * Be used for simple problems. Use taste to decide if something like this is needed.


Design documents should have:

  * A clear title.
  * A list of the authors, the date the document was created, the status of the document, the names of those reviewing it, and the the time allowed for the review. All names should be individuals, not groups - it’s not okay to say “engineering” as a reviewer, since that means nobody will review it.
  * A summary of the problem, document goal, and proposed solution.
  * The problem
  * Definition
  * Examples
  * Why the problem is important to the business.
    * Cost
    * Priority
    * Magnitude
  * Goal of this design
  * A list of explicit non-goals for this design. It’s
    important to include these to avoid scope creep, especially from
    topics that are goal-adjacent but not actually related to the
    goal.

  * A description of any current solution, including
    architectural diagrams and why this solution isn’t good enough, if
    one is being replaced/altered.

  * Requirements for the solution:
    * Key assumptions
    * These are **measurable** with **specific units.**
    * For example, it is not acceptable to say “The system must be fast”; it is acceptable to say “the system must handle a peak load of 500,000 queries per second with a mean latency of 20ms and 95%tile latency of 35ms when under peak load”.
    * Without measurable goals, this section is not complete and the design doc is not done.
 
    * There should be:
     * Business requirements.
     * Technical requirements.
     * Schedule & resource requirements.
      * Effectively, what’s the budget we have to work with, including capital spend, people, computers, etc.
  * Solutions Considered (or to be considered):
      * This section contains at least three different solutions considered, in some detail.
      * Each solution considered should have details on how the solution does or does not meet the measurable goals from the requirements section.
      * Each solution should be explored in some depth; if possible, measurements of actual solution performance should be here. This isn’t always possible.
      * If there’s an existing system in place that isn’t working for some reason, you must include research into how the existing system could (or could not) be updated to meet the requirements.
  * Solution Chosen:
      * Why?
      * Implementation approach, including:
       * Architecture diagrams.
       * System interaction diagrams (what other existing or new systems will the interact with, and how).
      * General idea about the time and resources equired to implement this, in priority order.
      * Test & validation approach.

  * FAQ/Open Questions


A design doc is best written in a format that allows
extremely fast collaboration and commenting. We recommend Google Docs
for this. We don’t recommend Markdown, as Markdown doesn’t allow for
easy commenting, requires additional rendering tools, and importantly
has no way to easily represent tables. It’s fine to move the doc to a
revision-controlled format and location once the doc has been
approved.

## See [design doc template](template.md) ##

Copyright 2019, Adam Fletcher
