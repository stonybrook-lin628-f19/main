Computational syntax
====================


| Course        | Info                            |
| --:           | :--                             |
| Course#       | lin628                          |
| Time          | M 5:30-8:20pm                   |
| Location      | CompLab (SBS N-250)             |
| Website       | lin628.thomasgraf.net           |
|               |                                 |
| Instructor    | Thomas Graf                     |
| Email         | [coursenumber]@thomasgraf.net   |
| Office hours  | tbd                             |
| Office        | SBS N-249                       |

Course outline
--------------

### Bulletin description

An in-depth survey of natural language syntax from a computational perspective.
The primary focus is on combining state-of-the-art techniques from formal language theory with empirical insights from linguistic theory.
Topics covered vary by year and may include tree transducers, logics for tree description, weak and strong generative capacity of natural language, lexicalized grammar formalisms, unification grammars, or the expressivity of probabilistic formalisms.

### Full description

This course will focus on three aspects of computational syntax and  evaluate them from a perspective that is equally rooted in theoretical linguistics and NLP:

1.  Does syntax require tree structures?

    We will look at finite-state approaches to syntax and how these formalisms --- even though they generate strings instead of trees --- naturally give rise to tree structures.
    We will also discuss why the competence-performance distinction is computationally inevitable, and what this entails for real-world applications. 

2.  What purpose does syntactic structure serve?

    Combinatory Categorial Grammar (CCG) will be introduced as an example of how syntactic structure isn't just a matter of ivory-tower theorizing, but offers concrete advantages in real-world applications.
    In particular, we will look at how CCG directly maps syntactic structures to semantic interpretations, why CCG's allow for efficient parsing, and how CCGs are automatically inferred from corpora.
    CCGs will be contrasted to Minimalist grammars (MGs), a formalization of Minimalist syntax.
    Great attention will be paid to what parts of the MG ecosystem are currently lacking compared to CCG, and what needs to happen for MGs to make major inroads into NLP.

3.  What are the limits of syntactic structure?

    CCG and MGs (and any other grammar formalism under the sky) still allows for massive overgeneration.
    Overgeneration is not only theoretically unappealing, it also complicates parsing and machine learning.
    I will discuss recent work on subregular syntax that identifies tighter restrictions on the shape of syntactic structures.
    This work ties directly into my NSF Career award, and this part of the course acts as a kind of boot camp for potential RAs.


### Prerequisites

Students are expected to have some previous experience with syntax at the undergraduate or graduate level.
Students who do not satisfy this requirement should be enrolled in Syntax 1 at the same time.
No other computational courses are enforced prerequisites, but students who have not taken MathMethods, CompLing 1 or CompLing 2 should bring a great deal of willingness to engage with syntax at a high level of abstraction and formalization.


Selected topics
---------------

### Schedule

The schedule consists of three components:

1. a *boot camp period* for the first three weeks,
1. an *exploration period* with one meeting each for weeks 4-15.
1. a *public workshop* on Readings Day (Tuesday, Dec 10).

The boot camp is run in a normal lecture style and covers important concepts and techniques to get everybody up to speed.
The exploration period is more like a seminar, with students reading, discussing, and producing bleeding edge research with the instructor's guidance.
By condensing the boot camp into a high intensity period of three weeks, there is overall more time for student research outside of the class room.

A preliminary schedule of topics for the boot camp is shown below.
The schedule will likely change after the first meeting based on student requests.

| **Day**   | **Time**  | **Topics**                                             |
| --:       | :--       | :--                                                    |
| M, Aug 26 | 5:30-8:20 | syllabus, scheduling, big picture                      |
| W, Aug 28 | 2:30-3:50 | tree structures from string models                     |
| W, Aug 28 | 5:30-8:20 | CFGs, AVMs, CG, and lexicalization                     |
| F, Aug 30 | 2:40-5:20 | CCG overview, comparison to MGs                        |
| M, Sep 2  | none      | Labor Day                                              |
| W, Sep 4  | 2:30-3:50 | CCG and MG practice session                            |
| W, Sep 4  | 5:30-8:20 | corpora and treebanks, basics of parsing               |
| F, Sep 6  | 2:40-5:20 | Parsing of CCGs and MGs                                |
| M, Sep 9  | 5:30-8:20 | More on parsing                                        |
| W, Sep 11 | 5:30-8;20 | Generative capacity and the need for subregular syntax |
| F, Sep 13 | none      | attend Sprouse colloquium!                             |

