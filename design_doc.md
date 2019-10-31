# <span dir="ltr">Software Design Documents: Thoughts and Template</span>

<span dir="ltr">Last update: April 8, 2018</span>

*<span dir="ltr">Adam Fletcher, Jonathan Mortensen</span>*

<span dir="ltr"></span>

<span dir="ltr"></span>

**<span dir="ltr">The goal of a design document is to provide some
structure around thinking in depth about a complex problem that will be
solved in software before writing that software.</span>**

<span dir="ltr"></span>

<span dir="ltr">The goal of a design document is NOT to:</span>

  - > <span dir="ltr">Detail a schedule for the creation of software;
    > it’s not the waterfall style specifications document.</span>

  - > <span dir="ltr">Be 100% correct. No design doc has ever survived
    > meeting reality, and that’s fine.</span>

  - > <span dir="ltr">Be used for simple problems. Use taste to decide
    > if something like this is needed.</span>

<span dir="ltr"></span>

<span dir="ltr">Design documents should have:</span>

  - > <span dir="ltr">A clear title.</span>

  - > <span dir="ltr">A list of the authors, the date the document was
    > created, the status of the document, the names of those reviewing
    > it, and the the time allowed for the review. All names should be
    > individuals, not groups - it’s not okay to say “engineering” as a
    > reviewer, since that means nobody will review it.</span>

  - > <span dir="ltr">A summary of the problem, document goal, and
    > proposed solution.</span>

  - > <span dir="ltr">The problem</span>
    
      - > <span dir="ltr">Definition</span>
    
      - > <span dir="ltr">Examples</span>
    
      - > <span dir="ltr">Why the problem is important to the
        > business.</span>
        
          - > <span dir="ltr">Cost</span>
        
          - > <span dir="ltr">Priority</span>
        
          - > <span dir="ltr">Magnitude</span>

  - > <span dir="ltr">Goal of this design</span>

  - > <span dir="ltr">A list of explicit non-goals for this design. It’s
    > important to include these to avoid scope creep, especially from
    > topics that are goal-adjacent but not actually related to the
    > goal.</span>

  - > <span dir="ltr">A description of any current solution, including
    > architectural diagrams and why this solution isn’t good enough, if
    > one is being replaced/altered.</span>

  - > <span dir="ltr">Requirements for the solution:</span>
    
      - > <span dir="ltr">Key assumptions</span>
    
      - > <span dir="ltr">These are **measurable** with **specific
        > units.**</span>
    
      - > <span dir="ltr">For example, it is not acceptable to say “The
        > system must be fast”; it is acceptable to say “the system must
        > handle a peak load of 500,000 queries per second with a mean
        > latency of 20ms and 95%tile latency of 35ms when under peak
        > load”.</span>
    
      - > <span dir="ltr">Without measurable goals, this section is not
        > complete and the design doc is not done.</span>
    
      - > <span dir="ltr">There should be:</span>
        
          - > <span dir="ltr">Business requirements.</span>
        
          - > <span dir="ltr">Technical requirements.</span>
        
          - > <span dir="ltr">Schedule & resource requirements.</span>
            
              - > <span dir="ltr">Effectively, what’s the budget we have
                > to work with, including capital spend, people,
                > computers, etc.</span>

  - > <span dir="ltr">Solutions Considered (or to be considered):</span>
    
      - > <span dir="ltr">This section contains at least three different
        > solutions considered, in some detail.</span>
    
      - > <span dir="ltr">Each solution considered should have details
        > on how the solution does or does not meet the measurable goals
        > from the requirements section.</span>
    
      - > <span dir="ltr">Each solution should be explored in some
        > depth; if possible, measurements of actual solution
        > performance should be here. This isn’t always possible.</span>
    
      - > <span dir="ltr">If there’s an existing system in place that
        > isn’t working for some reason, you must include research into
        > how the existing system could (or could not) be updated to
        > meet the requirements.</span>

  - > <span dir="ltr">Solution Chosen:</span>
    
      - > <span dir="ltr">Why?</span>
    
      - > <span dir="ltr">Implementation approach, including:</span>
        
          - > <span dir="ltr">Architecture diagrams.</span>
        
          - > <span dir="ltr">System interaction diagrams (what other
            > existing or new systems will the interact with, and
            > how).</span>
    
      - > <span dir="ltr">General idea about the time and resources
        > required to implement this, in priority order</span>
    
      - > <span dir="ltr">Test & validation approach.</span>

  - > <span dir="ltr">FAQ/Open Questions</span>

<span dir="ltr"></span>

<span dir="ltr">A design doc is best written in a format that allows
extremely fast collaboration and commenting. We recommend Google Docs
for this. We don’t recommend Markdown, as Markdown doesn’t allow for
easy commenting, requires additional rendering tools, and importantly
has no way to easily represent tables. It’s fine to move the doc to a
revision-controlled format and location once the doc has been
approved.</span>

<span dir="ltr"></span>

<span dir="ltr">A design doc template is available after the page
break.</span>

<span dir="ltr"></span>

<span dir="ltr"></span>

<span dir="ltr"></span>

<span dir="ltr">Name: A System for Foo</span>

<span dir="ltr"></span>

**<span dir="ltr">Date:</span>**

**<span dir="ltr">Authors:</span>**

**<span dir="ltr">Status: \<draft, in review, approved\></span>**

**<span dir="ltr">Reviewers:</span>**

**<span dir="ltr">Review done by date:</span>**

<span dir="ltr"></span>

# <span dir="ltr">Summary</span>

# <span dir="ltr">Problem</span>

## <span dir="ltr">Definition</span>

## <span dir="ltr">Examples</span>

## <span dir="ltr">Why the problem is important to the business?</span>

### <span dir="ltr">Cost</span>

### <span dir="ltr">Priority</span>

### <span dir="ltr">Magnitude</span>

# <span dir="ltr">Goal \[of *this* document\]</span>

## <span dir="ltr">Explicit non-goals</span>

# <span dir="ltr">Solution Requirements</span>

### <span dir="ltr">Business requirements</span> 

### <span dir="ltr">Technical requirements</span>

### <span dir="ltr">Schedule & resource requirements</span>

# <span dir="ltr">Current Solution</span>

### <span dir="ltr">Degree Current Solution meets stated requirements</span>

# <span dir="ltr">Solutions Considered</span> 

### <span dir="ltr">Solution 1: Foo</span>

### <span dir="ltr">Solution 2: Bar</span>

### <span dir="ltr">Solution 3: Baz</span>

# <span dir="ltr">Solution Chosen</span>

## <span dir="ltr">Test & Validation Approach</span>

# <span dir="ltr">Appendix</span>

## <span dir="ltr">Supporting Data</span>

## <span dir="ltr">Supporting Documents</span>

<span dir="ltr"></span>

<span dir="ltr"></span>

<span dir="ltr"></span>
