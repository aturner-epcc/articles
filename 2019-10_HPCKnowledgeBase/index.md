# UK public HPC knowledge base

*Andy Turner, EPCC, The University of Edinburgh*

In this blog post I consider how we (as the UK HPC community) could go about creating a 
community HPC knowledge base that would allow us to share and reuse useful technical 
information. Much of these thoughts came out of discussions at the HPC Champions meeting
that took place on 16 September 2019 alongside the UK RSE Conference in Birmingham, UK.

## Motivation

The UK HPC landscape has changed a lot over the past 5 years with the introduction of the EPSRC
national Tier-2 HPC facilities to supplement the national supercomputing service, ARCHER, and
the DiRAC national HPC service. A lot of work has gone on to increase information and experience
sharing between the different national HPC services and to institutional HPC services with a large
amount of success. There are groups that successfully join together HPC systems technical staff, RSEs that 
support users and service management across the UK.

One question that has been raised within the current community meetings is: how can we share 
technical solutions and information that we have locally across the community and potentially
publicly to the wider HPC community (including users, RSEs and service providers)? Many services
and sites have internal knowledge bases (both private and public) that contain information that
would be useful across the community and one option would be to find a way to create a public
knowledge base that could be used by the community to expose this useful information.

## Current situation

Currently, the useful information is stored in a number of different locations with different
access:

   - Internal knowledge bases, wikis and service desks. These systems do not allow public access to 
     the information and sometimes are even difficult to use internally to query information.
   - Public repositories and wikis. A number of different sites provide public repositories and wikis that cover
     particular technical aspects, such as compilation and installation instructions for different
     research software. Although useful, the information is fragmented and often difficult to
     find without knowing where it is.

There is actually a large amount of information already publicly available, for example:

   - Compilation instructions for different HPC systems: [https://github.com/hpc-uk/build-instructions](https://github.com/hpc-uk/build-instructions)
   - Isambard GW4 Arm benchmarks (including compilation instructions): [https://github.com/UoB-HPC/benchmarks](https://github.com/UoB-HPC/benchmarks)
   - UCL build scripts: [https://github.com/UCL-RITS/rcps-buildscripts](https://github.com/UCL-RITS/rcps-buildscripts)
   - UK HPC benchmarks: [https://github.com/hpc-uk/archer-benchmarks](https://github.com/hpc-uk/archer-benchmarks0

## Requirements

What would the requirements for a public UK HPC knowledge base look like? Based on discussions 
at the HPC Champions meeting it should be:

   - Publicly visible through a web browser: available for anyone to view the information and 
     make use of it
   - Searchable and well-indexed: the most powerful search tools are internet search engines. The
     knowledge base should be well indexed and available to be found easily through standard
     search engines.
   - Permissions allow public addition of knowledge base entries: so all can contribute. This,
     however, means that we need a way to...
   - Rate answers based on correctness: to ensure that entries are kept up to date and that
     publicly-added entries are reviewed.
   - A single service/location to avoid the issues of fragmentation of information.

The solution chosen should also likely be free as there is currently no funding stream to support this
activity!

## Potential solutions

From the discussion at HPC Champions and more recently at the RSE HPC monthly open meetings, two initial
services that could provide potential solutions for a shared, open knowledge base have been identified:

   - Stack Overflow and related Stack Exchange sites
   - ask.cyberinfrastructure
   - Others?

### Stack Overflow and related Stack Exchange sites

[Stack Overflow](http://stackoverflow.com) is an public, online knowledge base aimed at sharing technical
knowledge relevant to programming. The site uses peer review of answers to determine the most useful and
accurate answers and allows tagging of questions. The overarching [Stack Exchange](https://stackexchange.com/)
organisation provides the platform for Stack Overflow and also a number of other, less well-known, community
knowledge bases. One that is relevent for the discussion here is the [Computational Science Stack Exchange](https://scicomp.stackexchange.com/) site. The boundary between which questions would fit best on Stack Overflow
and which would fit best on CompSci Stack Exchange is a bit fuzzy but the
[CompSci topic definition](https://scicomp.stackexchange.com/help/on-topic) helps with the distinction boilings
down to programming questions go on Stack Overflow; e.g. How do I compile a code? How do I use MPI function X?,
and high-level questions about packages go on CompSci; e.g. Which is the best LAPACK funtion to do X? Should I use
the single-precision or double-precision version of GROMACS for modelling system Y?.

On all Stack Exchange sites it is perfectly acceptable to ask a question **and** provide an answer. This can 
be useful when transferring knowledge from an internal resource (e.g. a service desk ticket) into the 
public knowledge base.

The strengths of Stack Overflow (and related sites) include its high ranking in technical question searches
using standard search engines, its well designed interface, it has a strong definition of allowed questions
and their format and the fact that it is already the top resource for
this type of technical information on the internet. Stack Overflow also provides an API that would allow
integration with other tools. Disadvantages are that it is debatable how many HPC experts are currently 
engaged in the Stack Overflow communities so it is unclear on the value of the peer review function (at
least initially). Also, questions that are a matter of opinion or discussion are disallowed; e.g. Should 
is use C++ or Fortran for my next HPC coding project?, though this can also be cast as a strength in the 
context of a technical knowledge base as such questions usually lead to open-ended discussion which is not
useful for answering the original question.

### ask.cyberinfrastructure (Ask.CI)

The [Ask.CI](https://ask.cyberinfrastructure.org/) site was created in the US as:

> a centralized, searchable, archived site to aggregate expert knowledge that is widely distributed throughout
> the research computing community. It is a joint project of the [Northeast Cyberteam](https://necyberteam.org/)
> and the [Campus Champions](https://www.xsede.org/community-engagement/campus-champions), it was launched in
> July, 2018 at PEARC18.

The site provides a Q&A interface aimed at all people involved in research computing (e.g. researchers, users,
support staff, RSEs, systems administrators). Like the Stack Exchange sites, Ask.CI is free to use and publicly
available, allows for tagging of questions by topic and allows people to ask a question and answer it themselves.
Unlike Stack Exchange sites, it allows discussion-style questions and allows topics from across the whole range
of research computing - all of the example questions discussed in the Stack Exchange section above would be 
acceptable questions on Ask.CI. It does not have a peer review functionality to allow for rating of answers,
people can simply *like* posts that they think have merit.

The strengths of Ask.CI are that it is focussed particularly on research computing (though this is broader than
just HPC), it already has a dedicated, committed community asking and answering questions and that it allows all
types of questions. Weaknesses are the lack of peer review, the limited community involved and the lack of specific
question guidelines that mean that many of the questions descend into discussion with no indication of what the
*accepted* answer is.

## Next steps

   - Testing Stack Overflow
   - Examining ask.cyberinfrastructure (who is involved? what are activity levels like? quality of answers? user focussed or not?)
   
## Summary

   - Interesting opportunity
