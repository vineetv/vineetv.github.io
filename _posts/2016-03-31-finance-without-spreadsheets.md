---
layout: post
title: Finance without spreadsheets
subtitle: 
tags: [open-source, python, r, spreadsheets]
comments: true
---

As part of the syndicated "View from IIMA" series, my article appeared in
[livemint](https://www.livemint.com/Opinion/2dvUwiWaymaPP9pJ6DSARJ/Finance-without-spreadsheets.html){:target="_blank"}
yesterday. Here is the unabridged version with hyperlinks.

What is common to Barclays, Fidelity and JP Morgan, other than the fact that
they are all large multinational financial institutions? As the regular readers
of this daily would probably recognize, all the three have had to face the
embarrassment of acknowledging spreadsheet errors amounting to hundreds of
millions of dollars.

It has not only been the financial services firms that have been left red-faced
due to "Excel mistakes". MI5, the British intelligence agency ended up [bugging
hundreds of wrong phones in
2011](https://www.gov.uk/government/uploads/system/uploads/attachment_data/file/247324/1239.pdf){:target="_blank"}
due to formatting errors, and the 2012 London Olympics organizing committee
[oversold 10000
tickets](http://www.theguardian.com/sport/2012/jan/04/london-2012-olympic-swimming-tickets-oversold){:target="_blank"}
because of wrong 'data entry'. Such examples abound, just Google ['spreadsheet
errors'](https://www.google.co.in/search?q=spreadsheet+errors){:target="_blank"}. And
by all accounts it seems that people have learned to live with it, and, thanks
to regulators, some have even found ways to make money off it.

The Basel Committee on Banking Supervision [explicitly
instructs](http://www.bis.org/publ/bcbs239.pdf){:target="_blank"} banks to have
"effective mitigants in place" against errors creeping in due to "manual
processes". The industry has naturally responded, and many risk consulting firms
today provide advisory services to manage spreadsheet risk. Not many outside the
risk management world would probably be aware, but there even exists a [European
Spreadsheet Risks Interest Group](http://www.eusprig.org/){:target="_blank"}.

If one looks back at the evolution of spreadsheet software since the days of
Lotus 1-2-3, the look-and-feel apart, nothing much has changed in
substance. Yes, a user has more tricks up her sleeve and there are web apps to
work in groups now, but, fundamentally, the data in Microsoft Office Excel is
still organized and analysed in a tabular form.

The first version of Excel dates back to 1985, and what is astonishing is that
for almost 30 years much of the corporate world has been using versions of the
same software sold by one firm. As a comparison, despite the market share
enjoyed by Maruti Suzuki Ltd, its cars today are no longer the obvious choice
for most upper-middle class Indians, and one would have thought loyalty would
matter more for automobiles where after-sales service network is valued. But in
the corporate world, the larger the organization, more prevalent seems to be the
use of Excel.

Now lest this piece be seen as a rant against Excel or spreadsheets, let me
admit that I am no anti-spreadsheet evangelist. I used to be an Excel user in my
earlier job, and continue to use [Libre
Office](https://www.libreoffice.org/download/libreoffice-fresh/){:target="_blank"}
for quick, back of the envelope calculations. There is no denying the utility of
a spreadsheet software, and given the ubiquity of Microsoft systems in
organizations, perhaps even unavoidable. It remains useful for prototyping,
basic data analysis and teaching elementary statistics, but, in my opinion, it
is not exactly suited for large projects and serious scientific research.

As Harvard professors Carmen Reinhart and Kenneth Rogoff found out, despite the
quality and substance of their research, a couple of [avoidable spreadsheet
errors](http://www.livemint.com/Politics/HMBU2nP7oI8Cb6wnEPddgN/Influential-economists-acknowledge-errors-in-debt-paper.html){:target="_blank"}
unnecessarily diverted attention from the main message of their work. And then
there is the famous [London
Whale](http://www.livemint.com/Politics/fSiuUeqDerBodPhC8eao5I/US-indicts-2-former-JPMorgan-traders-in-London-Whale-case.html){:target="_blank"}
incident. As Mint's readers would remember, it took more than a year for JP
Morgan to get that monkey off its back, and not without its [CEO Jamie Dimon
having to take a huge salary
cut](http://www.livemint.com/Companies/7il3Sd5CMoXZeTKjVbd8YN/JPMorgan-cuts-Dimons-bonus-on-Whale-trade.html){:target="_blank"}.

I can't speak for other areas, but use of spreadsheets for quantitative
finance - by which I mean portfolio analysis, financial engineering and risk
management - is just inefficient, if not outright lazy. Even at the basic level,
given the quantum and nature of data involved, it just invites too many bad
practices - cell references, manual inputs and copy-and-paste habits, virtually
unreadable formulas, unwieldy formatting, multiple tabs and resultant humongous
file sizes, over-use of colors with clumsy legends, misleading and ugly graphs,
and the list goes on. Yes, I know many of these can be obviated, and existing
power users are smart about it, but am not sure beginners appreciate the
pitfalls until it's too late.

More than reflecting problems with any particular spreadsheet software, what
these examples illustrate is a lack of context of the scale and scope involved
in the choice of computing environment. Working in large projects, with
interconnected data and modern techniques, is best done in an environment which
facilitates efficient separation of raw data, its organization, analysis and
output. A spreadsheet software is simply isn't up for it.

Perhaps Newton's first law of motion has something to do with it too, but this
inertia in the industry has meant that many business schools continue to
predominantly use spreadsheets for quantitative courses. While jobs in the data
science and analytics world has meant more acceptance of the programming
languages R and [Python](https://www.python.org/){:target="_blank"} in
'elective' courses, much of the basic curriculum still relies on spreadsheets.

All this, of course, goes back to the more fundamental issue of whether a
business school curriculum should be proactive or reactive. As far as the choice
of computing environment in curricula is concerned, most business schools have
been in the reactive mode, likely because of placement pressures. The students,
of course, do not have an incentive to shift and prefer the status quo, as most
naturally want to 'blend in'. The question is whether these arguments hold water
in today's environment of easy availability of MOOCs on all kinds of things
quantitative, including free training courses in Excel, R and Python. Not in my
opinion.

When it comes to doing complex quantitative analysis and using cutting-edge
methods, spreadsheets simply lack the statistical sophistication of R and the
power of Python. In fact, both today come with their web apps -
[Shiny](http://shiny.rstudio.com/gallery/){:target="_blank"} for R and
[Jupyter](http://ipython.org/){:target="_blank"} for Python - that makes
illustrating and sharing applications a cinch, and fun.

An unfortunate response to lack of ability of spreadsheets to do modern
statistical analyses in finance has been to purchase proprietary/black-box
software, many of which often simply adapt and package the existing freely
available open-source programs. This not only results in an inefficient use of a
business school's money, but also leads to perpetuation of bad habits, as for
commercial reasons most software try to give their software the look-and-feel of
spreadsheets. It is also problematic from a pedagogical standpoint as one is
implicitly telling students to rely on someone else's implementation without
worrying about the details. The more courses use such software, stronger this
reinforcement to rely on black-box software. To say that 'my teacher used that'
or 'US schools do that' is, at best, naive.

A common refrain against switching to R/Python is that their use requires
programming and 'I am not from engineering/science background'. It is like
saying that I do not want to learn English because I studied in a school where
the medium of instruction was vernacular. Yes, as with any new language, no
denying there is a set-up cost involved, but not more than about a week from an
interested user.

Although we still have a long way to go, I believe that among Indian business
schools, IIMA is at the forefront of introducing open-source computing
environment to its students, both at our post-graduate and doctoral programs. We
have done away with our compulsory Excel course in the first year, and many of
us use R and Python in the classroom regularly. A few of us in the finance area
have not only completely shifted to open-source environment for our research and
teaching but have also completely ditched the proprietary operating systems in
favor of [Ubuntu](http://www.ubuntu.com/desktop){:target="_blank"}, or even
[Arch Linux](https://www.archlinux.org/){:target="_blank"}. Now that's a topic
for another day.

[PS: In my rant against the outlet, I wish the sub-editor had taken a *bit more*
effort to write the blurb than just snipping a sentence off the text, with the
first person singular and all!)]