After the bootcamp, we will have 11 meetings of 80 minutes each, spread evenly over the rest of the semester. 
Weekday and time will decided together with the students.

### Readings

Some topics may have assigned readings, which will be announced in class.
All readings will be made available in the [readings repository](https://lin628.thomasgraf.net/readings).
This is a private Github repository, so students will need a Github account to get access.


Teaching goals
--------------

- assess the challenges of syntax for cognitive science on the one hand and language technology on the other hand
- identify important areas of interaction between theoretical syntax and computational linguistics
- critique syntactic proposals from a computational perspective
- develop familiarity with computational ecosystems for syntax (tree banks, parsers, software packages)
- master the basic concepts of phrase structure grammars, CCG, MGs, Dependency grammar, and subregular syntax
- compare CCG and MGs on empirical, theoretical, and computational grounds
- develop learning autonomy and the ability to expand your knowledge of computational syntax through self-study


Grading
-------

This course can be taken for variable credit (0-3).
Student grades are determined by the following components:

1.  **Attendance & class participation** (0+ credits)  
    Everybody is expected to attend every class.
    Attendance here means both physical and mental presence.
    You are expected to be actively engaged, ask questions, and participate in discussions.
    Simply parking your body in the CompLab at the scheduled time does no constitute attendance.

1.  **Class summary** (1+ credits)
    Instead of lecture notes, there will be student-produced summaries of each class.
    For each session, a small group of students who are enrolled for at least 1 credit will compile their lecture notes into a short handout.
    Group size will vary between 1 and 3 depending on the length of the session.

1.  **Workshop participation** (2+ credits)
    We will have a computational syntax workshop at the end of the semester.
    Students who are enrolled for at least 2 credits have to actively contribute to this workshop.
    This may take the form of:

    - a short tutorial session, e.g. on CCGbank or how to set up and use a specific parser,
    - a 10 minute presentation of an open research problem,
    - a 20 minute presentation of novel research results by a student.

1.  **Abstract, paper, or piece of software** (3 credits)
    Students who are enrolled for 3 credits must do some kind of original work, either research or coding-oriented.
    They must also convert this work into a concrete product for their academic or professional portfolio.
    This may take the form of:

    - a highly polished 2 page abstract that will be submitted to a conference, or 
    - a short research paper (8 to 16 pages, depending on the targeted conference), or
    - a demo paper for a piece of software, or
    - a piece of code, released on Github, Gitlab or a comparable online repository, or
    - a series of high-quality posts for publication on the [Outdex](https://outde.xyz), or
    - anything else the student believes will help raise their public profile and marketability (pending permission by the instructor).


Policies
--------

### Contacting me

- Emails should be sent to [coursenumber]@thomasgraf.net.
  Disregarding this policy means late replies and is a sure-fire way to get on my bad side.
- Reply time < 24h in simple cases, possibly more if meddling with bureaucracy is involved.
- If you want to come to my office hours and anticipate a longer meeting, please email me so that we can set apart enough time and avoid collisions with other students.

### Disability support services

If you have a physical, psychological, medical or learning disability that may impact your course work, please contact Student Accessibility Support Center, ECC (Educational Communications Center) Building, Room 128, (631)632-6748.
They will determine with you what accommodations, if any, are necessary and appropriate.
All information and documentation is confidential.

Students who require assistance during emergency evacuation are encouraged to discuss their needs with their professors and Student Accessibility Support Center.
For procedures and information go to the following website: <http://www.stonybrook.edu/ehs/fire/disabilities>.

### Academic integrity

Each student must pursue his or her academic goals honestly and be personally accountable for all submitted work.
Representing another person's work as your own is always wrong. Faculty is required to report any suspected instances of academic dishonesty to the Academic Judiciary.
Faculty in the Health Sciences Center (School of Health Technology & Management, Nursing, Social Welfare, Dental Medicine) and School of Medicine are required to follow their school-specific procedures.
For more comprehensive information on academic integrity, including categories of academic dishonesty please refer to the academic judiciary website at <http://www.stonybrook.edu/commcms/academic_integrity/index.html>.

### Critical incident management

Stony Brook University expects students to respect the rights, privileges, and property of other people.
Faculty are required to report to the Office of University Community Standards any disruptive behavior that interrupts their ability to teach, compromises the safety of the learning environment, or inhibits students' ability to learn.
Faculty in the HSC Schools and the School of Medicine are required to follow their school-specific procedures.
Further information about most academic matters can be found in the Undergraduate Bulletin, the Undergraduate Class Schedule, and the Faculty-Employee Handbook. 
