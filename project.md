# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?

Current presentation softwares all have roughly the same output: a deck of
slides that can be played through linearly.
For my project, I hope to create a DSL that expands the capabilities of the user
to make more dynamic presentations that don't have to follow this format.
Some restrictive elements of traditional presentations I want to change are:
* All the information on previous slides is lost on the next (unless explicitly
copied)
* It is difficult to change styles of components (size, color, transparency,
etc.) other than visibility at each transition
* Examining parts of large diagrams typically involves disjointed transitions

This would be more geared toward those familiar with web design since it would
borrow many of the behaviors and syntax rules from CSS/JS.
Although this target audience may make the tool seem more restrictive, I believe
it will offer an avenue for users to more rapidly understand how to use this DSL
since it won't be a completely foreign language.

### Why a language?

Since this is a visual domain, I can see how a language may seem like an
ineffective tool to use rather than a GUI, but I believe there are advantages
the language format provides.
Firstly, I really like components of my presentation to be constrained precisely
how I want them, so I think a language is more suitable for this.
Next, this is using web-based output, so those familiar with web development
will be familiar with this process of programming components and viewing the
output in a browser.
Finally, I really want the resulting program to not feel limiting, so if the
user wants to add features beyond what I am able to incorporate into the
program, I think they should be able to simply edit the output HTML/CSS/JS with
their desired behavior.
If this is a language, it makes that process much more seamless since they will
already be working with certain variable names and know what attributes
different components have, so they can easily find what they want to edit.

### Why you?

I am really interested in seeing if I can find a way to make presentations
completely different than the rigid slide-based format of every other software.
I also love web design and trying to make websites aesthetically pleasing, so
this project is something that I will find both satisfying and useful.
There wasn't really any particular thing that sparked this idea for me.
I think just generally, I have been dissatisfied with the structure of
presentations and have been considering ways to make them more understandable
and engaging for a while now.
As a bonus, I am also a bit dissatisfied by how most websites are layed out with
a bunch of text or graphics layed out linearly (although I know there's more
variety in websites than there are in presentations), so this could be an
alternative tool for creating websites as well.

### Domain

Dynamic web-based presentation design

### Interface (syntax)

How I am imagining it is that the user can add _components_ and _behaviors_ to
their presentation, and then immediately open the result as a webpage.
The webpage could have a frame selector at the bottom for easy navigation
between keyframes.
This resulting webpage would be completely usable as the final presentation.
As they are developing, they can refresh the webpage to see the updates they
make, but this would also require the user to render the program each time they
want to check.
I want the experience to be similar to web development, except, unfortunately,
the web developer tools won't work with my language since it is external.

Additionally, I think it would be useful if the user could see each component
they create as a stand-alone file with annotations for debugging purposes.
This is more of an added feature, so I am not sure I will actually be able to
get to this part of the project by the end of this class.


### Operation (semantics)

The main way I hope this project runs is that after the user creates a file with
objects and keyframe controls, they can render the file which will result in
HTML, CSS, and JavaScript files being created.
The user can then open the main HTML file in any browser and it will be a
working presentation!
I believe the main error that will occur is invalid syntax.
If the syntax is part of what I define for the structure of the presentation, I
will ideally display an appropriate error message when the user tries to compile
the program.
If the syntax is something borrowed from CSS/JS, then I may let that compile and
defer to the CSS/JS debugging tools to display those errors, but I'm not
entirely sure how I will convert the user-defined styles and transitions yet.

If I want to get ambitious, another output I would like to add is annotated
versions of each component the user creates (also HTML/CSS/JS).
The primary annotation could be an overlayed coordinate grid so the user can
easily determine where visual features of their object lie.
This would help when the user wants to align a specific visual point to another
rather than aligning only based on the bounding box edges.
The annotation could also show bounding boxes and alignment constraints which
could help with debugging.

### Expressiveness

It should be easy to create fluent web-based presentations.
In contrast to other presentation softwares, it should be easy to keep select
components visible when going between keyframes, it should be effortless to
transition many different object styles rather than just object visibility, and
it should be straightforward to incorporate any web media (animations,
simulations, interactive components, etc.) into the presentation.
Although possible, it should be more difficult to create a "slide deck" in this
language than it would be in other software since doing that would kind of
defeat the purpose of using this language.
It should be impossible to use this program for things outside the domain like
complex computations, creating software, or generally getting non-web-based
outputs.

### Related work

From what I can find, nothing comes close to what I want.
When I look for presentation softwares, every. single. one. uses a slide deck
format and they only seem to differ in more minor features.
Some examples of the existing softwares are PowerPoint, Google Slides, Prezi,
Keynote, Beamer, etc.
In terms of languages that offer the flexibility, HTML/CSS/JS are closest, but
way to broad by themselves to make them easy to create presentations in.
When specifically looking for DSLs, it was a bit difficult to determine if there
could actually be anything because most of what came up was just presentations
about DSLs no matter how I searched it.
Thus, I believe there are not any DSLs in this domain.
I think a main reason there aren't is because slide decks are such a familiar
format, so people tend to create software that follows this tradition.
One drawback of creating a completely new design flow is that it will be foreign
to th user making it more difficult and thus less likely to be used.
However, I believe that the opportunities for more fluidly displaying
information will make my design favorable enough to be usable.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

I think a significant portion of the project will be based on the "language"
aspects since a key part of this is creating features which will essentially be
language components that make different designs easier.
I will spend much of my time debating which features would be most useful to a
user and how I can make the syntax clear, concise, and non-restrictive.
There will, however, also definitely be "systems" aspect that I will need to
consider.
For each feature, I need to think about how I will actually render it in the web
languages, but since I plan to make the syntax fairly similar to CSS/JS, I hope
this part will not be too difficult or time consuming.
Thus, I would guess 60% of the time would be spent on "language" and 40% on
"systems".

### Scope

If I wanted to make a complete replacement for presentation software in this one
class, I believe this would be highly ambitious, but since I just plan to start
the process and make a few unique features, I think the scope is much more
manageable.
What's nice about this project is that the scope can be grown as desired simply
by adding more features.
I think the basic features I want to add may be a little ambitious, but should
definitely be doable in the amount of time we have.

### Benefits and drawbacks

I think the largest benefit is that I am excited about this project, so I will
be eager to spend time working on it and putting in lots of effort to see it
grow.
Additionally, it is helpful that I am pretty familiar with web languages which
makes the interpretation aspects of this project more straightforward than if I
were trying to create an output that I was not already familiar with.
I really like that this project would result in something that I could regularly
use in my day-to-day life and share with others that may have similar
reservations against presentation software.
Finally, I like that the scope is adjustable.
It keeps the project from being overwhelming, but also offers many ways to
challenge me.
When programming, I like having relatively immediate feedback on the
functionality of what I'm writing, so it helps that I can create a basic start
that will allow parsing and interpretation before I create all the features.

In terms of drawbacks, there are a few.
Firstly, I plan to output files in multiple languages which can make the
processing a bit complicated.
Additionally, since I plan to make this an external DSL, I won't have the added
benefits of existing ways to compile the project which may make the result less
user-friendly.
Finally, since there seems to be no similar software related to this domain, it
could suggest that a) this domain is particularly difficult to work with and
there may be some functional issues that I overlooked or b) no one really cares
about this domain and most people are satisfied with current presentation styles
enough that they would not go through the effort of learning a new syntax to get
the added features of this DSL.