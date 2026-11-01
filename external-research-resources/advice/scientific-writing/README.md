---
metaLinks:
  alternates:
    - /broken/spaces/mzd6xx2kCQ8dn7PxnBoD/pages/S5a18u922etG8HhmSEWv
---

# 🛠️ Scientific Writing

Scientific writing is difficult—words on the page can expose the depth and subtlety of one's thought—often it leaves the writer surprised by the parts of their logic that are under-developed or under-supported. There are many styles of writing that suit different people and writing styles: from carefully constructing each piece, to the dump-and-clean model of putting relatively raw info down on the page in the first stage, and then refining it later into polished scientific prose in subsequent stages.

<div align="center" data-full-width="true" data-with-frame="true"><figure><img src="../../.gitbook/assets/bafkreigu6ifvz6zpz5jlqqbpwptivir67tgf6drln7og4azvngw3ckkuv4.jpg" alt="" width="288"><figcaption><p>Writing clearly, coherently, and with depth about a complex scientific process is very difficult.</p></figcaption></figure></div>

Scientific writing is an art, and like any human art form, you can spend a lifetime working on improving your clarity of thought and presentation. It's challenging but there should be some joy in this. This is part of the craft of science as a social process—if you have great ideas but cannot articulate them clearly, it will hold back progress.

Also, like many other human traditions, we are following a historical line of scientific practice; **When we write scientific manuscripts, we're following in the footsteps of some of the deepest and most creative thinkers in human history**. You should respect this human tradition by taking seriously the challenge of thinking deeply about difficult problems, and articulating your thought process in the form of valuable contributions to the scientific literature.



## Structuring arguments

Scientific writing is different from a technical set of notes from say a lab book. We are communicating a human's thought process: from what motivated an investigation, to how a method was designed, to how we chose to present the results, and to what we think the interpretation of the results are (and why), through to drawing generalities from the specifics.

**Structuring a paper**

