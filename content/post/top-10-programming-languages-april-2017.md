+++
title       = "Top 10 Programming Languages: April 2017"
description = "Relative Strength Index for Programming Languages (RSIPL)"
date        = "2017-04-01"
+++

![Languages Logo](/languages.png) The Relative Strength Index for Programming Languages (RSIPL) is a metric I devised and first published starting in March 2017.  RSIPL was created after reading several similar articles and lists.  The ranking methodology that most other lists use is based upon the popularity of the languages on Github (measuring "code"), and on StackOverflow (measuring "discussion").  As good as these lists are, I feel that they are perhaps less timely than they could be, and that they are missing a third critical piece of the puzzle: job postings.

## 10 Most Popular Programming Languages

Following are the top 10 languages in April 2017, using the RSIPL formula:

<center class="moreSpace">
    <table>
        <thead><td>Rank</td><td>Language</td><td style="text-align:right">RSIPL</td></thead>
        <tr><td>1.</td><td>JavaScript</td><td style="text-align:right">82.0</td></tr>
        <tr><td>2.</td><td>Java</td><td style="text-align:right">73.3</td></tr>
        <tr><td>3.</td><td>Python</td><td style="text-align:right">55.2</td></tr>
        <tr><td>4.</td><td>PHP</td><td style="text-align:right">34.9</td></tr>
        <tr><td>5.</td><td>C#</td><td style="text-align:right">34.6</td></tr>
        <tr><td>6.</td><td>SQL</td><td style="text-align:right">34.4</td></tr>
        <tr><td>7.</td><td>C++</td><td style="text-align:right">25.0</td></tr>
        <tr><td>8.</td><td>C</td><td style="text-align:right">16.9</td></tr>
        <tr><td>9.</td><td>Swift</td><td style="text-align:right">12.9</td></tr>
        <tr><td>10.</td><td>Objective-C</td><td style="text-align:right">12.6</td></tr>
    </table>
</center>

This list deviates a fair amount from the [prior list](/post/top-10-programming-languages-march-2017), published one month ago.  This is for two reasons.  First, I have further refined the algorithm for computing scores.  And second, SQL has been added as a language.  Adding SQL greatly effects scoring because RSIPL sub-scores are relative to each other, and SQL does very well with the Job Posting component.

## RSIPL Criteria

I am sure there are many who look at these lists and wonder what the potential is for landing a job if they invest their time and effort into learning one or more of these languages.  Because of this, I felt it important to reflect this in the score. By using job postings as a criteria, the list reflects what I feel is a pragmatic view into the popularity of languages.

Another important note regarding RSIPL: the rating attempts to reflect popularity based on *current activities*, rather than cumulative popularity over the years.  To achieve this, I looked at recent Stack Overflow tags, recent GitHub activity, and recent job postings from both Indeed and Dice.  The job postings were blended together to form one aspect of the score.

So, to summarize, this ranking is intended to reflect very recent activity from the perspective of Open Source code activity, tagged discussions, and job postings.  Each criteria was normalized on a scale of 0-100.  Results were then averaged for each language.

While I feel RSIPL does a better job at capturing current popularity of programming languages than other lists, it is far from perfect.  Although job postings do add a meaningful aspect to the analysis, it is somewhat flawed, because job postings tend to lag behind the latest and greatest trends, as industry is typically slow to respond to change.  In addition, there will always be jobs related to corporate legacy systems that will also skew such ratings.  But to counter that argument, even though there are jobs available for legacy technology, they are still jobs nonetheless, and they still do reflect on the popularity of a given language (so COBOL programmers take heart!).

I intend on posting RISPL ratings over time, perhaps monthly.  I also intend to revise the index as better data becomes available.  Hopefully it is helpful to some in its current form.

---

### **Reader Comments**

none yet.
