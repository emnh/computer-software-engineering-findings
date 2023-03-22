# Computer Software Engineering Findings

# EDIT: ChatGPT wins

Verdict: Don't read this article. Go ask ChatGPT your questions instead. Or another suitable AI tool.

# EDIT: I found a verdict

The verdict is that the real world with as broad scope as large scale software development can't as of yet be reliably studied in isolated University studies, so for now the best we can do is use our intuitions about what works best as rational and intelligent people given common arguments for and against different features in programming languages, which boils it down to an aggregation of subjective votes, i.e company politics. If you do want some arguments to rally your cause, look further below:

[Dan Luu quotes an article](https://danluu.com/empirical-pl/) with the conclusive verdict that the choice of programming language is significant but modest compared to other factors. The article he quotes, [A large scale study of programming languages and code quality in github](https://dl.acm.org/doi/10.1145/2635868.2635922) has the following abstract:

> What is the effect of programming languages on software quality? This question has been a topic of much debate for a very long time. In this study, we gather a very large data set from GitHub (729 projects, 80 Million SLOC, 29,000 authors, 1.5 million commits, in 17 languages) in an attempt to shed some empirical light on this question. This reasonably large sample size allows us to use a mixed-methods approach, combining multiple regression modeling with visualization and text analytics, to study the effect of language features such as static v.s. dynamic typing, strong v.s. weak typing on software quality. By triangulating findings from different methods, and controlling for confounding effects such as team size, project size, and project history, we report that language design does have a significant, but modest effect on software quality. Most notably, it does appear that strong typing is modestly better than weak typing, and among functional languages, static typing is also somewhat better than dynamic typing. We also find that functional languages are somewhat better than procedural languages. It is worth noting that these modest effects arising from language design are overwhelmingly dominated by the process factors such as project size, team size, and commit size. However, we hasten to caution the reader that even these modest effects might quite possibly be due to other, intangible process factors, e.g., the preference of certain personality types for functional, static and strongly typed languages.

# Introduction
This project started out as my attempt to choose an open source project to contribute to, preferably a programming language of global impact.
The criteria for choosing a project are the impact on the global economy and my own biased and perhaps not entirely rational motivations.
Since these may be opposed to each other, I started on a journey to discover my own biases and try to uproot any irrational motivations.
It may be appropriate for me (and you, if you like) to read the Wikipedia article on [rationality](https://en.wikipedia.org/wiki/Rationality) at some point.

# Contribute towards General AI or to an existing impactful programming language
There is a conflict in my mind whether I should contribute to the development of artificial intelligence, towards its generality, as worked on for example in Google Deepmind. I deem general AI most important and seems to be in line with the times. But on the other hand my motivations and feelings tell me I should contribute to a programming language, which I find easier, and thus more practical to get started hands-on with. I'm not sure I'm sufficiently intelligent, I just have an insecure feeling about it, to contribute towards general AI, which is why I instead set off on a journey to discover the impact of various programming languages on software engineering and thus the economy of the world.

# Are all programming languages created equal?
On one hand, as Bob Martin says, all programming languages are just [sequence, selection and iteration](https://twitter.com/unclebobmartin/status/1010660993851117569?lang=en). Are they therefore created equal? People do have different preferences, but are they rational? Some people argue that [mathematics must be beautiful](https://en.wikipedia.org/wiki/Mathematical_beauty), a position taken by G. H. Hardy, and one may think that the same may be true about programming, but I think only very short algorithms and programs can be beautiful, not complex programs that deal with the real world, simply because they are too large and complex to be held in anyone's mind, and if they are too complex to be held they are too complex to be understood in their totality. This means that being rational in software development boils down to having intelligent people who apply rational thinking based on heuristics and statistics. Another reason is that the inputs to large computer programs quickly explode combinatorially such that there is no way of testing all inputs.

# Personal bias
Given that I want to contribute to an impactful programming language I want to know more about which features are statistically and economically useful in a programming language in order to decide on a language to contribute too. As a personal criteria or bias I also must note that I want to contribute to a programming language which has a company behind it where I could potentially look for a job later on, and this, due to personal reasons, excludes Microsoft, where I've worked before, even though I like the F# programming language. I do currently have a bias towards statically typed functional programming languages. I find functional beautiful and elegant, but that is not necessarily a rational motivation. On the other hand I do also feel that the cognitive load is higher when writing functional code. Let's also remember that the selecting the right tool for the job is also important, and that for small scripts and one-off jobs dynamic and imperative may be the most efficient even though for large software engineering other tools, say statically typed and perhaps functional, may be more appropriate. There is never a substitute for having intelligent rational people do the software development, because as we said earlier, testing for all possible inputs is impossible and we have to resort to heuristics (a philosophy or discipline of software engineering perhaps). You can't just have an irrational person rely on the compiler or running limited tests until the program works for some particular cases and expect it to be maintainable, robust, secure and efficient. 

# What features are statistically and economically useful in a programming language?
Before we start, is this even the right or all-encompassing question? I think for the industry it is the most relevant one, but it completely omits the impact of psychology in software development. Whether a language is psychologically beneficial to use for a human is a neglected question, as I consider myself more knowledgeable about programming than about psychology. With this "disclaimer" out of the way, I proceed to research which features are useful in differentiating the economical impact of various programming languages. [A comparison of programming languages](https://en.wikipedia.org/wiki/Comparison_of_programming_languages) might be useful in discovering which features to differentiate by.

# Is static typing useful?
[The article "An empirical study on the impact of software maintainability"](https://www.researchgate.net/publication/259634489_An_empirical_study_on_the_impact_of_static_typing_on_software_maintainability) attempts to answer the question.
Quoting the conclusion of the article, the answer in my opinion is yes:

> The result of the experiment can be summarized as follows:
> * Static type systems help humans use a new set of classes: For four of the five programming tasks that required using new classes, the experiment revealed a positive impact of the static type system with respect to development time. For one task, we did not observe any statistically significant difference (possibly due to learning effects).
> * Static type systems make it easier for humans to fix type errors: For both programming tasks that required fixing a type error, the use of the static type system translates into a statistically significant reduction of development time.
> * For fixing semantic errors, we observed no differences with respect to development times: For both tasks where a semantic error had to be fixed, we did not observe any statistically significant differences.

> We believe that the most important result is that the static type systems showed a clear tendency in class identification tasks, and that we found a first indicator that this is caused by a reduced navigation effort. This makes the result closely related to the study by Ko et al. (2006) who measured in an experimental setting that 35 % of the development time was spent on navigating through the code. It seems plausible to assume that—due to the type annotations in the code—developers do not have to search in a large number of different files how they can use a given (undocumented) API. Instead, the type annotations directly guide them to the right place. This implies a reduction of the navigation costs.

# Is meta-programming useful?
First off I'll give my personal opinion rather than do the research: Perhaps for the Ivory tower of University projects and excessive cognitive capacity it might be useful with metaprogramming, but I question the legibility and comprehensibility of such advanced techniques to the lowest common denominator of other people who have to maintain your software. I do love the challenge of using meta-programming now and again in personal projects though. I encountered an abandoned university project in programming language research, without naming it, and from there I also encountered an active project that totes itself as the ["The one-stop shop for metaprogramming"](https://www.rascal-mpl.org/) and its [github repo](https://github.com/usethesource/rascal) with around 19k commits but only 345 stars as of this writing. I defer judgement on whether it is a useful project for the industry as I need to research on who uses it, but my intuition is that it is too academic for me to want to contribute to it. I'm on a quest to be more rational and therefore I want to have broader impact.