* [This PLoS CB article](https://doi.org/10.1371/journal.pcbi.1005619) provides a strong foundation for structuring a paper across 10 Simple Rules.
* And this PLoS CB article is on [How to write a scientific paper in fifteen steps](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1013505).

**Writing an abstract**

Writing a good abstract is crucial—the vast majority of people are time-strapped and, if they get past your title, this is as much as they will read of your work. So writing a clear statement of what you have done and how it impacts key open questions in a widely accessible way, is super important.

* [This Nature template](https://www.nature.com/documents/nature-summary-paragraph.pdf) for how to structure an abstract is very informative.

#### Structuring a scientific argument

* **The template:** A general template for structuring a scientific argument is to first explain the problem, then the solution, then the results, then the implications.
  * This can be applied across all scales of a paper: globally, within each section, and sometimes even across each paragraph.
  * A good paper will have a clear global objective/narrative, and each piece will be clearly set up and explained how it fits within/contributes to that global structure.
* **Logical ordering.** Avoid going backwards, e.g., explaining what the result means and then describing the method method was applied and then afterwards explaining why. This is more confusing than explaining the problem to be solved first, and then motivating the method that appropriately addresses it.
* **Distinguish between the solution and its implementation**. Primarily we make a scientific case for the theory or method to be applied and why it's appropriate. Secondarily we explain how the method was implemented (e.g., the software package or specific numerical scheme used and its version), which can be included in _Methods_, but clearly separated from the scientific argument made on the basis of theory/methods.

## Style

#### Neutral tone

Write clearly and without bias or hype, in a neutral tone. It's important to be interesting and compelling, but never at the expense of accuracy. Read [this](https://elifesciences.org/articles/88654) eLife article for elaboration.

Avoid normative language. Scientific writing is not opinion writing, so do not use normative language about what is better or worse in general, or tell the reader what they should or shouldn't do. In scientific writing, you aim to describe the benefits or advantages of something (or its weaknesses or limitations), but in general, avoid subjectively judging something (either positively or negatively).

#### **Provide sufficient context**

Good scientific writing clearly documents a reasoning process. It's not a technical white paper (describing what was done), it also explains the scientific process (describing why it was done). So make sure you give the reader clear context and motivation for what you are doing and why.

_Examples_:

* Opening a section with "We first outline X".
  * This text can be disorienting for a reader as it assumes that they knows why X is important and how it relates to the rest of the paper. Walk them through: the goal, why it's important, and then the design of an experiment to test that goal.

#### Specify ambiguous terms/phrases

Put yourself in the reader's shoes and be on the lookout for phrases that make assumptions of the reader's knowledge that could make them feel confused, or require them to work harder to follow your logic.

It is common for early drafts to contain many such cases of vague phrasing where the meaning is clear to the writer but need to be spelled out for the target audience. Iterating with this mindset can usually plaster over these gaps.

Keep an eye out for phrasing that implicitly asks the reader to fill in the gaps. Sometimes the answer to the missing question is obvious in context and over-specifying can slow down the pace of the text and annoy the reader, but most writers under-specify more than over-specify, so it's safer to err on the side of clarity and carefully spell out your meaning.

_Examples of potentially vague phrases_:

* Most common case is the use of "this" or "these "
  * These terms/phrases are making the claim to the reader that they should know exactly what we mean by "this" without us specifying. Is it crystal clear in context? If not specify.
* _Example text_: "As a solution, here we" \[solution to what?] _Fix:_ "As a solution to XX, here we"
* _Example text_: "Examples include" \[examples of what?]. _Fix_: "Examples of XX include"

### Tools

**Making LaTeX tables**

You can more easily make tables in LaTeX using this [online editor](https://www.tablesgenerator.com/).

#### Some 'house' rules/tips

* Use the Oxford comma.
* Avoid somewhat vague words like 'framework'.
* Use active voice. E.g., instead of "we provide a detailed description of X", it's much clearer to write: "we describe X in detail". Instead of "X is observable" or "X can be observed", say instead "we observed X".

#### Figures and Captions

* Don't put a reference to a figure/table in parentheses unless it's _super obvious_ what the reader is supposed to get from it. Better practice is to introduce it clearly, and tell the reader what they should expect to see there (in the case of a figure), e.g., "(this concept is illustrated in Fig. 1A)".
* The reader will not look at the figure unless told to—the main text should introduce the figure and all of its panels in the appropriate context of drawing on the evidence shown there to build/support your scientific argument.
* The first line of a caption should (where possible) be a short, descriptive take-away message from the figure (e.g., a scientific claim that the figure supports). Relative to a neutral, descriptive title, this can be very helpful for the reader to know what the results in the figure are being used as evidence for.
* The rest of the caption should describe what is shown in the figure, and contain enough information to be able to understand the axes and plot elements, etc. But it is not a place to describe the results or their implications---this is what the main text is for.

#### Numbers

* If your measurement is a physical quantity, _always_ accompany it with the physical units it was measured in. Separate the unit with a small-space `\,` in Latex, e.g., `3\,m`, or using option-space in a text editor.

#### Precision

* Phrase ideas precisely, avoiding ambiguity. For example, "we conducted experiments on **various** simulated dynamical processes" (clearer as "we conducted experiments on three simulated processes: (i) …"). Look out for words like "various" or "around" or "like" of "few" or "small" or "low" or "high" and check whether they could be made more precise.
* Avoid words like "would" or "could" or "can" when talking about what was done. Instead, use "we did X" or "we applied Y" or "we used Z".
* Think about the number of significant figures that you report your measurements to. Do not specify a quantity to greater precision than the order of magnitude of error in the measurement of that quantity.
* If you have an error associated with a measurement, (3.421 +/- 0.5), this tells you explicitly where the precision of the measurement is irrelevant: 3.4 +/- 0.5.
* _p_-values should be reported to one significant figure (e.g., 0.04, not 0.037621). Ain't no one be caring about further precision.

#### Equations

* Each variable should be clearly defined with a single symbol. Don't use multiple symbols to define a single variable, like _TN_, for example, as it is then considered as the variable _T_ multiplied by the variable _N_.
* When using text in an equation, use `\mathrm{}` or `\text{}` to ensure it is typeset correctly,
  * e.g., `a_\mathrm{max}` or `a_\text{max}`, not `a_{max}`.

#### Text

* Don't use ampersands (&) unless desperate for space (e.g., in tables).
* Semicolons should be used to separate list items when each item is long (and may itself contain a comma).

#### Abbreviations

* Shorten "Figure" to "Fig.", "Figures" to "Figs" or "Figs.", and "Equation" to "Eq.", except never abbreviate the first word of a sentence.
* Use "\~" to force-prevent a line break for references, as "Fig.\~\ref{fig:label}" and "Eq.\~\eqref{eqn:label}"
* Write as "e.g.," and "i.e.," (with commas) not "eg" and "ie" (without commas). The abbreviation "cf." is used to mean "compare" and is not followed by a comma.
* When using an N-dash, do _not_ use a space either side of it, e.g., "the results---which were surprising---were published in Nature", but _do_ use a space either side of an M-dash, e.g., "the results -- which were surprising -- were published in Nature".
* Don't hyphenate after an adverb ending in -ly, e.g., "a highly significant result" not "a highly-significant result".

#### Citations

* Use a consistent cite key format with the BetterBibTeX package for Zotero. I recommend `auth+year+":"+shorttitle(3,3)`.
* Use `\citet{}` when embedding a reference in the sentence (e.g., "Following `\citet{}`, we decided to…").

