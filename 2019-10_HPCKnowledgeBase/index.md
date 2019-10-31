# UK public HPC knowledge base

*Andy Turner, EPCC, The University of Edinburgh*

In this blog post I consider how we (as the UK HPC community) could go about creating a 
community HPC technical knowledge base that would allow us to share and reuse useful technical 
information. Much of these thoughts came out of discussions at the
[HPC Champions meeting](https://rseconuk2019.sched.com/event/RxMV/hpc-champions-workshop-colocated-with-rseconuk2019)
that took place on 16 September 2019 alongside the [UK RSE Conference 2019](https://rse.ac.uk/conf2019/) in Birmingham, UK along
with subsequent discussions at the [monthly HPC RSE calls](http://www.hpc-uk.ac.uk/rse/rse_network.html).

## Motivation

The UK HPC landscape has changed a lot over the past 5 years with the introduction of the EPSRC
national Tier-2 HPC facilities to supplement the national supercomputing service, ARCHER, and
the DiRAC national HPC service. A lot of work has been going on to increase information and experience
sharing between the different national HPC services and to institutional HPC services with a large
amount of success. There are groups that successfully join together HPC systems technical staff, RSEs that 
support users and service management across the UK.

One question that has been raised within the current community meetings is: **How can we share 
technical solutions and information that we have locally across the community and potentially
publicly to the wider HPC community (including users, RSEs and service providers)?** Many services
and sites have internal knowledge bases (both private and public) that contain information that
would be useful across the community and one option would be to find a way to create a public
knowledge base that could be used by the community to expose this useful information.

## Current situation

Currently, the useful information is stored in a number of different locations with different
access:

   - *Internal knowledge bases, wikis and service desks.* These systems do not allow public access to 
     the information and sometimes are even difficult to use internally to query information.
   - *Public repositories, websites and wikis.* A number of different sites provide public repositories,
     websites and wikis that cover particular technical aspects, such as compilation and installation
     instructions for different research software. Although useful, the information is fragmented and
     often difficult to find without knowing where it is.

There is actually a large amount of information already publicly available, for example:

   - Compilation instructions for different HPC systems: [https://github.com/hpc-uk/build-instructions](https://github.com/hpc-uk/build-instructions)
   - Isambard GW4 Arm benchmarks (including compilation instructions): [https://github.com/UoB-HPC/benchmarks](https://github.com/UoB-HPC/benchmarks)
   - UCL build scripts: [https://github.com/UCL-RITS/rcps-buildscripts](https://github.com/UCL-RITS/rcps-buildscripts)
   - UK HPC benchmarks: [https://github.com/hpc-uk/archer-benchmarks](https://github.com/hpc-uk/archer-benchmarks)

and, I am sure, many others that I do not know about (which is one of the reasons we are having this
discussion!).
   
## Requirements

What would the requirements for a public UK HPC knowledge base look like? Based on discussions 
within the community, it should be:

   - **Publicly visible through a web browser:** available for anyone to view the information and 
     make use of it.
   - **Searchable and well-indexed:** the most powerful search tools are internet search engines. The
     knowledge base should be well indexed and available to be found easily through standard
     search engines.
   - **Permissions allow public addition of knowledge base entries:** so all can contribute. This,
     however, means that we need a way to...
   - **Rate answers based on correctness:** to ensure that entries are kept up to date and that
     publicly-added entries are reviewed.

The solution chosen should also likely be free as there is currently no funding stream to support this
activity!

## Potential solutions

From the discussion at HPC Champions and more recently at the RSE HPC monthly open meetings, two initial
services that could provide potential solutions for a shared, open knowledge base have been identified:

   - Stack Overflow and related Stack Exchange sites
   - ask.cyberinfrastructure
   
We have look at two options above in more detail but there must be others out there - please comment and share with your 
own suggestions!

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

Some examples of where this has already been used for questions in this area are:

   - https://stackoverflow.com/questions/58396548/mpi-send-and-receive-after-task-is-completed-is-it-even-possible
   - https://stackoverflow.com/questions/48545264/how-can-i-compile-castep-18-1-on-cray-xc30
   - https://stackoverflow.com/questions/33249907/h5py-installation-via-setup-py-undefined-symbol-iso-c-binding
   
Note the focussed nature of the questions that leads to specific technical answers.

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
types of questions. Weaknesses are the low weight leading to answers being low in search engine rankings, lack
of peer review, the limited community involved and the lack of specific question guidelines that mean that many
of the questions descend into discussion with no indication of what the *accepted* answer is.

Examples of technical questions asked on Ask.CI:

  - https://ask.cyberinfrastructure.org/t/why-is-docker-not-widely-used-in-multi-user-cluster-environments/205/2
  - https://ask.cyberinfrastructure.org/t/how-do-i-run-mpi4py/943
  
As you can see, compared to Stack Overflow, the questions are vague and muh more open-ended and do not lend
themselves as well to a technical knowledge base.

## What next?

Based on the analysis above, my personal opinion is that using the Stack Exchange sites, primarily Stack Overflow
will provide the strongest solution. The key feature that drive me towards this solution are the strong rules
around questions that are allowed which drive the responses towards being a useful knowledge base rather than 
a question and answer resource where posts tend to discussions with no clear answer to the technical question
being asked. These types of questions have a place but they do not fit as well into the idea of a useful technical
knowledge base.

The next step is for the community as a whole to take a decision on how to take this idea of a shared technical 
HPC knowledge base forward and boostrap its use. One initial option that has been briefly mooted is to run 
a community hack day where the community comes together to seed the chosen option with initial questions and
come up with documentation and guidelnes to help sites adopt the chosen solution.

I think there is a great opportunity here for the community to come together to provide an amazing resource that
will help everyone get the most benefit out of HPC for research.

If you have questions or comments on this topic, I would love to hear them!

