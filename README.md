# cs61a-homework-8--regular-expressions-bnf-solved
**TO GET THIS SOLUTION VISIT:** [CS61A Homework 8- Regular Expressions, BNF Solved](https://www.ankitcodinghub.com/product/cs61a-homework-8-regular-expressions-bnf-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119658&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS61A  Homework 8- Regular Expressions, BNF Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Instructions

Download hw08.zip.

Using Ok: If you have any questions about using Ok, please refer to this guide.

Grading: Homework is graded based on correctness. Each incorrect problem will decrease the total score by one point. There is a homework recovery policy as stated in the syllabus. This homework is out of 2 points.

Questions

RegEx

Q1: CS Classes

Write a regular expression that finds strings that resemble a CS or EE class- starting with “CS” or “EE”, followed by a number, and then optionally followed by “A”, “B”, or “C”. Your search should be case insensitive, so both “CS61A” and “cs61a” would match.

“`py import re

&gt;&gt;&gt; cs_classes(“Is it unreasonable to take CS61A, CS61B, CS70, and EE16A in the summer?”) True

&gt;&gt;&gt; cs_classes(“Can I take ECON101 as a CS major?”)

False

&gt;&gt;&gt; cs_classes(“Should I do the lab lites or regular labs in EE16A?”) True

&gt;&gt;&gt; cs_classes(“thoughts on ee127?”)

True

&gt;&gt;&gt; cs_classes(“Is 70 considered an EECS class?”)

False

&gt;&gt;&gt; cs_classes(“What are some good CS upper division courses? I was thinking about CS 161 or CS 169a”) True “”” return bool(re.search(__________, post))

“`

Use Ok to test your code:

py python3 ok -q cs_classes Q2: Time for Times

You’re given a body of text and told that within it are some times. Times can be written in two different ways:

12-hour AM/PM clock: 07:23AM, 05:24PM

24-hour clock: 23:59, 12:22, 00:00

Write a regular expression which, for a few examples, would match the following:

[’07:23AM’, ’05:24PM’, ’23:59′, ’12:22′, ’00:00′]

but would not match these invalid “times”

[’05:64′, ’70:23′]

“`py import re

def match_time(text): “”” &gt;&gt;&gt; match_time(“At 07:23AM, I woke up and had some coffee.”) True &gt;&gt;&gt; match_time(“I looked at my phone at 12:22 to check the weather.”) True &gt;&gt;&gt; match_time(“At 05:24PM, I had sesame bagels with cream cheese.”) True &gt;&gt;&gt; match_time(“At 23:59 I was sound asleep.”) True &gt;&gt;&gt; match_time(“After, the clocked turned to 00:00.”) True &gt;&gt;&gt; match_time(“Mix water in a 1:2 ratio with chicken stock.”) False &gt;&gt;&gt; match_time(“At work, I pinged 127.0.0.1:80.”) False &gt;&gt;&gt; match_time(“The tennis score was 40:30.”) False “”” return bool(re.search(____, text)) “`

Use Ok to test your code:

py python3 ok -q match_time

BNF

Q3: Linked List BNF

For the next two problems, you can test your code on code.cs61a.org by adding the following line at the beginning before the problem’s skeleton code:

?start: link — replace link with tree_node for the next question

In this problem, we’re going to define a BNF that parses integer Linked Lists created in Python. We won’t be handling Link.empty.

For reference, here are some examples of Linked Lists:

Your implementation should be able to handle nested Linked Lists, such as the third example below.

Link(2)

Link(12, Link(2))

Link(5, Link(7, Link(Link(8, Link(9)))))

“` link: “null”

?link_first: “null”

?link_rest: “null”

%ignore /s+/ %import common.NUMBER “`

Use Ok to test your code:

py python3 ok -q linked_list Q4: Tree BNF

Now, we will define a BNF to parse Trees with integer leaves created in Python.

Here are some examples of Trees:

Your implementation should be able to handle Trees with no branches and one or more branches.

Tree(2)

Tree(6, [Tree(1), Tree(3, [Tree(1), Tree(2)])])

“` tree_node: “null” ?label: “null” branches: “null”

%ignore /s+/ %import common.NUMBER “`

Use Ok to test your code:

py python3 ok -q tree

Regex Parser

Previously in CS61A you studied regular expressions (regex), a grammar for pattern matching in strings. In this question you will create a BNF grammar for parsing through regular expression patterns, which we will denote as an rstring. Below, we’ve defined the following skeleton for rstring grammar:

“` rstring: “r”” regex* “””

?regex: character | word

character: LETTER | NUMBER word: WORD

%ignore /s+/ %import common.LETTER %import common.NUMBER %import common.WORD “`

The current implementation is very limited, and can only support alphanumeric patterns which directly match the input. In the following questions, you will implement support for a limited subset of regular expression features.

NOTE: for the purposes of testing, we require that your syntax trees match the doctests’. Be sure to define all expressions as noted in the question, and prefix all extra expressions not mentioned in the question with a ? (such as ?rstring).

Q5: Grouping and Pipes

In this question, you will add support for grouping and piping.

Recall that grouping allows for an entire regular expression to be treated as a single unit, and piping allows for a pattern to match an expression on either side. Combined, these will let us create patterns which match multiple strings!

Define the group and pipe expressions in your grammar.

1. A group consists of any regex expression surrounded by parentheses (()).

2. A pipe operator consists of a regex expression, followed by a pipe (|) character, and lastly followed by another regex expression.

For example, r”apples” would match exactly the phrase “apples” in an input. If we wanted our pattern from before to match “oranges” as well, we could expand our rstring to do so using groupings and pipes: r”(apples)|(oranges)”.

Use Ok to test your code:

py python3 ok -q regex_grouping Q6: Classes

Now, we will add support for character classes.

Recall that character classes allow for the pattern to match any singular character defined within the class. The class itself consists either of individual characters, or ranges of characters.

Specifically, we define the following:

1. A range consists of either NUMBERs or LETTERs separated by a hyphen (-).

2. A class expression consists of any number of characters or character ranges surrounded by square brackets ([]).

Use Ok to test your code:

py python3 ok -q regex_classes

Submit

Make sure to submit this assignment by running:

py python3 ok –submit
