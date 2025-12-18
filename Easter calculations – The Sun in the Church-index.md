---
master_file: "[[@EasterCalculationsSun]]"
---
# Index for Easter calculations – The Sun in the Church.pdf

1
The Sun in the Church
Ng Yoke Leng
An academic exercise presented in partial fulfilment for
the degree in Bachelor of Science with Honours in Mathematics
Supervised by
Associate Professor Helmer Aslaksen
Department of Mathematics
National University of Singapore
2002/2003



2
CONTENTS
Acknowledgements i
Summary ii
Author’s contributions iii
1 Preliminaries 1
1.1 About Easter 1
1.2 Roman dating system 3
1.3 The Julian calendar 4
2 Lunar Cycles 6
2.1 Background – why the need for lunar cycles? 6
2.2 Examples of lunar cycles
2.2.1 Augustalis’ cycle 9
2.2.2 The Metonic cycle 10
2.2.3 The Great Paschal Cycle 13
3 Determining Easter in the Julian calendar 14
3.1 Tools
3.1.1 Golden number 14
3.1.2 Paschal full moon 19
3.1.3 Dominical letter/number 20
3.1.4 Epact 25
3.2 Determining the Julian Easter Sunday
3.2.1 Using paschal table, dominical letter and golden number 27
3.2.2 Using Easter tables containing epacts 28
3.2.3 By calculation 30



3
4 From Julian to Gregorian 34
4.1 Problems with the Julian calendar 34
4.2 Gregorian reforms 35
5 Determining Easter in the Gregorian calendar 39
5.1 Modifications of tools
5.1.1 Golden number and lunar table 39
5.1.2 Dominical letter/number 46
5.1.3 Paschal full moon 47
5.1.4 Epact 48
5.2 Gregorian paschal lunar table
5.2.1 Problem 51
5.2.2 Adjustments 53
5.2.3 Effect of the adjustments on Gregorian epact 55
5.3 Determining the Gregorian Easter Sunday by calculation 56
6 Easter algorithms 60
6.1 A selection of Easter algorithms
6.1.1 Easter tables in the Book of Common Prayer 60
6.1.2 Gauss’ Easter algorithm 63
6.1.3 O’Beirne’s algorithm 64
6.1.4 Gregorian algorithm by Lilius and Clavius 65
6.1.5 Carter’s algorithm 67
6.2 Final remark 68
Appendix A 69
Appendix B 70
Bibliography 73



4
ACKNOWLEDGEMENTS
I would like to thank my supervisor, A/P Aslaksen, for all the time he had spent with
me to bring this project to completion. He has been most patient with me, despite
having to explain and re-explain concepts to me sometimes. I appreciate the concern
he has over my general academic work and the humour he injects into our meetings.
Most importantly, I am thankful for the chance to pick up from him, an attitude of a
keen learner and researcher.
“How do you know if you have understood something? First you know it, then you
can explain it, and finally you can explain it in a simpler way for others to
understand.” – a quote from A/P Aslaksen that I will always remember.
A special note to:
Jeremy... for proof-reading my thesis,
Lionel & Ivan... for your daily encouragement and wonderful company,
Daphne, Xuelin, Brandon, Daryl & Xianchang... for your messages and support,
my entire batch of honours classmates...for making classes much more enjoyable,
and my family, especially my sister Kelly,... for your love and understanding,
“thank you.”



5
SUMMARY
There are many indications that the sole important application of arithmetic in Europe
during the Middle Ages was the calculation of Easter date. At that time, the Catholic
Church played an active role in calendar research in order to determine a systematic
way of finding the date to celebrate Easter.
J.L Heilbron’s book, The Sun in the Church, contains a succinct historical account of
how the calculation for Easter had influenced the design for a calendar. He
highlighted the main problems and concerns for the design, the key personnel behind
calendar refinements, and the resultant method of finding a fixed date for Easter. This
is a broad mix of topics which Heilbron had managed to condense into a single
chapter. Inevitably, readers may find it hard to fully grasp the issues packed behind
the few lines of explanation. This paper is thus compiled as a supplement to
Heilbron’s book, to
1. provide more background for Easter and its calculation;
2. give details on the calendar reforms;
3. clarify certain points raised in the book.
Chapter 1 gives a quick overview of what Easter is about, the ancient Roman dating
system and the Julian calendar.
Chapter 2 introduces lunar cycles, a key factor that influences the design of a
calendar. Examples of lunar cycles, including the important Metonic cycle, are
furnished.
Chapter 3 is broadly divided into two parts. The first describes general tools used for
determining Easter Sunday and the second gives the methods themselves.
Chapter 4 outlines the problems with the Julian calendar and the calendar reforms that
were made to the Julian calendar
Chapter 5 is similar to Chapter 3 in structure. It contains descriptions of the modified
tools and methods used in finding Easter Sunday in the Gregorian calendar.
Chapter 6 highlights Easter tables found in the Book of Common Prayer and other
established Easter algorithms by famous people such as Gauss and Knuth.
It is hoped that readers would have a better appreciation of the first part of Heilbron’s
book after going through these various chapters.



6
AUTHOR’S CONTRIBUTIONS
Here is a list of my inputs to this project:
1. I expanded on Heilbron’s explanation of the term “bissextile” by introducing
the ancient way of Roman dating.
2. In Chapter 2, I provided information on lunar cycles to enable readers to
understand Heilbron’s algebraic method of finding luni-solar cycles. Pertaining
to his method, I have also rearranged it to improve clarity.
3. In Table 2, I added the entries corresponding to J = 84 and thereafter found 2
discrepancies between the entries and those quoted by Heilbron.
4. The concept of saltus lunae is highlighted through the introduction of the
Metonic cycle and Table 2.
5. With the help of my supervisor, I have managed to identify interesting
properties about Table 4 and provided explanations for their occurrence
accordingly. Through the discussion of these properties, the concept of golden
numbers can be better appreciated.
6. To demonstrate how the regression of dominical letters takes place, I have
included an example through Table 7.
7. The derivation of the formulae for dominical letters for both Julian and
Gregorian calendars are given in greater detail than that in the source, [8].
8. I have brought up a confusing feature in Table 10, taken from [3]. Here I have
suggested for the epact “0” to be interpreted as “30” and the epact range used
for that table to be taken as 1 to 30 instead of 0 to 29.
9. The Easter algorithms described in [8] are explained in more detail. For
instance, the uniqueness of epact to golden number has been justified
mathematically.
10. Flow-charts have been drawn to summarize the algorithms for determining
Easter Sunday for both the Julian and Gregorian calendars, proposed in [8].
11. Table 11, extracted from [3], has been treated differently from that by Heilbron
to provide a better appreciation of how the solar and lunar equations influence
the epacts over a millenium.
12. Based on one of the meetings I have had with my supervisor, I have come up
with a schematic diagram to illustrate how golden numbers corresponding to
new moons may be shifted out of the usual range of dates into 6 April.



7
Chapter 1
Preliminaries
1.1 About Easter
Even though Christmas seems to draw more enthusiasm from most people, it
is Easter that carries far greater significance for the meaning of Christianity.
The commemoration of the Crucifixion on Good Friday and of the
Resurrection on Easter Sunday is the recognition of the central mysteries and
promises of the religion: the forgiveness of sin and the enjoyment of eternal
life.
There is a chronological discrepancy over when the Crucifixion took place.
The Synoptic Gospels differ from the Gospel of John in their indication of
when the Last Supper – the last meal that Jesus had shared with his disciples
before his Crucifixion – took place. In order to appreciate the account for this
discrepancy better, let us first have an overview of what the Passover Festival
is.
The Passover Festival is the most important event in the Jewish calendar. It is
an 8-day festival, held from the 14th to the 21st day of the Jewish month of
Nisan, to remember the exodus of the Israelites from Egypt under the
leadership of Moses. The Passover meal is consumed on the first evening of
the Passover on 14 Nisan (or technically, 15 Nisan, since the Jewish day
begins after 6pm). During this meal, the food served contains food which
symbolizes the events during the exodus: the paschal lamb which was slain
earlier in the evening and unleavened bread.
All four gospels are agreed that Jesus died on a Friday and the Last Supper
was taken on a Thursday. According to the Synoptic Gospels, the Last Supper
was a Passover meal, which falls on the evening of 14 Nisan (start of 15



8
Nisan). However, for the Gospel of John, Jesus was the new paschal lamb (the
lamb of God) and sacrificed at the same moment of the slaughter of the
Passover lamb. Hence for John, the Last Supper would only be a normal meal
taken on the evening of 13 Nisan instead of 14 Nisan. The discrepancy over
when the Last Supper was held in turn leads to the discrepancy of dates for
when Jesus’ Crucifixion took place. This is seen clearly from the following
table.
Table 1
Date Synoptics’ Chronology John’s Chronology
13 Nisan – Thursday: Last Supper (normal meal) 14 Nisan Thursday: Last Supper (Passover meal)
Friday: Crucifixion
15 Nisan Friday: Passover & Crucifixion Saturday 16 Nisan Saturday Sunday: Resurrection 17 Nisan Sunday: Resurrection
Therefore, Jesus died on 15 Nisan according to the Synoptic Gospels and 14
Nisan according to John. Nevertheless, all 4 Gospels agree that Jesus Christ
was resurrected three days after Friday, which by inclusive counting, was a
Sunday.
By the middle of the second century, the problem of exactly which date that
Easter should be celebrated on had arisen. There were two main groups of
Christians who had different Easter celebration practices. One group, known
as the Quartodecimans, insisted on celebrating Easter on 14 Nisan. These
included Christians who converted from Judaism and others in Asia Minor.
The other, called the Quintadecimans, emphasized the day of the week by
celebrating the Resurrection on the Sunday which followed 14 Nisan. This
group comprised Roman and Alexandrian Christians. Initially, both groups
received great support. However, the unity among the Quartodecimans started
to break down. In addition, there was a rising desire among the Christians to
break away from their dependency on the Jewish authorities in order to
determine the date for Easter. Eventually, the Quintadecimans’ practice
spread.



9
A significant event that reaffirmed the dominance of the Quintadecimans’ or
Western Church’s practice was the first ecumenical council of the Church, the
Council of Nicaea, convened in AD 325. The Nicene Creed was established
then. It declared the Quartodeciman practice heretical and that Easter was to
be celebrated on the same day by all Christians based on the practices of the
Western Church. The following rule was incorporated into their practice:
Easter Sunday, the anniversary of the Resurrection, was to be celebrated on
the 1st Sunday after the paschal full moon that fell on or after the vernal
equinox; the paschal full moon was taken to fall on the 14th day from the
paschal new moon. This rule was designed to ensure, among other things, that
Easter Sunday was never on or before the Jewish Passover.
Despite having a common rule, there was still a significant disparity in the
dates of Easter Sunday as determined by members of the Western Church
the Romans and the Alexandrians. The Romans considered 25 March to be the
vernal equinox but the Alexandrians used 21 March. They also had different
dates for the paschal full moon because they had used different lunar cycles.
The issue of lunar cycles is discussed in detail in Chapter 2.
1.2 Roman dating system
The Romans had an unusual way of dividing their months. The three chief
points of the month were the Kalends, the Ides and the Nones. The Kalends
represented the 1st day of a month and originally marked the appearance of a
new moon. The Ides represented the full moon and occurred in the middle of
the month. For March, May, July and October, Ides fell on the 15th day of the
month, and for the remaining months, Ides fell on the 13th day. The Nones
occurred 9 days before the Ides, counting inclusively in Roman style. Hence it
fell on the 7th day of March, May, July and October and the 5th in other
months. In addition to inclusive counting, the Romans used backward
counting when naming the days within each division. This is illustrated by the
Table 2 and the explanation follows after that.



10
Table 2
Date Term in Roman dating 1 March 2 March
Kal. Mar. VI Non. Mar.
...
...
5 March 6 March 7 March
III Non. Mar. pridie Non. Mar. Non. Mar.
...
...
13 March 14 March 15 March
III Idus Mar. pridie Idus Mar. Idus Mar.
...
...
29 March 30 March 31 March 1 April
IV Kal. Apr. III Kal. Apr. pridie Kal. Apr. Kal. Apr.
The Latin word “pridie” refers to “the day before”. The last day of March was
termed, “pridie Kalendas Aprilis”, meaning day before 1 April, and was
abbreviated as “pridie Kal. Apr.” on calendars used then. By inclusive
counting, 30 March was the third day before 1 April and so it was termed
“ante diem III Kalendas Aprilis” or “III Kal. Apr.” Then 29 March was “ante
diem IV Kalendas Aprilis” and so on, back to 15 March which was the Ides of
March. The day before the Ides, 14 March, was called “pridie Idus Martius”.
13 March was “ante diem III Idus Martius” and so on, back to the Nones on 7
March. Similarly, 6 March was termed “pridie Nonae Martius”, 5 March
termed “ante diem III Idus Martius” and so on until 1 March – the Kalends of
March – was reached. With this inclusive and backward dating system in
mind, we proceed to understand what “bissextile” refers to and highlight other
features of the Julian calendar in the following section.
1.3 The Julian calendar
Prior to the Julian calendar, the Romans used the AUC calendar and numbered
years Ab Urbe Condita, or “from when Rome was founded”. This old calendar
was inadequate for the needs of the emerging Roman empire. Hence in 45 BC,
equivalent to 709 AUC. of the old calendar, Julius Caesar, the commander of



11
the Roman empire then, accepted astronomer Sosigenes’ recommendations
and adopted the Julian calendar.
The Julian calendar introduced a solar year of 365 days and the year was
divided into twelve months. April, June, September and November had 30
days, February, 28 days, and all other months, 31 days. In every 4th year, an
extra day was added into the calendar, making that year 366 days long.
Consequently, the average length of a Julian solar year became 365.25 days.
The extra day added in the 4th year was called a “leap day” and the year
containing the leap day, “leap year”. The leap day was inserted before 24
February, that is, “ante diem VI Kalendas Martius” or the 6th day before 1
March. Hence, the leap day was the second 6th day before 1 March. The table
below illustrates the insertion.
Table 3
Date in nonleap year
Date in leap year
Term in Roman dating
Remarks
23 February
24 February 25 February 26 February 27 February 28 February 1 March
23 February 24 February
25 February 26 February 27 February 28 February 29 February 1 March
VII Kal.Mar. bis. VI Kal. Mar.
VI Kal. Mar. V Kal. Mar. IV Kal. Mar. III Kal. Mar. pridie Kal. Mar. Kal. Mar.
Second 6th day before 1 March; the inserted leap day 6th day before 1 March
In Latin, “sextus” refers to the ordinal “6th”. From this, “sextile” was derived
to refer to the 6th day in a calendar month, and in turn, “bissextile” was second
6th day. The leap day, being the second 6th day before 1 March, was thus also
termed the “bissextile” and the year containing it, “bissextile year”.
After the Julian calendar was adopted, the vernal equinox was kept on 25
March for many years. However, the average Julian solar year length of
365.25 days was longer than the average astronomical tropical year length.
The error accumulated over the centuries and by the 16th century, it had
become a significant amount. Eventually, a new calendar, in use till today,
evolved to replace the Julian calendar.



12
Chapter 2
Lunar Cycles
2.1 Background – why the need for lunar cycles?
The tropical year is the period between the occurrence of one vernal equinox
and the next. Some sources refer to this instead as the vernal equinox year.
However for the scope of this supplement, this definition of tropical year is
adequate. Astronomically, the average length of the tropical year is 365.24219
days. The synodic month or lunation is the period from one phase of the moon
to its next occurrence. Two commonly phases used are the new moon and the
full moon. The astronomical average lunation is 29.53059 days long.
Recall that in order to determine when Easter was to be celebrated, it was
necessary to identify the dates for both the vernal equinox and the paschal new
moon. The vernal equinox is a solar event while the new moon is a lunar
event. This meant that to fix a calendar date for Easter, the calendar so
constructed had to be able to keep its months synchronous with the moon and
its years with the sun. Such a calendar is termed a luni-solar calendar. It would
have been easy to construct such a calendar if the ratio of the length of a
tropical year to that of a synodic month was a rational number. For example, if
a tropical year had 300 days and a synodic month had 30 days, the ratio of the
length of a year to a month is a rational number. It is then natural to construct
a 300-day calendar which is divided into 10 months of 30 days. Such a
calendar would ensure that a lunar event occurs on the same date in the
calendar every year.
Yet the fact is that the ratio of length of the average astronomical tropical year
to that of the synodic month is not an integer. It is thus not possible to fit a
whole number of lunations, forming a lunar year, into a solar year without any
remainder. To reconcile the difference between the lunar years and solar years,
suitable intercalation or insertion of lunations may be used. The calendar thus



13
produced would bear the feature that after a certain number of solar years has
passed, the total length of the solar years is brought into synchrony with that
of the lunar years, or it can be said that this whole number of solar years
would contain the same number of days as a whole number of lunations
would. A lunar cycle is precisely the period of several solar years which has
this property. It ensures that a lunar date is returned to the same calendar date
after a period of several solar years.
Heilbron highlighted an algebraic method in finding suitable lunar cycles, or
what he termed as “luni-solar cycles”, in the Julian calendar. His explanation
is reorganized and made clearer below.
We first highlight a few assumptions made of the lunations used in the
method. Now, because the average synodic month is 29.53059 days long, it is
reasonable to vary the lengths of the lunations between 29 and 30 days; the
former is considered as a hollow lunation and the latter, a full lunation. In the
computation later, assume that a lunar year has 12 lunations, 6 of which are
29-day lunations and the remaining 6, 30-day lunations. Then the average
length of a lunation in the lunar year is 29.5 days. We next assume that all the
intercalated lunations are full lunations. Finally, the lunation containing the
leap day or bissextile is deemed as a full lunation as well. This implies that the
leap day is always inserted into a lunation of length 29 days and never a 30
day lunation. At this point, we may argue that this is an unfair assumption
because in the actual lunar calendar, the leap day could have been inserted into
a 30-day lunation, thereby making it a 31-day lunation. However since we are
only concerned with making sure that the average lunation length is 29.5 days
for the lunar year, it does not matter how long each lunation is and how the
lunations are arranged in the lunar year. It is thus possible to set the leap day
to always fall in a 29-day lunation.
Suppose the lunar cycle is made up of J Julian years, and K lunations. Our aim
is to find the number of lunations to intercalate in the lunar years such that the
number of days contained in J years is equivalent to that contained in K
lunations.



14
We note that each Julian year is longer than a lunar year before intercalation.
Hence in the J-year lunar cycle, the number of lunations, K, contained in the
cycle would be greater than the number of lunations contained in J lunar years,
12J. Mathematically, this is expressed as K > 12J. Let the number of lunations
required for intercalation be p. Hence, K = 12J + p. On the left hand side of the
equation, K has the same number of days as J Julian years, by definition of a
J-year lunar cycle. The average length of a Julian year is 365.25 days and so K
is equivalent to 365.25J days. Then on the right hand side of the equation, 12J
+ p is equivalent to 354.25J + 30p days. The first term is obtained by
assuming that in each of the J Julian years, it contains a lunar year of 12
lunations of 29.5 days each, thereby adding up to 12 x 29.5 = 354 days, and
another 0.25 days due to the insertion of a leap day every four Julian years.
The second term comes about from the earlier assumption that each
intercalated lunation has 30 days. Therefore, the resultant equation is:
365.25J = 354.25J + 30 p ⇒ 11J = 30 p.
Our original aim would be achieved, subjected to a very small error, once we
obtain whole numbers J and p that satisfy the following two conditions:
1. J and p satisfy equation 11J = 30p as nearly as possible;
2. J and p give a close approximation of the average length of a calendar
lunation to the average astronomical lunation length. That is, the calendar
month of length 354.25 30
12
Jp
Jp
+
+ , denoted by Λ closely approximates
29.53059 days.
The attractive possibilities are as laid out in the table that Heilbron has
provided in his book. We reproduce his table with some amendments in the
headers to ensure coherence with the explanation above – wherever “month”
occurs, it is replaced by “lunation”; and in the final column, “mean” is
replaced by “average”. Note that the term embolismic years refer to years in
which an extra lunation has been inserted. Since no two or greater intercalated
lunations are inserted into the same year, the number of embolismic years is
equivalent to the number of intercalated lunations, p, and hence the header for
the second column “Embolist[m]ic years, p”. In addition, we also add in the
quantities for J = 84 in the last row.



15
Table 4 Solar-lunar cycles
Julian years, J
Embolistic years, p
Total lunations, K
Days in J years, M
Days in K lunations, N
Average lunation, Λ
3 1 37 1095.75 1092.75 29.5338 8 3 99 2922.00 2924.00 29.5353 11 4 136 4017.75 4016.75 29.5349 19 7 235 6939.75 6940.75 29.5351 30 11 371 10957.50 10957.50 29.5350 84 31 1039 30681.00 30687.00 29.5351
From Table 4, we observe that all the combinations of J and p gave average
lunations which were all larger than the astronomical average yet very close
among themselves. Coupled with the difficulty of computing the average
lunation to higher accuracy, the people in the ancient days had a lot of
disagreement over which lunar cycle was the most accurate one. In particular,
comparing the average lunation lengths of the 19-year and 84-year lunar
cycles, we see that up to the fourth decimal place, the lengths were the same.
The 19-year lunar cycle was adopted by the Alexandrians and the 84-year
cycle was adopted by the Romans; both cycles are discussed in later sections.
The equal average lunation lengths of these two lunar cycles lends justification
for the conflict between the Romans and the Alexandrians. Even though they
produced lunar tables which did not agree with each other, they had believed
that their own set of tables was the more accurate one. Both groups adhered to
their own set of tables to find the date for Easter Sunday. As a result, the two
groups arrived at different dates for Easter celebration.
2.2 Examples of lunar cycles
In the following sections, we give descriptions of some prominent lunar cycles
that were proposed and/or implemented in the construction of lunar tables.
2.2.1 Augustalis’ cycle
This cycle was created by Augustalis, an unknown Roman, in the early third
century. It was 84 years long and contained 1039 lunations, as indicated in
Table 4. Heilbron has also mentioned this cycle in his book. However there
are two discrepancies between the values he claims in his narrative and what



16
he would have charted in Table 4 had he continued to compute figures for J =
84. He wrote, “he took J = 84, which, with 6 jumping moons and 30
embolist[m]ic years, agrees to within 1.3 days with 1039 lunations”. By
comparing these values, we see that the discrepancies lie in the number of
embolismic years, p, and the deviation between the Julian years and whole
number of lunations, that is, N – M. By evaluating p from the rule “11J =
30p”, with J = 84, the resultant value of p is closer to 31 than 30. In addition,
the difference between N and M is 6 days, rather than the 1.3 days that he
states. However, this second discrepancy can be resolved by using values for
the lengths of average astronomical tropical year and synodic month. By these
values, the number of days in 84 years, M, is 84 × 365.2422 = 30680.3448 and
the number of days in 1039 lunations, N, is 1039 × 29.53 = 30681.67. The
difference between these two values would then be approximately 1.3 days.
Augustalis’ cycle was a significant improvement from a previously adopted 8
year cycle but was soon replaced by a more accurate 19-year cycle, the
Metonic cycle. After the Alexandrians started using the Metonic cycle, it took
some time before the Romans adopted the same cycle. Nevertheless,
Augustalis’ cycle is significant because it was through this cycle that the idea
of the epact was first introduced. The concept of “epact” is discussed in
Section 3.1.4.
2.2.2 The Metonic cycle
The Metonic cycle was discovered by a Greek mathematician, Meton. It was a
19-year lunar cycle, containing 12 common years and 7 embolismic years.
Note that a lunar year is classified as “common” if it does not have an extra,
intercalated lunation, and “embolismic” if otherwise.
In the Metonic cycle, each of the common years consisted of 12 lunations, six
of which contained 29 days and the remaining six, 30 days each. Every
embolismic year consisted of 13 lunations. Six of the embolismic years had a
similar complement of 29 and 30-day lunations as the common year, together
with an extra, intercalated full lunation of 30 days. In the last embolismic year,
the extra lunation was hollow with 29 days. This omission of a day in the extra



17
lunation was known as the “saltus lunae”, meaning “jump of the moon”. If we
refer back to Table 4, we would see why such an omission had to be made.
Compare the values for the number of days in 19 years, M, and that in 235
lunations, N. There is a 1-day difference and the “saltus lunae” is precisely
added to cover this difference.
Hence, the 12 common years contained 354 days each, and the 7 embolismic
years, 384 days each except the last, which contained 383 days. There was no
constant alignment between the start of the lunar years and the Julian years.
By convention, the first lunation of a Julian year was taken to be the first one
that ended in it. Thus the first lunation of a year might have started in
December of the previous year.
With such a composition of common and embolismic years, the cycle
contained a total of 235 lunations. 120 of them are full lunations and the
remaining 115 are hollow lunations. In turn, the number of days contained in
these 235 lunations was 6935. This was shorter than the length of 19 Julian
years only by 4.75 days. The shortfall is accounted for by the leap days that
were inserted at four-year intervals throughout the lunar cycle. Since the
original lunation could either have contained 29 or 30 days, the leap day
brought the length of this lunation to either 30 or 31 days respectively. After
the intercalation of leap days, the lunar cycle was brought into complete
harmony with the Julian calendar.
To set up a lunar table based on the Metonic cycle, not only was it necessary
to identify the composition of lunations, but it was also important to stick to
systematic rules that guided the arrangement of these lunations on the table.
The table on the next page, extracted from [8], shows how the 120 full and the
115 hollow lunations had been distributed among the 19-year cycle.



18
Table 5 Distribution of full and hollow lunations among the 19-year cycle.
Lunation
Golden
number year/cycle 1 2 3 4 5 6 7 8 9 10 11 12 13
Total
III 30 29 30 29 30 29 30 29 30 29 30 29 354
IV 30 29 30 29 30 29 30 29 30 29 30 29 354
V 30 29 30 29 30 29 30 29 30 30 29 30 29 384
VI 30 29 30 29 30 29 30 29 30 29 30 29 354
VII 30 29 30 29 30 29 30 29 30 29 30 29 354
VIII 30 29 30 30 29 30 29 30 29 30 29 30 29 384
IX 30 29 30 29 30 29 30 29 30 29 30 29 354
X 30 29 30 29 30 29 30 29 30 29 30 29 354
XI 30 30 29 30 29 30 29 30 29 30 29 30 29 384
XII 30 29 30 29 30 29 30 29 30 29 30 29 354
XIII 30 29 30 29 30 29 30 29 30 29 30 29 354
XIV 30 29 30 29 30 29 30 29 30 29 30 29 354
XV 30 29 30 29 30 29 30 29 30 29 30 29 354
XVI 30 29 30 29 30 29 30 29 30 30 29 30 29 384
XVII 30 29 30 29 30 29 30 29 30 29 30 29 354
XVIII 30 29 30 29 30 29 30 29 30 29 30 29 354
XIX 30 29 30 30 29 30 29 29 29 30 29 30 29 383
I 30 29 30 29 30 29 30 29 30 29 30 29 354
II 30 29 30 29 30 29 30 29 30 29 30 29 30 384
Note that the first lunation (of 30 days) begins (except for year III) in the previous calendar year. The lunations assigned to a golden number define a lunar year; the last column gives the number of days in each such lunar year (which does not include any leap day). The embolismic years have 13 lunations and the others, 12.
The arrangement of the lunations had been made with respect to the following
criteria:
1. The first lunation of each year should have 30 days and begin in the
previous year.
2. There should never be more than 1 golden number on the same day in the
table.
3. All the paschal lunations should contain just 29 days.
4. Full and hollow lunations should generally alternate, particularly at the
beginning and end of each year.



19
The first 3 rules were followed with no exceptions in the distribution of the
lunations. However for the last rule, there were instances in the table where
full and hollow lunations did not alternate.
2.2.3 The Great Paschal Cycle
This cycle was attributed to Victorius, Bishop of Aquataine, and sometimes
called the “Victorian cycle” or “Dionysian cycle”. Victorius had been
requested by the deacon of Rome then, Hilary, who later became Pope, to find
a way to reconcile the computation results of Easter dates of Alexandria and
Rome. By sheer computation, Victorius found that the dates of Easter Sunday,
determined according to the Alexandrian practice, would repeat on the same
days every 532 years. In fact, in any year, the days of the month would fall on
the same weekday, and the phases of the moon on the same dates, as they did
in the year 532 years ago. This 532-cycle was none other than the Great
Paschal Cycle.
There is a shorter way of finding the length of the Great Paschal Cycle. This
requires us to view the Great Paschal Cycle as having two constituent
subcycles, the Metonic cycle and the solar cycle (to be discussed in Section
3.1.3). The former has length 19 and the latter, 28. By the mathematical
principle that the length of a cycle is equal to the lowest common multiple of
the lengths of its constituent subcycles, we can then compute the length of the
Great Paschal Cycle simply by taking the lowest common multiple between 19
and 28. This gives 532, as found by Victorius.



20
Chapter 3
Determining Easter in the Julian calendar
3.1 Tools
Lunar tables provide the dates of notional new moons throughout a number of
years. Such notional moons are predicted without actual observation of the
heavens or elaborate astronomical calculations. The Metonic cycle, as
introduced in the previous chapter, governs the behaviour of these notional
moons by way of stating the length of each lunation and where the lunation is
placed. Hence good estimates of the dates of real new moons are obtained
from use of the Metonic cycle.
The traditional way of determining the date for Easter Sunday involves lunar
tables as well as golden numbers, the paschal full moon and dominical
letters/numbers. To calculate Easter Sunday without using tables, the concept
of epact is employed. The following sections would give an elaboration for
each of these underlined notions.
3.1.1 Golden number
The Metonic cycle was introduced earlier in the chapter about lunar cycles.
The length of the Metonic cycle is 19 years and the golden number is defined
to be the number that indicates the position of a particular year in the Metonic
cycle. The golden number ranges from 1 to 19, often stated in Roman
numerals I to XIX. 1 BC was deemed to be the first year of a Metonic cycle,
and thus the golden number, G, is given by the formula,
G = 1 + mod (Y, 19)
where Y is the year number in AD dating.
We note that the expression, mod (Y, 19), represents the remainder of Y after
dividing Y by 19. For example, the golden number for AD 2003 is G = 1 +
mod (2003, 19). The remainder of 2003 after dividing it by 19 is 8. Therefore
the final result for G is 9. Hence AD 2003 is the 9th year in a Metonic cycle.



21
We next give a sample of a lunar table based on the Julian calendar which is
sourced from [8]. Using it, we will study the golden numbers that appear on it
in greater detail.
Table 6
All 365 days of a year are listed in the table. The golden numbers of the years
in which a new moon is scheduled to occur on various dates are indicated
against those dates. (Ignore the letters for the time being; they will be
discussed in section 3.1.3.) Therefore, the table presents the dates of all 235
notional new moons in the Metonic cycle. For example, according to the table,
on 12 May, there is a new moon occurring on this date in the 10th year of the
Metonic cycle.
How have the golden number entries been inserted into the table? Firstly, the
new moons in the year of golden number III are entered into the table, with the
first occurring on 1 January. Let us pause to think over why such a choice had



22
been made. This is related to the choice of 1 BC as the start of a Metonic
cycle. If we are lunar table makers, there are three natural choices for a year in
AD dating to begin a Metonic cycle. The first is AD 1. It is a good choice
because it would simplify the calculations for determining golden numbers.
AD 1 would have golden number I, AD 2 would have golden number II,...
and AD 19 would have golden number XIX. The following year, AD 20,
would return to having I as the golden number. Such a relation can be
described by G = 1 + mod (Y – 1, 19) or equivalently, G = mod (Y + 1, 19) – 1,
where G is the golden number and Y is the year in AD dating. This choice
would lead to golden number II on 1 January in the lunar table. A second
choice for a year to start the Metonic cycle is AD 2. This would translate to
having golden number I on 1 January of the lunar table, making the table look
neater. Finally, 1 BC is another valid choice since it is the year that was taken
to be when Jesus Christ was born in.
Among the three choices, the third was picked. It is unknown as to what
exactly had made this arrangement seem most desirable. However we can
speculate that mathematics aside, historical, religious and political reasons
have made an equal, if not larger, influence on the decision. The simplicity of
golden number calculations and neatness of lunar tables could then have been
compromised for these other reasons. By such a choice, the notional new
moon on 1 January came to belong to year 3 of the Metonic cycle and this
fixes the rest of the construction of the lunar table.
After the golden number of 1 January is fixed as III, the subsequent golden
numbers III are filled in according to the distribution of full and hollow
lunations as listed in Table 5. For example, the second new moon in the third
year of the Metonic cycle is scheduled after a full lunation, that is, a 30-day
interval, from the first new moon. Hence, the second golden number III is
inserted at 31 January. When the counting passes into the following year, the
next golden number is introduced. For instance, after the last new moon of
year III occurs on 21 December, the next new moon would occur 29 days
later. This day coincides with 20 January of the next year and thus the new
moon entered on 20 January has golden number IV. The rest of the golden



23
numbers are entered in similar fashion. In particular, since the Metonic cycle
is a 19-year cycle, golden number I follows XIX.
Having discussed the construction of the lunar table, we highlight some
properties of the table.
Firstly, there are dates that have no golden numbers attached. We call them
“empty dates”. This phenomenon is expected because there are only 235 new
moons in the Metonic cycle, which translates to at most 235 date slots of a
365-day table being filled. Furthermore, since each date slot can only hold 1
golden number, exactly 235 date slots are required to contain all 235 new
moons. This leaves 130 “empty dates” in a common year lunar table. What
happens to the lunar table during a leap year? No doubt there are 366 days in a
leap year. Yet, since the dates marked with golden numbers indicate notional
new moons which may not correspond to the real astronomical new moons, it
is therefore a legitimate choice for deeming 29 February, the leap day, not to
carry any notional new moon at all throughout the Metonic cycle. Hence the
given lunar table with 365 date slots is sufficient to list the new moons that
occur in a certain year of the Metonic cycle, regardless of whether the year is a
common or a leap year.
Secondly, in the table, the golden numbers repeat in a fixed sequence
throughout the year; the sequence of golden numbers runs as follows: III, XI,
XIX, VIII, XVI, V, XIII, II, X, XVIII, VII, XV, XII, I, IX, XVII, VI, XIV.
This happens because the insertion of golden numbers is based on a fixed
distribution of full and hollow lunations, as listed in Table 5. Remember that
the construction of the lunar tables begins from golden number III and the next
golden number is brought in when the lunation ends in the following year.
After the last new moon of the second year in the Metonic cycle occurs on 2
December, the next new moon occurs on 1 January of the next year. In this
way, after every nineteen years, golden number III would be returned to 1
January and not to some other date. Since the distribution of the lunations
remains unchanged, that is, Table 5 is unaltered, the golden numbers of a
second Metonic cycle would be repeated identically on the same dates as



24
before. By similar argument, the golden numbers of any subsequent Metonic
cycle would also repeat on the same dates.
The third observation concerns the interval between two successive golden
numbers, and a distinct pattern in the values of the golden numbers. For each
golden number, the next golden number occurs either on the next day or on the
second day following. This gives 1 as the maximum number of “empty dates”
between any two golden numbers. Furthermore, the next golden number
would always be increased by 8, as shown in Table 7.
Table 7
G Subsequent G G Subsequent G III XI XIII II IV XII XIV III V XIII XV IV VI XIV XVI V VII XV XVII VI VIII XVI XVIII VII IX XVII XIX VIII X XVIII I IX XI XIX II X XII I
We observe that golden number XII, after adding 8, is followed by golden
number I instead of XX. This is expected since the golden numbers run from I
to XIX only. Any golden number, G, bigger than XIX would bear the golden
number, 1 + mod (G – 1, 19). Then by adding 8 into the argument of the
function, we have 1 + mod (G + 7, 19). That is, given any golden number G,
the following golden number is of value, 1 + mod (G + 7, 19).
The regular pattern of occurrence of the golden numbers can be explained by
the Octaeteris Cycle. This is a period of 8 solar years after which a new moon
occurs on the same calendar date plus 1 or 2 days. Suppose a new moon
occurs on day d. Then the next new moon listed on the table would occur on
either day d + 1 or d + 2. Respectively, this brings about either zero or one
“empty date” on the lunar table between the two golden numbers in question.



25
Let us understand the Octaeteris Cycle in greater detail. Recall that the
Metonic cycle has the property that 19 solar years contains approximately the
same number of days as 235 lunations do. Embedded within the Metonic
cycle, we find that there is an 8-year cycle that gives a fairly close
approximation too. The number of days contained in 8 solar years is 2922
days, and that in 99 lunations, assuming that the average length of a lunation is
29.5 days, is 2920.5 days. By a simple comparison, there is only an average
difference of 1.5 days. Such a difference amounts to having a subsequent new
moon occurring on either one or two days after the date of the initial new
moon. We call this the Octaeteris Cycle.
Finally, we observe that all nineteen different golden numbers could be found
in either a 29-day or 30-day period. The sequence of the numbers is
unchanged even though the length of days that accommodates the golden
numbers varies between 29 and 30. This is made possible by reducing the
number of “empty dates” in the period. The golden numbers are in turn
“squeezed” together. For instance, in certain lunations, golden number VIII is
followed immediately by XVI, yet in others, there is an “empty” date between
the two golden numbers. For later discussion, let us note that for golden
numbers XII and bigger, the subsequent golden number would always occur
without any “empty” date in between.
3.1.2 Paschal full moon
The word “paschal” is used in any context that relates to the celebration of
Easter. As highlighted earlier on, Easter is to be celebrated on the Sunday
following the paschal full moon. The paschal full moon is defined to be the
first full moon that occurs on or after the vernal equinox that is traditionally
taken to be 21 March.
Now, a full moon occurs on the 14th day from its corresponding new moon,
where the day of new moon is considered as the 1st day. Hence the paschal
new moon occurs no earlier than 13 days before 21 March; it falls on or after 8
March. Referring back to Table 6, we note that there is a new moon on 8
March in year XVI of the Metonic cycle. Moving down the table from 8



26
March, we find that the last paschal new moon of the remaining 18 years of
the Metonic cycle, falls on 5 April in year VIII. This new moon on 5 April has
its corresponding full moon on 18 April. In summary, the range of dates for a
paschal new moon is between 8 March and 5 April while that for a paschal full
moon is between 21 March and 18 April.
Taking the range of dates for paschal full moon into consideration, we now
seek to find out the range of dates possible for Easter celebration itself.
Suppose 21 March has a full moon, the earliest Sunday after 21 March would
be on 22 March. Suppose 18 April has a full moon, and it is a Sunday, then
Easter celebration would take place on 25 April, but no later. Hence Easter
Sunday can occur on any date between 22 March and 25 April.
On Table 6, dates with paschal new moons have been marked with asterisks.
Within the period of 29 days, all 19 golden numbers are represented. This
indicates that the paschal new moons of different years in the Metonic cycle
fall on different dates. If a lunar table is constructed such that it marks out the
dates of full moons, then it is possible to identify a similar 29-day period that
contains the paschal full moons. Such a period also has 19 distinct golden
numbers occurring in it.
3.1.3 Dominical letter/number
Since Easter is to be celebrated on a Sunday, there must be a way to find out
which day of the week a date falls on. Both calendar letters/numbers and
dominical letters/numbers are used to determine the day of the week. We first
discuss the former.
Seven letters, A to G, are used to specify the different days of a week. In
addition, there is also an associated set of seven numbers to the days of a
week. The letter or number corresponding to Sunday in any year is called the
“dominical letter/number” for that year. The associations are laid out clearly in
Table 8.



27
Table 8
Day of week Letter Number Sunday A 1 Monday B 2 Tuesday C 3 Wednesday D 4 Thursday E 5 Friday F 6 Saturday G 7
Imagine that the seven letters A to G are allocated sequentially to every day of
the common year: A is allocated to 1 January, B to 2 January and so on, with 7
January receiving G. Thereafter, 8 January receives A and the allocation
continues till the end of the year. In a leap year, 29 February receives the same
letter as 1 March. These letters are called “calendar letters”. Referring back to
Table 6, the letters indicated beside the golden numbers are in fact the
calendar letters.
With such an allocation in place, we then have a fixed calendar letter for the
first day of each month, regardless of whether it is in a common or leap year.
The leap day is given the same letter as that on 1 March and thus it does not
upset the sequence of the calendar letters. From January to December, the
fixed calendar letter of the first day of each month in that order is A, D, D, G,
B, E, G, C, F, A, D, and F. The letter entries in the sequence are not arbitrarily
chosen. Since January has 31 days, counting on from A on 1 January, we
arrive at D on 1 February. February has 28 or 29 days. So 1 March has
calendar letter D. Similarly, the subsequent letters are derived. Given any date,
it is then easy to count on from the first day of the particular month that the
date is in, to find out the day that the date falls on.
To work out the day via numerical calculations, we first convert the calendar
letters into calendar numbers. Let F denote the calendar number of the first
day of the month, D denote the day in the month and C denote the calendar
number of the date in question. Then,
C = 1 + mod (F + D – 2, 7)



28
The basic formula for calculating the calendar number of a date is mod (F + D
– 1, 7). However this gives 0 to 6 as the range for calendar numbers. To
augment the range to yield 1 to 7, the formula receives a “-1” within the
argument of the modulo function and a “+1” outside. For later discussion, let
us take R as the day of March, that is, R = F + D. Then the calendar number of
this day is,
C = 1 + mod (R – 2, 7).
We now turn towards the dominical letters/numbers. As defined earlier, the
dominical letter/number is a letter/number which specifies Sunday. This
letter/number changes from year to year due to two reasons.
Firstly, since each solar year comprises 52 weeks and 1 day, the last day of the
year would bear the same calendar letter as the first day of the year. In the
following year, the calendar letters/numbers would have “regressed” by one.
By this, it means that Sunday has letter G instead of A, Monday is given A
instead of B, Tuesday is given B instead of C, and so on; the allocation of
letters to the days has been shifted “backwards” by one place. Consequently,
the dominical letter regresses by one every succeeding year.
Secondly, the inserted leap day, 29 February, also causes the set of calendar
letters after this date to regress by one. Hence, in a leap year, each day has two
different calendar letters to represent it. In turn, there are also two dominical
letters in a leap year. Every Sunday before 1 March has a certain letter while
every Sunday on or after 1 March has another letter. The letter for the later
Sundays is one letter back from that for the earlier Sundays. Adding the one
letter regression brought about by the leap day and the usual one-letter
regression brought about by the yearly transition, we can thus understand why
the calendar letters for a year succeeding a leap year regresses by two.
The following example helps to illustrate the regression pattern of the calendar
letters just described.



29
Table 9
Day Calendar letters in Year 1998 1999 2000 2001 Sunday D C B, A G Å Dominical letter Monday E D C, B A Tuesday F E D, C B Wednesday G F E, D C Thursday A G F, E D Friday B A G, F E Saturday C B A, G F
The pattern of shift for every calendar letter in Table 9 is the same. For
simplicity, we just look at the dominical letter. AD 1998 has dominical letter
D. In AD 1999, the dominical letter is C, upon a regression of 1 letter. Since
AD 2000 is a leap year, there are two dominical letters; letter B prior to 1
March and A on and beyond 1 March. Finally, compared to the initial
dominical letter of AD 2000, the dominical letter of AD 2001 has regressed by
two (from B to G).
From the above, we see that the dominical letter/number is closely tied to the
number of regressions that has occurred prior to the year in question. Indeed,
we can work out the dominical letter/number N of a certain year Y from the
number of regressions Γ made by the end of year Y. Here, the Julian leap year
rule is considered.
The number of regressions Γ made by the end of year Y, starting from AD 1, is
Y – 1; AD 1 has 0 regressions. In addition, in the period between AD 1 and
year Y, there are Y 4
  regressions. Therefore, by the end of year Y, the total
number of regressions is,
Γ = Y – 1 + Y 4

1 January of AD 1 fell on a Saturday. This means that the dominical letter of
AD 1 was B and dominical number, 2. Therefore, whenever mod (Γ, 7) = 0,
the dominical number N = 2; when mod (Γ, 7) = 1, the dominical number
would have regressed by one to N = 1; and when mod (Γ, 7) = 2, the dominical
number would have further regressed to N = 7. We can in turn express the



30
dominical number N as 7 – mod (Γ – 2, 7). Substituting Γ = Y – 1 + Y 4
  , we
have ( ) ( )
7 mod 1 2, 7 7 mod 3 , 7 .
44
YY
NY Y
 
= − −+ − = − − +
    This is
equivalent to
()
7 mod 4 , 7
Y4
N Y 
= − + + 
For instance, the dominical number for AD 2003 is
()
2003
7 mod 2003 4 , 7 7 mod(2507, 7) 6
4

− ++ =− =
 .
Hence, the dominical letter for AD 2003 in the Julian calendar is F.
Equipped with the knowledge of how calendar letters and dominical letters are
worked out, we can then obtain an easy method to determine the day of the
week, W, that a particular date falls on.
Had the calendar number C of the chosen date been the same as the dominical
number N of the year from which the date is picked, this date clearly falls on a
Sunday. The difference C – N indicates the number of days that the date falls
beyond Sunday. That is, if C – N is 1, the day is a Monday. If C – N is 2, the
day is a Tuesday and so on. Such a relation can be expressed in a modulo
function, 1 + mod (C – N, 7). To avoid negative values of W, a further
adjustment to this formula yields,
W = 1 + mod (C – N + 7, 7)
Having seen an application of the dominical letters/numbers, let us now study
the dominical letters or Sunday letters closer. Dominical letters or numbers
occur in a cycle which is called the “solar cycle”. The solar cycle reaches the
point for restart when an arbitrary date returns to the same day that it fell on
during the previous cycle. Let us consider 1 January to be the date in question.
Suppose it falls on a Sunday in year x. If the calendar has no leap years, the
next earliest year in which 1 January is a Sunday, is x + 7. On a Julian
calendar, things are being complicated by the insertion of a leap day every
four years. The lowest common multiple between the lengths of the Julian leap



31
year cycle and the week is 4 × 7 = 28. Therefore, the length of a solar cycle on
a Julian calendar is 28 years.
We conclude this section with a table that shows the position of a year in the
solar cycle and its related dominical letter(s). The numbers 1 to 28 are called
“solar numbers”. It is assumed that the first year of a solar cycle should be a
leap year and that 1 January is a Monday, yielding dominical letters G and F.
Unfortunately, the justification for such a convention is not known.
Table 10 Relation between the position of a year in the solar cycle & its dominical letter
Year of the cycle Dominical letter Year of the cycle Dominical letter 1 G, F 15 C 2 E 16 B 3 D 17 A, G 4 C 18 F 5 B, A 19 E 6 G 20 D 7 F 21 C, B 8 E 22 A 9 D, C 23 G 10 B 24 F 11 A 25 E, D 12 G 26 C 13 F, E 27 B 14 D 28 A
3.1.4 Epact
The epact of a year is defined as the age of the notional moon, in terms of
days, on 1 January of the year. If a new moon occurs on 1 January, that year
has epact 0. However strictly speaking, such a definition does not apply in the
Julian calendar but rather in the Gregorian calendar that developed after. For
the Julian calendar, some sources define the epact as the age of the notional
moon on 22 March each year.
With reference to [22], the Julian epact E (with epact as the age of notional
moon on 1 Jan) may be calculated from the golden number G with the
following formula: E = 8 + mod (11 × (G – 1), 30). This agrees with the neater
formula for all values of G running from 1 to 19, as given in [8],



32
E = mod (11 × (G – 3), 30)
This formula would be the one used in the subsequent development of this
paper. We now highlight several reasons for why this formula works for
finding the epact.
As reflected in Table 6, the epact of year III in the Metonic cycle is 0. The
same result is obtained from the formula when G = 3 is substituted in it.
Furthermore, it encapsulates a characteristic property of the epact that it
increases by 11 every succeeding year. This regularity stems from the fact that
the lunar year of 354 days is shorter than the solar year by 11 days. However,
there is one exception. Recall that saltus lunae occurs during the transition
from the 19th year of the Metonic cycle to the 1st year of the next cycle. This 1
day skip in the Metonic cycle leads to a 12-day increase in the epact instead of
11 days. Since a lunation has a maximum length of 30, the value of the epact
does not exceed 30, which gives rise to the congruence modulo 30 component
in the formula. As a result, the epact lies in the range of 0 to 29. This is the
traditional way of stating epacts. In astronomical studies however, the epact is
usually given in the range 1 to 30, where the age of a new moon corresponds
to epact value 1. For the rest of this paper, the epact range should be taken as 0
to 29, unless otherwise stated.
From the formula, we can deduce that there is a unique epact for every golden
number. Once we have shown that the given formula is an injective function,
we are done.
Suppose E1 = E2 where E1 = mod (11 x (G1 – 3), 30) and E2 = mod (11 x (G2
3), 30). Then,
12
12
12
12
12
mod(11 ( 3),30) mod(11 ( 3,30)
mod(11 ( ),30) 0
mod( ,30) 0
0
GG
GG
GG
GG
GG
×− = × −
⇒ ×− =
⇒ −=
⇒− =
⇒=
since gcd(11,30) = 1
This shows that the function is injective. Hence, there is a one-to-one
correspondence between every golden number G and epact E.



33
3.2 Determining the Julian Easter Sunday
Easter Sunday may be determined with or without the use of tables. The
calculation uses the concept of epact and its link with the day of March of
paschal full moon. The following three sections provide a discussion of three
methods used in finding Easter Sunday. The first two methods make use of
tables and were put into practice in the past. The last method is proposed in [8]
as a possible computation algorithm for obtaining the date for Easter.
3.2.1 Using paschal table, dominical letter and golden number
Before the practice of using epacts became common, people used lunar tables
to determine Easter. They first extracted information from lunar tables to form
a paschal table. The sample paschal table below is extracted from [8].
Table 11



34
Table 11 contains a lot of information. However, in the most primitive way of
determining Easter, only a few items from the table are required. These
include the date, its calendar letter, and associated golden number, if any. We
note that these golden numbers in the paschal table indicate paschal full moons
and not paschal new moons. Here is a brief run-through of the steps used in
using the paschal table to determine Easter Sunday: firstly, the golden number
and dominical letter are found through the formulas as given before:
G = 1 + mod (Y, 19)
N = 7 – mod (Y + 4 + Y 4
  , 7)
Next, the line that contained the golden number is identified. From this line
downwards in the date column, the first date that has a calendar letter that
matches the dominical letter of the year in question, is Easter Sunday.
3.2.2 Using Easter tables containing epacts
There is an alternative kind of tables that were used to determine Easter. They
made use of both golden numbers and epacts. A sample has been taken from
[3] and reproduced below as Table 12.
Table 12 Excerpt from the Easter table of Dionysius
A B C DE F G 532b 1 0 4 5 Apr 11 Apr 20 533 2 11 5 25 Mar 27 Mar 16 534 3 22 6 13 Apr 16 Apr 17 535 4 3 7 2 Apr 8 Apr 20 536b 5 14 2 22 Mar 23 Mar 15 537 6 25 3 10 Apr 12 Apr 16 538 7 6 4 30 Mar 4 Apr 18 539 8 17 5 18 Apr 24 Apr 20 540b 9 28 7 7 Apr 8 Apr 15 541 10 9 1 27 Mar 31 Mar 18 542 11 20 2 15 Apr 20 Apr 19 543 12 1 3 4 Apr 5 Apr 15 544b 13 12 5 24 Mar 27 Mar 17 545 14 23 6 12 Apr 14 Apr 18 546 15 4 7 1 Apr 8 Apr 21 547 16 15 1 21 Mar 24 Mar 17 548b 17 26 3 9 Apr 12 Apr 17 549 18 7 4 29 Mar 4 Apr 20 550 19 18 5 17 Apr 24 Apr 21



35
This table is an excerpt from an Easter table which was prepared by Dionysius
Exiguus. It contains information only from AD 532 till AD 550. Let us first
familiarize ourselves with the denotations of each column and then find out
how epacts were actively used in such tables to determine Easter.
Column A lists the years in the cycle where “b” signifies leap year. The
golden numbers are given in column B. In Column C, the epact on 22 March
(original definition of the Julian epact) is given. In Heilbron’s labeling,
“Luna” is used to replace the Christian Nisan. “Luna” refers to the lunation
that contains the full moon that determines the holiday, or simply, the lunation
that contains the paschal full moon. 1 Luna refers to the day of that particular
month whose epact is 1 and 14 Luna refers to that with epact 14. That is, 14
Luna is the day on which the paschal full moon falls. Column D lists the
“ferial number” or what we refer to as “calendar number” of 24 March.
Column E provides the date for 14 Luna, column F, the date for Easter Sunday
and finally, column G, the age of the moon on Easter Sunday.
At this juncture, we highlight a potentially confusing feature of the table. At
first glance, the entries in Column C are found within the range 0 to 29. As
such, we would likely be influenced to use the traditional way of reading
epacts. That is, we take the epacts to range from 0 to 29 and that a new moon
has epact 0. However, if we inspect Columns C and E closely, we would
discover that the epacts should be taken to run from 1 to 30 instead, in order to
make sense of the dates entered for paschal full moon in Column E. We know
that the full moon occurs on the 14th day from the day of new moon. If the
epact range is 0 to 29, the full moon corresponds to epact value 13. If the
range is 1 to 30, the full moon corresponds to epact value 14. Consider the
row of entries for AD 532. Its epact on 22 March is given as 0 in Column C.
Suppose the epact range adopted is 0 to 29, the full moon should then occur on
12 April, and not 13 April as listed in Column E. Similarly, the rest of the
rows would be valid only if the epacts are read from the range 1 to 30. As
such, 22 March of AD 532 should be taken as the day before a new moon
occurred, and its “0” epact be interpreted as “30” instead.



36
How do epacts come into play in building the table? As can be inferred from
the description above, Column C leads to Column E. If the epact on 22 March
is known, then the date for 14 Luna or paschal full moon can be determined.
By knowing the day on which 24 March falls, we can then count to the date
found for 14 Luna to find out the day that it falls on. Thereafter, the date of
Easter Sunday may be obtained by counting on the dates from 14 Luna till the
first Sunday immediately after. Column F is thus established. This process of
finding the first Sunday after 14 Luna fits in with the rule that Easter is to be
celebrated on the first Sunday that follows the paschal full moon. Finally, the
difference in dates of 14 Luna and Easter Sunday gives the number of days
that the paschal full moon had waned by the time Easter is celebrated. Hence
the sum of this number and 14 gives the epact on Easter Sunday and the value
is inserted in Column G.
Let us work through an example to better appreciate the steps described above.
From the table, the epact on 22 March 546 is 4. Thus the date of 14 Luna is 10
days beyond 22 March. Counting on for 10 days from 22 March, we get 1
April as the date for 14 Luna. The “ferial number” of 24 March 546 is 7 and so
it is a Saturday. Counting on in terms of days of the week from 24 March, we
find that 1 April falls on a Sunday. Since the paschal full moon falls on a
Sunday, Easter is celebrated on the following Sunday, which is 8 April. The
age of the moon on 8 April is then 7 days older than the full moon. Its epact is
thus 14 + 7 = 21.
3.2.3 By calculation
Referring to Table 11 again, we identify a few properties concerning epacts
which enable us to calculate Easter Sunday without the use of tables.
In the paschal table, the epacts associated with each date from 21 March to 18
April are listed in column E. This is the range of dates for paschal full moons
and all 19 golden numbers are found in this range. As highlighted before, there
is a unique epact for each golden number. Therefore, there are also 19 values
for the epact. After these 19 epact values are filled up, a regular decreasing
sequence of epacts, other than a jump at 14 April, is discernible. The regularity



37
of the sequence makes it possible to allocate suitable epact values to the dates
that do not have any golden numbers attached. These epact values are
bracketed on Table 11. As a result, we have a sequence of epact values
between 21 March and 13 April that decreases steadily from 23 to 0, jumps to
29 on 14 April and begins decreasing again until 25.
Now consider the sum of the epact and the day of March of paschal full moon,
R, where R refers to the number of days that a date falls beyond 1 March,
taking 1 March as having R = 1. For instance, 3 March has R = 3 and 1 April,
being the 32nd day from 1 March, has R = 32. The last column of Table 11
indicates this sum. By observation, we see that the R values increase at the
same rate at which the E values decrease, except for a sudden break on 14
April. Therefore the sum between R and E remains constant at 44 between 21
March and 13 April, and at 74 between 14 April and 18 April. The difference
between these two constants is 30. This net increase of 30 days arises from the
jump in the values of the epact from 0 to 29 at 14 April. We also observed that
only those epacts that are greater or equal to 24 are linked to the sum 74 while
the rest of the epacts are linked to 44. This neat relation between the epact E,
and day of March R provides a quick way to determine the date of the paschal
full moon, as highlighted below.
To calculate Easter, first find the dominical letter, N, and golden number, G.
Then derive the epact, E from the golden number. The day of March, R, of the
paschal full moon can be found from the following,
R = 44 – E if E < 24
R = 74 – E if E ≥ 24
Alternatively, we can have a single formula for R. Since the paschal full moon
falls no earlier than 21 March, R has a minimum value of 21. Suppose the
paschal full moon falls on a date later than 21 March, then the difference is
accounted for by the relation mod (30 + 24 – E, 30), or equivalently, mod (54
– E, 30). The resultant formula for R is thus,
R = 21 + mod (54 – E, 30)
Using the result for R, we can find the calendar number, C, of that day by an
earlier mentioned formula,



38
C = 1 + mod (R + 2, 7)
Let d be the number of days after the paschal full moon that Easter is
celebrated. Easter Sunday thus falls on the day of March, R + d.
If C = N, then d = 7
If C < N, then d = N – C
If C > N, then d = 7 – (N – C) = 7 – N + C
In general, d = 7 – mod (C – N, 7)
Therefore, the day of March of Easter Sunday, S, is
S = R + 7 – mod (C – N, 7).
By following these steps, given any year Y in the Julian calendar, in AD
dating, we can find the date of Easter Sunday in Y. Here is an example.
If Y = 1550,
N = 7 – mod (1550 + 4 + 1550 4

  , 7) = 5.
G = 1 + mod (1550, 19) = 12
E = mod (11 × (12 – 3), 30) = 9
R = 21 + mod (54 – 9, 30) = 36
C = 1 + mod (36 + 2, 7) = 4
S = 36 + 7 – mod (4 – 5, 7) = 37.
So, Easter Sunday in AD 1550 fell on the 37th day of March, which
corresponds to 6 April.



39
Here is a flow-chart to summarize the steps taken to calculate Easter Sunday
for any year Y in AD dating.
During the time when the Julian calendar was still in use, the computation
steps given in this section no doubt could have been used to determine Easter
Sunday. However, in that age, people had still relied mainly on tables to
enable them to determine Easter Sunday. It was only after the Gregorian
calendar was adopted that determining Easter by calculation became popular.
In the next chapter, we see why the Gregorian calendar came to displace the
Julian calendar as the calendar of choice.
5. Dominical number, N
N = 7 – mod (Y + 4 + Y 4
  , 7)
Easter Sunday, S S = R + 7 – mod (C – N, 7).
1. Golden number, G G = 1 + mod (Y, 19)
2. Epact, E E = mod (11 × (G – 3), 30)
3. Day of March, R R = 21 + mod (54 – E, 30)
4. Calendar number, C C = 1 + mod (R + 2, 7)



40
Chapter 4
From Julian to Gregorian
4.1 Problems with the Julian calendar
Even though the Julian calendar was widely used throughout the Roman
Empire and later by various Christian churches, there were problems with it
that amounted to a sharp call for amendments to be made.
The average length of a solar year on the Julian calendar is 365.25 days.
However, the length of the average astronomical tropical year is about
365.2422 days. Hence, the Julian year is longer than the actual length of the
year by 0.0078 days or approximately, 0.0078 x 24 x 60 ≈ 11 minutes. What
this amounted to was the gradual shift of day of occurrence of astronomical
events, such as vernal equinox, to earlier calendar dates. By AD 1582, the
vernal equinox was observed to occur on 11 March, a whole ten days earlier
than the scheduled date for vernal equinox, 21 March.
Not only was the calendar year designed to be too long than the length of the
astronomical year, the length of the lunation used in building the lunar tables
was also longer than the actual length of a lunation. The Metonic cycle
contains in all, 19 x 365.25 days or equivalently, 6939.75 days. These days are
contained in 235 lunations. Thus each lunation has an average length of
6935.74/235 = 29.53085 days. Yet the value of the average synodic month is
about 29.53059 days. By a simple comparison, we find that the notional
lunation length has exceeded the true length by about 0.00026 days, or
approximately 22 seconds. As a result, the astronomical new moons were
observed to occur on earlier calendar dates than the ones listed in the lunar
tables. Eventually, by AD 1582, the real paschal full moon was observed to be
occurring 4 days before the notional paschal full moon.



41
Such discrepancies between the dates for astronomical phenomena and the
dates for tabulated phenomena were annoying. However, urgent calls for
reform only came along when the Catholic Church found that Easter was
gradually celebrated on dates that were increasingly removed from those
required to fulfill the original intentions of the Council of Nicaea. The Council
had ruled the celebration to take place on the first Sunday following the
paschal full moon. Yet over time, the celebration was taking place too late
because people referred to a delayed notional paschal full moon. It was
deduced that Easter would be celebrated in the seasonal summer and
eventually winter if no corrections were made to the calendar. Since Easter is a
very important event in the Christian faith, the continual slipping of dates for
its celebration was not accepted by the Catholic Church. To counter the
problem, the Church thought up and implemented amendments to the Julian
calendar. These have been brought up in “Papal Reform” of [3] and are further
elaborated upon in the next two sections.
4.2 Gregorian reforms
The reforms made to the Julian calendar were spearheaded by Pope Gregory
III and thus the new calendar was name after him as the “Gregorian calendar”.
He had recruited several astronomers, principally the Jesuit Christopher
Clavius, to come up with a solution to stop the slipping of dates for Easter
celebration. The astronomers came up with several calendar reform proposals
based on those by the astronomer and physician Luigi Lilio. Eventually,
Clavius’ proposal was implemented. Pope Gregory III issued a papal bull,
Inter Gravissimas, on 24 February 1582 and thereby established what is now
known as the Gregorian calendar reform. The reforms made may be broadly
divided into two categories: solar and lunar, and are summarized below:
• Ten days were omitted from the calendar.
• The rule for leap years was changed.
• The position of the extra day in a leap year was moved from the day
before 25 February to the day following 28 February.
• New rules for the determination of the date of Easter were adopted.



42
As highlighted before, by 1582, the vernal equinox was observed to be falling
on a date that was 10 days before the notional vernal equinox on 21 March. To
place the astronomical vernal equinox back in sync with the notional one, ten
days were dropped in one fell swoop from October 1582: 4 October 1582 was
immediately followed by 15 October 1582. The decision to drop ten days
instead of another number has been controversial.
Some argued that ten days was insufficient. With the Julian year being 0.0078
days longer than the mean tropical year, by the end of AD 1582, the vernal
equinox had slipped from that in AD 1 by 0.0078 x 1582 ≈ 12.34 days. So
why had Pope Gregory III not removed twelve days instead of ten? The reason
was because he had chosen the vernal equinox that occurred in AD 325 as the
epoch instead. This is the year when the First Council of Nicaea had convened
and established the vernal equinox as 21 March, thereby making AD 325 more
appropriate than AD 1 as the year of reference for the vernal equinox.
Between AD 325 and AD 1582, the vernal equinox had only slipped by
0.0078 x 1257 = 9.81 days, hence justifying the drop of ten days.
Yet there are still points of objection to AD 325 being a suitable epoch.
Firstly, the actual vernal equinox in AD 325 had occurred on 20 March and
not 21 March. The removal of ten days in AD 1582 had resulted in the vernal
equinox occurring mostly on 20 March and less often on 21 March, as
observations support. Thus some have argued that nine days should have been
dropped instead. There were also times when the vernal equinox was observed
to occur on 22 March. This has driven others to argue that an eleven-day
amendment is more appropriate than a ten-day one. Presumably Pope
Gregory’s astronomical advisors had considered all three possibilities and took
ten as a compromise. The fact that the omission of ten days required only the
insertion of an “X” to correct old calendars perhaps also made the choice of a
ten-day drop seem more favourable.
One last objection to AD 325 being a suitable epoch lies in that AD 325 was
one year after a leap year, AD 324. Since AD 1580 was a leap year, the year
that would have been in a more similar phase as AD 325 from AD 324, was



43
AD 1581. By such an argument, if changes were to be made in AD 1582, the
vernal equinox taken for reference should have been taken from AD 326
instead of AD 325.
Besides the omission of days, there was another solar adjustment. The rule for
leap years was changed in order to keep the calendar synchronized with the
vernal equinoxes. That is, the new rule in the calendar ensured that the real
vernal equinox occurred around the same calendar date every year. In the
Julian calendar, any year that was divisible by 4 was a leap year. The new rule
for leap years was aimed at shortening the Julian year by skipping some leap
years. It made any year divisible by 4, except years divisible by 100 but not
400, a leap year. For instance, 1700, 1800 and 1900 were not leap years but
2000 was. As a result, a period of 400 years contain 400 x 365.25 – 3 =
146097 days, giving the Gregorian year an average length of 365.2425 days.
Even though this was still longer than the mean tropical year length by 0.0003
days, or approximately 52 seconds, the vernal equinox would only lag behind
21 March by 1 day in about 1600 years.
The solar adjustments of dropping ten days from the calendar and changing
the leap year rule were complemented with lunar adjustments. Just as leap
days were dropped to shorten the calendar year, a similar scheme of dropping
days was applied to shorten the lunations.
Recall that the average notional lunation had been too long by about 1 day in
312.5 years or 8 days in 2500 years. To accomplish the adjustment, a day is
dropped from centurial years, or years divisible by 100, at intervals of 300
years for seven times and once more after another 400 years. The first drop
was made in AD 1800. In addition, between AD 325 and AD 1582, the
astronomical new moons had diverged from the notional new moons to dates
that were (1582 – 325) / 312.5 ≈ 4 days earlier. After the solar adjustment of
omitting ten days, these astronomical new moons were occurring 6 days after
the notional new moons instead. Hence the net change in the dates of notional
moons should have been a rescheduling of their dates to 6 days later. However
in the actual adjustment, the dates of notional new moons were moved on to



44
seven days later. The extra day was added to ensure that Easter Sunday will
never fall on or before the Jewish Passover, a stipulation believed to have been
made at the Council of Nicaea. In [3], it was mentioned that Gregory’s
committee justified this seven-day drop by “switching the epoch from the
Nicene Council to the time of Dionysius Exiguus, which reduced the lunar
correction from four days to three.” This may be interpreted as: instead of
taking AD 325 as the year where the astronomical new moons met the
notional new moons, Gregory’s committee used AD 532 as the reference year
instead. Therefore by AD 1582, the number of days that the astronomical new
moons had diverged from the notional ones amounted to (1582 – 532) / 312.5
≈ 3 days instead of 4.
Another reform made concerns the shift of the leap day to 29 February. It is
not clear exactly why such an adjustment was made. However here is a
possible explanation. Under the Roman dating, the leap day was the second
sixth day from the 1 March. After the reforms were made, the Roman way of
dating became obsolete and people started to count dates forward from the
start of the month instead. Naturally, rather than consider the extra day to be
inserted in the middle of February, people started to treat the last day of the
month, 29 February, to be the extra one.
The solar and lunar adjustments described above have led to alterations in the
tools used in the determination of Easter Sunday in the Gregorian calendar.
These alterations and new rules adopted for determining Easter Sunday in the
Gregorian calendar are discussed in detail in the next chapter.



45
Chapter 5
Determining Easter in the Gregorian calendar
5.1 Modifications of tools
Since the Gregorian calendar is built upon the Julian calendar, the tools used
for determining the Gregorian Easter Sunday are essentially the same ones that
are used for determining the Julian Easter Sunday. However, some of these
tools are modified before being put to use with the Gregorian calendar. The
following sections give elaborations for the modifications done to each tool.
Any concept or property that was mentioned in Section 3.1, if not brought up
in the elaborations, should be taken as applicable to the Gregorian calendar as
well.
5.1.1 Golden number and lunar table
Under the solar adjustment, certain leap years are skipped. Each time this is
done, the date of a given astronomical event is increased by one day. In
particular, the astronomical new moon occurs on a calendar day that is one day
later than otherwise expected. This leads to the need to increase the dates of
the notional moons by one and in turn, the need to move the golden numbers
in the lunar table down to a position one day later. This adjustment is known
as the solar equation, denoted by SOL. AD 1700 was the first centurial year
after AD 1582 that had its leap date skipped and thus SOL was first applied in
AD 1700.
Another amendment to the golden numbers arises from the lunar adjustment.
In order to remove eight days in 2500 years, the golden numbers are shifted up
by one day every 300 years for seven times and then once more after an
interval of 400 years. This adjustment is known as the lunar equation and is
denoted by LUN. AD 1800 was the first year in which LUN was applied.



46
The following is a timeline to indicate in which centurial years SOL and LUN
are applied after AD 1582. Each Y’ marks a centurial year with the 0’s
omitted. For instance, AD 1600 is expressed as 16 on the timeline. A “ √ ”
above centurial year Y’ along the row “SOL” or “LUN” means that SOL or
LUN is applied in that centurial year, respectively.
SOL √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ √ LUN √ √ √ √ √ √ √ √ √
16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43
Centurial year, Y’ in AD dating
Even though SOL and LUN are applied only in centurial years, the shifts in
the golden numbers induced by them are cumulative over every year. SOL and
LUN shift the golden numbers in opposing directions; the former shifts them
down, the latter shifts them up. During centurial years, there are four
possibilities in the way that golden numbers are shifted in the lunar tables,
namely:
1. Both SOL and LUN are not applied. → Golden numbers are not shifted.
2. Both SOL and LUN are applied. → Since their effects cancel each other
out, the golden numbers are not shifted.
3. SOL is applied, but not LUN. → Golden numbers are shifted down to a
day later.
4. LUN is applied, but not SOL. → Golden numbers are shifted up to a day
earlier.
SOL is applied more often than LUN and thus there is a progressive
downward drift in the golden numbers. Let us work out the number of
centuries required before the sequence of shifts repeats itself. SOL is applied 3
times every 4 centuries; LUN is applied 8 times every 25 centuries. Once
more, we apply the principle: the length of a cycle is equivalent to the lowest
common multiple of the lengths of its constituent cycles. The sequence of
shifts forms a cycle with its constituent cycles being that of SOL and LUN.
The lowest common multiple of the lengths of the SOL cycle and LUN cycle
is 4 × 25 = 100. Therefore, the sequence of shifts repeats after every 100
centuries.



47
Over 100 centuries, there are 25 four-century periods and so SOL is applied 25
× 3 = 75 times. In addition, within these 100 centuries, there are 4 twenty-five
century periods. Thus, LUN is applied 4 x 8 = 32 times. The net shift in the
golden numbers over these 100 centuries is therefore 75 – 32 = 43 days
downward in the lunar table.
Depending on whether SOL or LUN is applied, in different years, a particular
golden number could occur on different dates. It is not practical to mark the
family of dates of each golden number into a single lunar table, such as the
one shown as Table 6. Therefore, for the Gregorian calendar, multiple lunar
tables have been constructed based on the Julian lunar table.
As a result of the seven-day increase in the dates of notional new moons, each
golden number in the Julian lunar table was shifted to a position seven days
later. This gave an initial Gregorian lunar table which was valid from AD
1582 to AD 1699. In AD 1700, SOL was applied but not LUN. Therefore, the
golden numbers in the lunar tables were shifted down one more day. In
subsequent centurial years, the golden numbers are shifted up and down
according to the dictates of SOL and LUN.
How long does it take for the golden numbers in the lunar tables to return to
their position after the seven-line drop in AD 1582 before the sequence of
shifts begins again? This requires us to find out how many centuries it takes
before the downward shift of golden numbers amounts to 30 days. 30 days is
considered because it is the period that always contains all the 19 different
golden numbers. Therefore, after a downward shift that amounts to 30 days,
the dates covered by the initial sequence of golden numbers will be covered
again by the exact same sequence of golden numbers.
Even though we know that that there is a 43-day shift every 100 centuries, it is
not possible to work out the number of centuries a 30-day shift requires by
using a direct ratio method. This is because the shift does not occur at regular
intervals. Instead, we have to break the calculation up into several
components. Firstly, compute the number of days by which the dates of



48
notional new moons are increased by SOL after x centurial years have passed.
Secondly, compute the number of days by which the dates of notional new
moons are decreased by LUN after x centurial years have passed. Lastly, find
x such that the difference of days shifted due to SOL and LUN is 30. Here is a
demonstration of the computation process; x is arbitrarily chosen at each stage:
Table 13
x centurial years after AD 1582 No. of days shifted by SOL LUN
Net shift
25 Down by 18 Up by 8 Down by 11 50 Down by 37 Up by 16 Down by 21 60 Down by 45 Up by 19 Down by 26 70 Down by 52 Up by 22 Down by 30
Note: The first centurial year after AD 1582 is AD 1600. SOL was first applied in AD1700; LUN was first applied in AD 1800.
From the above, we see that it takes 70 centurial years to elapse after AD 1582
before the golden numbers would return to their original positions in AD
1582. That is, the golden numbers between AD 8500 and AD 8599 will be in
the same positions as those in AD 1582 after the seven-line drop.
We could have formulae to compute the number of days that the golden
numbers are shifted by SOL and LUN. These are discussed in the following.
Let SOL* denote the number of days by which the dates of the notional new
moons must be increased on account of the decrease in the average length of
the calendar year for year, Y.
Let LUN* denote the number of days by which the dates of the notional new
moons must be decreased on account of the lunar adjustment for year, Y.
We first work out a formula for SOL*.
SOL* depends on the number of centurial years passed since AD 1600, that is,
it depends on 16.
100
Y  −
  SOL is applied 3 times in every four centuries,
starting from AD 1700. That is, 3 leap days are dropped in every four
centuries. By year Y, the number of complete four-century periods is



49
()
16
100
4
Y

 −





and hence the number of leap days dropped over all these
four-century periods is ( )
16
100
3.
4
Y

 −


× 


After all these complete four
century periods are considered, there may also be up to three centurial years
remaining before year Y is reached. The number of leap days dropped in this
remainder is equivalent to ( )
mod 16, 4 .
100
Y  −
  Therefore, the total number
of leap days dropped by the end of year Y is,
( )( )
( )( ) ( )
()
16
100
* 3 mod 16, 4
100
4
16 16
100 100
3 16 4
100
44
16
100
16
100 4
100
16 4
100 4
100 100 4
Y Y
SOL
YY Y
Y Y
Y Y
Y Y

 −

  
=× + −
  


 
 
−−
 
 

=× + − −×
 

 
 

 −



= − − 
  






= −− +
  


 



=−
  
12.
 −
 
We next work out a formula for LUN*.
LUN* depends on the number of centurial years passed since AD 1800, that
is, it depends on 18.
100
Y  −
  LUN is applied 8 times in every 25 centuries,
starting from AD 1800. Beginning the count from AD 1800, the number of
complete twenty-five-century periods that year Y contains is ( )
18
100
25
Y

 −





.



50
Hence the number of days dropped over all these twenty-five-century periods
is ( )
18
100
8.
25
Y

 −


× 


Let Z denote the number of centurial years that has
passed by the end of year Y, in the current twenty-five-century cycle of year Y.
Z is given by ( )
mod 18, 25
100
Y  −
  and thus Z can range from 0 to 24. Recall
that LUN is applied at 3-century intervals for the first 21 centuries of the
cycle, and its last application is made after another 4 centuries. If Z < 24, then
Z 3
  days are removed; if Z = 24, then 7 days are removed. However, Z 3

leads to 8 days being omitted when Z = 24. To fix this expression up to
describe the behaviour of LUN, we make use of .
24
Z 
  Note that 1
24
Z  =

if Z = 24; 0
24
Z  =
  if Z < 24. Hence the number of days omitted from the
current 25-century cycle of Y may be expressed as .
3 24
ZZ
  
− 
  To account
for the day omitted in AD 1800, 1 is added to the total lunar correction.
Therefore, the total number of days dropped by the end of year Y is,
()
18
100
* 1 8 3 24
25
Y
ZZ
LUN

 −

   
=+× + −
  



where ( )
mod 18, 25 .
100
Y
Z 
=−

There is a simpler formula for LUN*. Consider the following:
()
17
100
15
100 25
3
Y Y


 −



 − −












where 18.
100
Y  ≥

We check that this exactly describes LUN*. When 18,
100
Y  =
  the formula
gives a value of 1. This corresponds to the fact that LUN is first applied in AD



51
1800 and 1 day is dropped then. The value given by the formula increases by 1
every time 100
Y 
  increases by 3, which corresponds to the fact that LUN is
applied at intervals of 300 years. However, when 42,
100
Y  =
  we have
17
100 1,
25
Y

 −

 =



thereby causing the value of the formula to remain
constant at 8 at this stage. The value only increases by 1 more when 100
Y 

becomes 43. Thereafter, the value increases gradually by 1 and becomes
constant again when 68.
100
Y  =
  This pattern of increases describes the
intervals at which LUN is applied: once every 300 years for the first 2100
years of a twenty-five-century cycle, and another time after 400 years. In the
first twenty-five-century cycle beginning at AD 1800, a day each is dropped in
the years AD 2100, AD 2400, AD 2700, AD 3000, AD3300, AD 3600, AD
3900 and AD 4300. The term
17
100 25
Y

 −





in the formula serves to
postpone the one-day drop from AD 4200 (the 24th year in the first twenty
five-century cycle from AD 1800) to AD 4300, from AD 6700 (the 24th year
in the second twenty-five-century cycle from AD 1800) to AD 6800 etc. As a
result, we conclude that the refined formula corresponds exactly to the number
of days omitted by the end of year Y, due to the lunar adjustment. That is,
()
17
100
15
100 25
*3
Y Y
LUN


 −
  

 − −






= 





where 18.
100
Y  ≥

Using the formulae for SOL* and LUN*, we can easily verify that when
85,
100
Y  =
  SOL* – LUN* gives 30, as found by the computation earlier.



52
Mentioned earlier, multiple lunar tables are drawn up for the Gregorian
calendar. How many such tables are required? Since the golden numbers are
repeated in their original positions after a net downward shift of 30 days, we
know that there are a total of 30 different patterns of distribution of golden
numbers that have to be indicated on the lunar tables. Therefore, 30 different
lunar tables are constructed for the Gregorian calendar. These tables are
identified by index letters have a one-to-one correspondence to thirty index
numbers, 0 to 29. These index numbers are in turn obtained from mod (SOL*
– LUN*, 30), giving the number of days by which the golden numbers have
been shifted down.
5.1.2 Dominical letter/number
The dominical letter/number in a year regresses by 1 from that in the previous
year and by 2 if the previous year is a leap year. In the Gregorian calendar,
there is still a strong link between the number of regressions, Γ, made by the
end of year Y and the dominical letter/number, N, of year Y. However, the new
leap year rule adopted in the Gregorian calendar alters the number of
regressions that occur in a given period of time. Hence the formulae for Γ and
N derived in Section 3.1.3 have to be modified to cater to the Gregorian
calendar. The following discussion provides a derivation of these new
formulae.
AD 1 has 0 regressions and by the end of year Y, starting the count of years
from AD 1, the number of regressions Γ made is Y – 1. In the Gregorian
calendar, a year is a leap year if it is divisible by 4 unless it is a centurial year
not divisible by 400. Thus, between AD 1 and year Y, there are
4 100 400
YY Y
  
 − +
      leap years. Then by the end of year Y, the total
number of regressions is,
Γ = Y – 1 + 4 100 400
YY Y
  
 − +
   
By the Gregorian calendar, 1 January AD 1 is a Monday. Thus the dominical
letter of AD 1 was G and dominical number, 7. Therefore, when mod (Γ, 7) =
0, the dominical number N = 7; when mod (Γ, 7) = 1, the dominical number



53
would have regressed by one to N = 6; and so on. In this way, we can express
the dominical number N as 7 – mod (Γ, 7). Substituting Γ = Y – 1 +
4 100 400
YY Y
  
 − +
      , we have
N = 7 – mod (Y – 1 + 4 100 400
YY Y
  
 − +
      , 7)
For instance, the dominical number for AD 2003 is
()
2003 2003 2003
7 mod 2003 1 , 7
4 100 400
7 mod(2487, 7)
5
N    
= − −+ − +
   
=−
=
Therefore, the dominical letter for AD 2003 in the Gregorian calendar is E.
To determine the day of the week that a particular date falls on in the
Gregorian calendar, the same formula given in Section 3.1.3 may be used but
with one exception: N is obtained from the new formula given above.
What is the length of the solar cycle in the Gregorian calendar? We know that
the Gregorian leap year cycle is 400 years. However, contrary to the Julian
case, the length of the solar cycle in the Gregorian calendar is not equivalent
to the lowest common multiple of 400 and 7. Instead, its length is simply 400
years. By the end of 400 years, the number of leap years skipped during this
period is 3. This makes the number of days contained in a period of 400
Gregorian years to be 146 097, which is a figure divisible by 7. Thus an
arbitrary date bearing a particular dominical (or calendar) letter would return
to bear the same dominical (or calendar) letter after every 400 years.
5.1.3 Paschal full moon
Since there are 30 different lunar tables in the Gregorian calendar, 30 different
paschal tables may be extracted from them. In determining which date that the
paschal full moon falls on in a certain year, it is important to use the paschal
table that has the same index number as that of the lunar table applicable to
that year.



54
In general, the paschal full moon dates fall in the range 21 March to 18 April,
however there are exceptions in the Gregorian paschal lunar tables. This adds
an additional consideration in the calculation of Easter Sunday in the
Gregorian calendar. This issue is further discussed in Section 5.2.
5.1.4 Epact
In the Gregorian lunar tables, the solar equation, SOL, and lunar equation,
LUN, come into play in shifting the golden numbers down and up
respectively. Recall that the epact of a year is the age of the notional moon on
1 January of that year, taking the epact of a new moon as 0. As such, the value
of the epact is directly linked to when a new moon is scheduled.
Let us consider only the first lunation of the year. This refers to the lunation
that first ends in that year and may begin from the previous year. If SOL is
applied, golden numbers are shifted down by 1 day. Hence, the new moon for
this first lunation would occur 1 day later than what would have been the
scheduled date had SOL not been applied. As a result, the age of the moon on
1 January is reduced by 1 day. That is, when SOL is applied once, the epact is
decreased by 1. If LUN is applied, the golden numbers are shifted up by 1 day
on the lunar tables. Hence the new moon for the first lunation would occur 1
day earlier than the original date. This leads to the age of the moon on 1
January to increase by 1. That is, when LUN is applied once, the epact is
increased by 1.
The table on the next page has been extracted from [3] and would show how
SOL and LUN affect epacts over a millennium in the Gregorian calendar.



55
Table 14 Epacts through the third millennium
Cycle Epacts valid for 100 years beginning in year (Golden number)
1500, 1600
1700, 1800
1900, 2000, 2100
2200, 2400
2300, 2500
2600, 2700, 2800
2900, 3000
1 1 0 (30) 29 28 27 26 25 2 12 11 10 9 8 7 6 3 23 22 21 20 19 18 17 4 4 3 2 1 0 (30) 29 28 5 15 14 13 12 11 10 9 6 26 25 24 23 22 21 20 7 7654321 8 18 17 16 15 14 13 12 9 29 28 27 26 25 24 23 10 10 9 8 7 6 5 4 11 21 20 19 18 17 16 15 12 2 1 0 (30) 29 28 27 26 13 13 12 11 10 9 8 7 14 24 23 22 21 20 19 18 15 5 4 3 2 1 0 (30) 29 16 16 15 14 13 12 11 10 17 27 26 25 24 23 22 21 18 8 7 6 15 4 3 2 19 19 18 17 26 15 14 13
Table 14 lists the values of epact for every year in the third millennium. An
epact in row n is the epact of an nth year in the Metonic cycle. Recall that
there is a unique epact for every golden number. Since the rows correspond to
the 19 golden numbers, there are 19 different epact values found in each
column. In this table, the epacts range from 1 to 30, with epact of value 30
being listed as “0 (30)” on the table. The epact between succeeding years
increases by 11, as can be readily observed from the sequence of epacts in
each column. This is because the lunar year is 11 days shorter than the solar
year. The exception arises when we consider the epact change from the 19th
year to the 1st year of the Metonic cycle. The saltus lunae takes place at this
juncture, thereby increasing the epact by 12 instead of 11. So far, the features
described are familiar ones which apply also to Julian epacts. What is peculiar
to Gregorian epacts is this: at every turn of a century, there is a possibility for
the sequence of epacts to change.



56
The epact values in a column are valid for 100 years beginning in the centurial
year that is stated at the top of the column. The sequence of epacts runs
through the column from the top to the bottom and back to the top again. After
100 years, whether the sequence of epacts remains within the existing column
or switches to that in the next column depends on whether SOL or LUN has
been applied in the centurial year in question. For example, in the first column,
the epacts run in the sequence: 1, 12, 23, 4, 15, 26, 7, 18, 29, 10, 21, 2, 13, 24,
5, 16, 27, 8, and 19. This sequence is valid from AD 1500 to AD 1599, and
again from AD 1600 to AD 1699. No switch of columns occurs at AD 1600
because both SOL and LUN are not applied in that centurial year. However,
SOL is applied in AD 1700 and thus epact values are reduced by 1 in the
following century. For example, after the last entry “19” in the first column of
epacts, had SOL not been applied in AD 1700, the 1st entry for AD 1700
would be mod (19 + 12, 30) = mod (31, 30) = 1. However SOL reduces the
epact by 1. Hence a new sequence of epacts beginning with “0 (30)” is
generated for 100 years beginning at AD 1700. The sequence of epacts thus
switches from running through the first column to running through the second
column. We observe that the entries in the second column are indeed smaller
by 1 when compared to the epacts in the first column within their respective
rows. The second column holds true for years from AD 1700 to AD 1899. No
change occurs at AD 1800 because both SOL and LUN are applied then and
their effects cancel out, thereby not shifting the epacts at all. At the onset of
AD 1900, there is a reduction of epact values by 1 again for the 100 years
beginning from then. This is the result of applying SOL in AD 1900.
As we progress through the centurial years 1500, 1600, 1700, 1800,... , the
columns are read from left to right in general. The first change comes about at
AD 2400. This is the centurial year where there is an increase in the epacts by
1 because only LUN is applied but not SOL. After AD 2399, we read the
columns from right (5th column) to left (4th column) instead. By comparison,
the epacts in the fourth column are bigger than those in the fifth column by 1,
as expected. By interpreting the rest of the table in the same way, we would
see how SOL and LUN influence epact values over a period of 1000 years.



57
Having seen how SOL and LUN affect Gregorian epacts on a table, we now
focus on studying how epacts are manipulated when used in the computation
of Easter Sunday.
From Section 3.4, we recognize that one of the key steps in the computation
makes use of the sum of the day of March of a paschal full moon and the epact
for the corresponding year. This sum either added up to 44 or 74 according to
the golden number. Suppose the golden numbers have drifted downwards by x
days due to SOL and LUN. This results in an epact which is x days smaller.
Yet at the same time, the day of March of any golden number in the lunar
table increases by x. By considering the action of SOL and LUN on the epact
and day of March themselves, the above explanation suggests that the sum
remains constant at either 44 or 74. From knowing the Gregorian epact, the
date of the paschal new moon, and in turn paschal full moon, may then be
determined easily. Unfortunately, there are exceptions to the sum being 44 or
74. Such exceptions stem from a problem in the paschal tables. The problem is
discussed in the next section.
5.2 Gregorian paschal lunar table
5.2.1 Problem
In the Julian paschal table, the paschal new moon occurs between 8 March and
5 April. All 19 golden numbers can be found within this range of dates.
However this range is not kept in all the newly constructed Gregorian paschal
tables. In some, only 18 of the golden numbers fell within this range of 29
days while the last golden number fell on the 30th day instead, that is, on 6
April.
Why has such an anomaly occurred? Recall the paschal lunation is the
lunation that contains the paschal new moon. The Julian lunar table was set up
with a condition that the paschal lunation contained only 29 days. Therefore
all the 19 paschal new moons, and in turn, the 19 golden numbers, can be
found within a period of 29 days. However, the lunation preceding the paschal
lunation is 30 days long. This means that two consecutive identical golden
numbers, with the latter corresponding to the paschal new moon, are 30 days



58
apart. The 30-day period before the period 8 March till 5 April therefore also
contains the full set of 19 golden numbers in the exact same sequence as that
in the latter period. Comparing the lengths of these 2 periods, we find that
there is an additional “empty date” in the 30-day period.
With the applications of SOL and LUN, the golden numbers are progressively
shifted down in the lunar table. We thus have a situation of 19 golden
numbers, which were originally spread over a period of 30 days, having to be
squeezed into a period of 29 days. When the downward shift occurs, either an
“empty date” or a golden number is being shifted out of the period between 8
March and 5 April into 6 April. Simultaneously, either an “empty date” or a
golden number from the previous 30-day period is being shifted into the gap
created on 8 March. The anomaly highlighted at the beginning of this section
occurs when the item that was shifted out of the period 8 March to 5 April was
a golden number but that which was shifted into the gap on 8 March was an
“empty date”. In such a case, the period 8 March to 5 April would only
contain 18 golden numbers, with the last one occurring on 6 April.
Here is a schematic diagram to illustrate how the anomaly has been created:
Legend: golden no. “empty date” golden no./ “empty date”
As the diagram suggests, the first row of entries is shifted to the right to obtain
the second row of entries. This corresponds to a downward shift of the golden
numbers in the Gregorian lunar table. In particular, an empty date is shifted
into the 29-day period as a substitution for the golden number that is shifted
out of the same period. Hence only 18 golden numbers remain in the period 8
March till 5 April while the 19th golden number falls on 6 April.
GE ?



59
It is not obvious why the missing golden number invariably lands on 6 April
and not any later. The underlying reason for this is that the number of “empty
dates” in the lunar table is at most 1 day long. We can also view it as: every
“empty date” is always sandwiched between 2 golden numbers. After an
empty date is shifted into the 29-day period on 8 March in the first round, the
subsequent entry to be shifted into the period in the second round is certainly a
golden number. This new entry either substitutes an “empty date” or a golden
number that was shifted out of the 29-day period during the second round. If
the new entry replaces an “empty date”, the end result is that the 29-day period
resumes its feature of containing all the paschal new moons. Equivalently, all
19 golden numbers would be returned into the range 8 March till 5 April after
this second round of shifts. If the new entry replaces a golden number, the end
result is that the 29-day period continues to contain only 18 golden numbers
and the missing golden number still falls on 6 April. Note however that the
golden number that is missing from the 29-day period after the second round
of shifts is different from the original golden number that was missing after
the first round. Recall that we are shifting golden numbers from a 30-day
period into a 29-day period. The original golden number had been omitted
because its earlier identical golden number had been blocked from entering the
range at 8 March by the extra day slot. After the second round of shifts, the
new golden number being shifted into the 29-day period is identical to the
original missing golden number. Hence, we conclude that the new missing
golden number after the second round of shifts is different from the original.
Nonetheless, Pope Gregory III and Christopher Clavius wanted to keep the
range of dates for the paschal new moon to be within 8 March and 5 April
across all the Gregorian lunar tables. They wanted to stick to the traditional
29-day period for which Easter celebration had been held in, for the past
thousand years. To achieve this, they made further adjustments which are
discussed in the next section.
5.2.2 Adjustments
To maintain the dates 8 March till 5 April as the range for the paschal new
moons, whenever a golden number fell out of this range of dates into 6 April,



60
it was shifted back up into 5 April. However this was not always possible
because 5 April is not an “empty date”. In making adjustments to the table,
Pope Gregory III and Christopher Clavius were not prepared to forgo another
condition which the lunar tables had been designed to satisfy: no date can bear
more than 1 golden number. Let us find out when it is possible to shift the
golden number into 5 April, when not, and what additional adjustment is then
required to deal with the second case.
In Section 3.1.1, it was mentioned that for golden numbers XII and bigger, the
subsequent golden number always occurred without any “empty” date in
between. These subsequent golden numbers are in the range I to VIII. Should
any of these numbers between I to VIII fall on 6 April, there would certainly
be another golden number on 5 April from the range XII to XIX. Therefore,
we can divide the missing golden numbers that land on 6 April into two
classes: the first class contains golden numbers between IX and XIX, and the
second class contains golden numbers between I to VIII.
When golden numbers between IX and XIX fell on 6 April, one shift is
required to shift them back to 5 April. When the golden numbers in the range I
to VIII fell on 6 April, the golden numbers in the range XII to XIX fell on 5
April. Therefore two shifts are needed to complete the adjustment: the golden
number on 5 April was shifted to 4 April and that on 6 April was shifted to 5
April. We note that for the second case, 4 April would always be an “empty
date” and therefore can accommodate the golden number shifted up from 5
April.
To understand why 4 April is invariably an “empty date”, we revert to
inspection of the Julian lunar table from which the Gregorian lunar tables are
derived. Recall that due to the influence of the solar equation (SOL) and lunar
equation (LUN), there is a net downward drift in the golden numbers in the
original Julian lunar table. A total of 30 different Gregorian lunar tables are
then derived to account for the 30 possible distributions of golden numbers.
These are then cycled through for use over the years. From the Julian lunar
table, the golden numbers, which are shifted into the period 8 March till 5



61
April, come from the period between 6 February and 7 March. There are no
strings of golden numbers which are longer than two within this period.
Therefore, among the 30 generated lunar tables, there is no string of golden
numbers exceeding two in length within the period between 8 March and 5
April. Equivalently, the 30 paschal lunar tables would only have strings of
golden numbers of length at most two. Hence whenever a golden number falls
on 6 April in the paschal lunar table, and another that falls on 5 April, the date
4 April would always be an “empty date”.
5.2.3 Effect of the adjustments on Gregorian epact
We have seen how the problem of the paschal lunar tables is solved through an
occasional adjustment of the golden numbers. However, such a solution has
led to cases where the sum of the day of March of the paschal full moon and
the epact for the corresponding year does not add up to either 44 or 74. This
section addresses these exceptions.
When a paschal new moon falls outside the period 8 March till 5 April into 6
April, the corresponding paschal full moon occurs on 19 April. 19 April is the
50th day of March and thus for that year, the epact is 74 – 50 = 24. However,
by rule of the adjustments to the golden numbers on a paschal lunar table as
given in the previous section, this paschal new moon must be shifted back by
one day to 5 April. The paschal full moon is thus pushed back to 18 April, the
49th day of March. This results in the sum of epact and ‘Day of March’ of
paschal full moon for that year to be 24 + 49 = 73 instead of the usual 74. To
patch up the shortfall, the epact for that year is increased from 24 to 25.
In addition, if the golden number being pushed back from 6 April to 5 April is
between golden numbers I to VIII, there is a golden number in the range XI to
XIX that falls on 5 April. Correspondingly, there is a paschal full moon from
the 9th to 19th years of the Metonic cycle occurring on 18 April, the 49th day of
March. The epact for this year is thus 74 – 49 = 25. By rule of the adjustments
again, the golden number on 5 April is shifted back to 4 April so that 5 April
can accommodate the golden number shifted up from 6 April. Thus the
paschal full moon on 18 April is shifted to 17 April, the 48th day of March.



62
After the adjustment, the sum of epact and day of March of paschal full moon
for that year becomes 25 + 48 = 73. To change this sum back to 74, whenever
a golden number between XII and XIX occurs with a calculated epact of 25,
the epact is increased to 26 instead.
Here is a summary of the two rules, henceforth to be referred to as “Clavius’
adjustments”, by which the calculated Gregorian epacts are adjusted:
1. If the calculated epact is 24, increase it to 25;
2. If the golden number is greater or equal than XII and the calculated epact
is 25, increase it to 26.
5.3 Determining the Gregorian Easter Sunday by calculation
After the Gregorian calendar was adopted, the primary way of determining the
date for Easter celebration involved calculations and not tables. The flow of
steps used is very similar to that in the Julian calendar. Comparing both
schemes of calculations, the main difference lies in how the final epact values
are derived. We first give a detailed elaboration of how the Gregorian epacts
are found before summarizing the calculation steps of Gregorian Easter via a
flow chart.
With the seven line drop of the golden numbers in the lunar tables, the Julian
epact formula, E = mod (11 x (G – 3), 30) is modified to, E = mod (11 x (G
3) – 7, 30). The net downward drift of the golden numbers is given by mod
(SOL* – LUN*, 30). Note that SOL* denotes the number of days by which the
dates of the notional new moons is increased on account of the decrease in the
average length of the calendar year for year Y, and LUN* denotes the number
of days by which the dates of the notional new moons must be decreased on
account of the lunar adjustment for year Y. With the downward drift, the epact
value is reduced by the same amount, mod (SOL* – LUN*, 30). Therefore, the
formula for the Gregorian epact after accounting for both solar and lunar
adjustments is given by,
() ()
mod 11 ( 3) 7,30 mod( * *,30)
mod 11 40 ( * *),30 .
E G SOL LUN
G SOL LUN
= × −− − −
= ×− − −



63
Substituting the formulae for SOL* and LUN* accordingly into the above, we
get,
()
17
100
15
100 25 100
mod 11 40 12 ,30
100 4 3
100 100 100
mod 11 28
100 4
Y Y
Y Y
EG
Y Y
Y Y
G




 −





 − −











  



= ×− − − − −


  


















 −






= ×− + − +
  


()
()
17
25
5 ,30
3
17
100 100 25 100
mod 11 33 ,30
100 4 3
Y Y
Y Y
G



−










 −















 −




 −









  


= ×− + − +


  












To ensure that the argument of the above modulo function is not negative, a
multiple of 30 is added into the argument to yield,
()
17
100 100 25 100
mod 57 11 ,30
100 4 3
Y Y
Y Y
EG



 −

  

 −









  


= +×− + +


  












However, this is not the final formula for the Gregorian epact; Clavius’
adjustments have to been fitted in. Here are two possible formulae for
calculating the value of the correction.



64
Let V denote the correction to be made in the epact as a result of Clavius’
adjustments. Consider,
()
24 25 12 24 25
G
EE EE
V     
 
= − +× −
 
    
where E is the epact value calculated by the earlier formula, and G is the
golden number for the year in concern.
V attains 1 either when E = 24, or E = 25 and G ≥ 12; V is 0 otherwise. Hence
V may be added to E, or to achieve the same effect, subtracted from the ‘Day
of March’ of the paschal full moon to give Efinal where Efinal indicates the final
epact value after considering Clavius’ adjustments.
Consider an alternative formula:
1 11
' 319
GU
V −+ ×

= 

where U = mod (53 – E, 30).
V ' attains 1 only when
G −1+11×U ≥ 319 ⇒ G −1 ≥ 319 −11×U ⇒ G −1 ≥ 11(29 −U ).
This relation holds in two cases. Firstly, when E = 24, we have U = 29 and
thus the above relation holds for all values of G. Secondly, when E = 25, we
have U = 28 and the above relation holds for G ≥ 12. Therefore, V ' may be
used in place of V to account for Clavius’ adjustments.
We present all the steps involved in the computation of the Gregorian Easter
Sunday in a flow chart next page.



65
In this flow chart, the first formula for Clavius’ adjustments, V, has been used
and it is added to E to yield Efinal instead of being subtracted from R. By
following these steps, we obtain the date for the Gregorian Easter Sunday for
any year Y in AD dating.
Easter Sunday, S S = R + 7 – mod (C – N, 7).
1. Golden number, G G = 1 + mod (Y, 19)
2. Epact, E
()
17
100 100 25 100
mod 57 11 ,30
100 4 3
Y Y
Y Y
EG



 −




 −








  

= +×− + +













5. Day of March, R R = 21 + mod (54 – Efinal, 30)
6. Calendar number, C C = 1 + mod (R + 2, 7)
7. Dominical number, N
N = 7 – mod (Y – 1 + 4 100 400
YY Y
  
 − +
      , 7)
4. Epact after Clavius’ adjustments, Efinal
Efinal = E + V
3. Clavius’ adjustments, V
()
24 25 12 24 25
G
EE EE
V     
 
= − +× −
 
    



66
Chapter 6
Easter algorithms
6.1 A selection of Easter algorithms
In chapters 3 and 5, we have described procedures for finding the date of
Easter Sunday by means of tables and calculations in both Julian and
Gregorian calendars. We note that the given algorithms are but a few which
have been constructed based on the rules found in Easter tables. In this
section, we furnish readers with a couple more examples of tables that people
have used to determine Easter. Then, a review of several other algorithms
would be provided.
The tables have been taken from the Book of Common Prayer and the source
for each algorithm is mentioned explicitly in its respective section. To honour
the sources of the algorithms, minimal changes have been made to their
manner of presentation as they are adapted into this supplement. As such,
there are differences between the notations used in the supplement so far, and
those that are to appear in the following algorithms. These notation differences
would be clarified accordingly.
6.1.1 Easter tables in the Book of Common Prayer
The first edition of the Book of Common Prayer was produced in AD 1549
and since then, the book has exerted major influence on the religious lives of
many. The AD 1549 edition of the prayer book was in use only for three years,
until extensive revision in AD 1552. However, much of its tradition and
language remains in the prayer books of today. See Appendix A for a
translation of the contents page of the second edition of the book to get a sense
of the sort of issues addressed in this book. Tables for determining the date of
Easter Sunday can be found in The Book of Common Prayer. We next
reproduce these tables from the AD 1662 edition of the Book of Common
Prayer found in [14].



67
Table 15
A Table to Find Easter-Day,
From the Present Time till the Year 2199 Inclusive According to the Foregoing Calendar.
Golden Number.
Days of the Month.
Sunday Letters.
March 21 C
XIV. ” 22 D
III. ” 23 E
” 24 F
XI. ” 25 G
” 26 A
XIX. ” 27 B
VIII. ” 28 C
” 29 D
XVI. ” 30 E
V. ” 31 F
April 1 G
XIII. ” 2 A
II. ” 3 B
” 4C
X. ” 5 D
” 6E
XVIII. ” 7 F
VII. ” 8 G
” 9A
XV. ” 10 B
IV. ” 11 C
” 12 D
XII. ” 13 E
I. ” 14 F
” 15 G
IX. ” 16 A
XVII. ” 17 B
VI. ” 18 C
” 19 D
” 20 E
” 21 F
” 22 G
HIS Table contains so much of the Calendar as is necessary for the determining of Easter; to find which, look for the Golden Number of the year in the first Column of the Table, against which stands the day of the Pascal Full Moon; then look in the third Column for the Sunday Letter, next after the day of the Full Moon, and the day of the Month standing against that Sunday Letter is Easter Day. If the Full Moon happens upon a Sunday, then (according to the first rule) the next Sunday after is EasterDay.
To find the Golden Number, or Prime, add one to the Year of our Lord, and then divide by 19; the remainder, if any, is the Golden Number; but if nothing remaineth, then 19 is the Golden Number.
To find the Dominical or Sunday Letter, according to the Calendar, until the Year 2099 inclusive, add to the Year of our Lord its Fourth Part, omitting Fractions; and also the Number 6: Divide the sum by 7; and if there is no remainder, the A is the Sunday Letter: But if any number remaineth, then the Letter standing against that number in the small annexed Table is the Sunday Letter.
0A
1G
2F
3E
4D
5C
6B
For the next Century, that is, from the year 2100 till the year 2199 inclusive, add to the current year its fourth part, and also the number 5, and then divide by 7, and proceed as in the last Rule.
Note, that in all Bissextile or Leap-Years, the Letter found as above will be the Sunday Letter, from the intercalated day exclusive to the end of the year.
” 23 A
” 24 B
” 25 C



68
Table 16
Another Table to Find Easter Till the Year 2199 Inclusive
Sunday Letters
Golden Number. A B C D E F G
I. April 16 —— 17 —— 18 —— 19 —— 20 —— 21 —— 15
II. April 9 —— 10 —— 4 —— 5 —— 6 —— 7 —— 8
III. Mar. 26 —— 27 —— 28 —— 29 —— 30 —— 24 —— 25
IV. April 16 —— 17 —— 18 —— 12 —— 13 —— 14 —— 15
V. April 2 —— 3 —— 4 —— 5 —— 6 —— 7 —— 1
VI. April 23 —— 24 —— 25 —— 19 —— 20 —— 21 —— 22
VII. April 9 —— 10 —— 11 —— 12 —— 13 —— 14 —— 15
VIII. April 2 —— 3 —— 4 Mar. 29 —— 30 —— 31 Apr. 1
IX. April 23 —— 17 —— 18 —— 19 —— 20 —— 21 —— 22
X. April 9 —— 10 —— 11 —— 12 —— 6 —— 7 —— 8
XI. Mar. 26 —— 27 —— 28 —— 29 —— 30 —— 31 April 1
XII. April 16 —— 17 —— 18 —— 19 —— 20 —— 14 —— 15
XIII. April 9 —— 3 —— 4 —— 5 —— 6 —— 7 —— 8
XIV. Mar. 26 —— 27 —— 28 —— 29 —— 23 —— 24 —— 25
XV. April 16 —— 17 —— 11 —— 12 —— 13 —— 14 —— 15
XVI. April 2 —— 3 —— 4 —— 5 —— 6 Mar. 31 Apr. 1
XVII. April 23 —— 24 —— 18 —— 19 —— 20 —— 21 —— 22
XVIII. April 9 —— 10 —— 11 —— 12 —— 13 —— 14 —— 8
XIX. April 2 —— 3 Mar. 28 —— 29 —— 30 —— 31 Apr. 1
O make use of the preceding Table, find the Sunday Letter for the Year in the uppermost Line, and the Golden Number, or Prime, in the Column of Golden Numbers, and against the Prime, in the same Line under the Sunday Letter, you have the Day of the Month on which Easter falleth that year. But note, that the Name of the Month is set on the Left Hand, or just with the Figure, and followeth not, as in other Tables, by Descent, but Collateral.
Both Tables 15 and 16 include clearly stated instructions of how they are to be
used to find Easter day. Notice that the same tools – day of month, golden
number, and dominical letter – have been employed. Pertaining to the
dominical letter and golden number, the Book of Common Prayer has included
general tables for finding them. Samples of these general tables can be found
in Appendix B. Notice that these tables are only valid between AD 1662 and
AD 2199; separate tables are drawn up for later periods of time. In modern
times, the computing approach is preferred to table look-ups. The next section
furnishes some established algorithms.



69
6.1.2 Gauss’ Easter algorithm
This algorithm is due to Carl Friedrich Gauss, a famous German
mathematician. It may be considered as an incomplete algorithm because it
involves the use of a table; nonetheless, it is fairly easy to use. When the
algorithm was first published, it contained an error. Recall that the lunar
equation, LUN, is applied eight times in every twenty-five century period. The
first seven applications are made at 300-year intervals and the last is made
after 400 years. LUN was first applied in AD 1800 and subsequently, it would
be applied at AD 2100, AD 2400, ... , AD 3600, AD 3900 and finally AD
4300. Gauss’ mistake in the algorithm was that he had ignored the final 400
year interval between LUN applications. By his algorithm, the date for Easter
Sunday in AD 4200 would be 13 April instead of the correct 20 April. The
corrected version of Gauss’ algorithm, taken from [12], is given below.
_______________________________________________________________
MM 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 M 22 22 23 23 24 24 24 25 26 25 26 27 27 27 28 28 29
MM 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 M 29 29 0 1 0 1 2 2 2 3 4 4 4 5 5 6 6
MM 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 M 6 7 8 7 8 9 9 9 10 10 11 11 11 12 13 12 13
MM 66 67 68 69 70 71 72 73 74 75 76 77 78 79 80 81 82 M 14 15 14 15 16 16 16 17 17 18 18 18 19 20 19 20 21
MM 83 84 85 86 87 88 89 90 91 92 93 94 95 96 97 98 99 M 21 21 22 22 23 23 23 24 25 25 25 26 27 26 27 28 28
()
() ()
100
4 mod 7
100 400
mod19
mod 4
mod 7
19 mod 30
2 4 6 mod 7
22
Year
M MM
Year Year
N
A Year
B Year
C Year
D AM
E B C DN
F DE

= = 
  
=+ −
  
=
=
=
= ×+
= × +× +× +
= ++
If F = 57, or (D = 28 and E =6 and A > 10), then F = F – 7.
_______________________________________________________________



70
MM refers to the century that the year concerned belongs to. For example, this
year, AD 2003, belongs to the 20th century. It thus corresponds to MM = 20. In
turn, we find the matching value for M from the table. This gives M as 24. The
remaining sequence of steps is straightforward. The end result F gives the date
of Easter Sunday in terms of day of March. When F exceeds 31, it would
mean that Easter falls on (F – 31) of April.
6.1.3 O’Beirne’s algorithm
An anonymous American had presented the first flawless, purely arithmetical
algorithm in AD 1876 in the journal Nature. In AD 1965, Thomas H.
O’Beirne published two algorithms based on the one in Nature in his book
“Puzzles and Paradoxes”. His algorithms differed slightly from that in Nature
but retain the feature of being wholly arithmetic. To begin the computation,
only the Gregorian year number is required. Then, through a series of ten
successive division operations, and use of the quotients and remainders thus
generated, the final outcome gives the day and month that Easter Sunday falls
in. The steps of both procedures are tabled below.
_______________________________________________________________
Algorithm 1 Step Dividend Divisor Quotient Remainder (1) x 19 – a (2) x 100 b c (3) b 4 d e (4) 8b + 13 25 g (5) 19a + b – d – g + 15 30 – h (6) a + 11h 319 μ (7) c 4 i k (8) 2e + 2i – k – h + μ + 32 7 – λ (9) h – μ + λ + 90 25 n (10) h – μ + λ + n + 19 32 – p _______________________________________________________________
In step (1), the position of the year in a 19-year cycle is identified. That is, the
remainder a is one unit less than the golden number. Step (2) gives the values
for which solar and lunar corrections are made: b increases by 1 at centurial
years only and c is used later in step (7). Step (3) gives d which increases only
in centurial leap years. It also gives remainder e, the number of centurial years
which have not been leap years, subsequent to the previous centurial leap year.



71
From step (4), g is obtained. The value of g increases only when there is an
increase of the epact because of the correction of the month. In step (5), the
value of b – d is required. This has a value which increases when a reduction
of the epact is required because of the omissions which gave the Gregorian
correction of the year. At step (5), the value h obtained is equivalent to the
epact. In fact, the epact is either 23 – h or 53 – h, whichever places the epact in
the range between 1 and 30. Step (6) results in a value μ which is used in steps
(8), (9) and (10) to account for Clavius’ adjustments. With step (7), it is
possible to find the day of the week for the Easter full moon date at step (8).
However, an intermediate step is required to find the dominical letter. This is
achieved by dividing 2e + 2i – k or 2j – k + 4 by 7. Multiples of 7 can be
added to this to attain the smallest non-negative remainder. The letter is A if
the remainder is 0, and it moves on in the alphabet as the remainder increases.
For the case of leap years, the follow dominical letter is added as a prefix.
Steps (9) and (10) give the month and day of Easter Sunday respectively.
______________________________________________________________
Algorithm 2 Step Dividend Divisor Quotient Remainder (1) x 100 b c (2) 5b + c 19 – a (3) 3(b + 25) 4 δ ε (4) 8(b + 11) 25 γ (5) 19a + δ – γ 30 – h (6) a + 11h 319 μ (7) 60(5 – ε) + c 4 j k (8) 2j – k – h + μ 7 – λ (9) h – μ + λ + 110 30 n q (10) q + 5 – n (32) (0) p _______________________________________________________________
Algorithm 2 is arithmetically equivalent to Algorithm 1; the steps have been
modified to simplify the computation of various dividends. The result gives
Easter Sunday as the pth day of the nth month, as in the first algorithm.
6.1.4 Gregorian algorithm by Lilius and Clavius
Together with Christopher Clavius, Aloysius Lilius was the primary designer
of the Gregorian calendar. The following algorithm, adapted from [5], was
developed by them in the late 16th century for determining the date of Easter in



72
the Gregorian calendar. As such, this algorithm is only valid for years after
AD 1582.
_______________________________________________________________
Algorithm E. (Date of Easter.) Let Y be the year for which the date of Easter is
desired.
E1. [Golden number.] Set G ← (Y + 19) + 1.
E2. [Century.] Set C ← Y 100
  + 1.
E3. [Corrections.] Set X ← 3C 4 −12,

  Z← ( )
 8C + 5 25 − 5.

E4. [Find Sunday.] Set D ← 5Y 4 − X −10.


E5. [Epact.] Set E ← ( )
11G 20 Z X mod 30.
+ + − If E = 25 and the golden
number G is greater than 11, or if E = 24, then increase E by 1.
E6. [Find full moon.] Set N ← 44 – E. If N < 21 then set N ← N + 30.
E7. [Advance to Sunday.] Set N ← N + 7 – ((D + N) mod 7).
E8. [Get month.] If N > 31, the date is (N – 31) APRIL; otherwise the date is
N March.
_______________________________________________________________
The same source had led to another one, [4], which included steps that allowed
the algorithm to work even in AD 1582 or any year before. The more general
algorithm is included below, with the “comment” omitted.
_______________________________________________________________ procedure Easter (year, month, day); value year; integer year, month, day;
comment (omitted)
begin integer golden number, century, Gregorian correction, Clavian
correction, extra days, epact;
integer procedure mod (a, b); value a, b; integer a, b; mod := a – b × (a ÷ b);
golden number:= mod (Y, 19) + 1; if year ≤ 1582 then go to Julian;
Gregorian: century := year ÷ 100 + 1;
Gregorian correction := (3 × century) ÷ 4 – 12;
Clavian correction := (century – 16 – (century – 18) ÷ 25) ÷ 3;
extra days := (5 × year) ÷ 4 – Gregorian correction – 10;
epact := mod (11 × golden number + 20 + Clavian correction – Gregorian
correction, 30);



73
if epact ≤ 0, then epact := epact + 30;
if (epact = 25 ∧ golden number > 11) ∨ epact = 24 then epact := epact + 1;
go to ending routine;
Julian: extra days := (5 × year) ÷ 4; epact := mod (11 × golden number – 4,
30) + 1;
ending routine: day := 44 – epact; if day < 21 then day := day + 30;
day := day + 7 – mod (extra days + 7, 7);
if day > 31 then begin month := 4; day := day – 31 end
else month := 3 end Easter
_______________________________________________________________
In this second algorithm, the steps, no doubt are expressed differently from
those in the first algorithm. Nonetheless, they refer to identical entities. The
line headed by “Julian” lists the steps for finding an Easter date of a year prior
to the time of adoption of the Gregorian calendar.
6.1.5 Carter’s algorithm
The algorithms brought up so far can serve for extended periods of time.
However, it is possible to find algorithms which are valid only for several
years. The following rules are found from [19]. Derived by Carter, this
algorithm only applies to the period between AD 1900 and AD 2099. We note
that in AD 2000, both the solar and lunar equations are not applied to the lunar
tables. In turn, the golden numbers in the period between AD 1900 and AD
2099 are not shifted about in the lunar tables. This means that Clavius’
adjustments are not needed in any algorithm used to determine the date of
Easter Sunday for that period. Consequently, Carter’s algorithm may be seen
as shorter than the previously mentioned algorithms. His algorithm is as
follows:
_______________________________________________________________
Calculate D = 225 – 11 (Y mod 19)
If D is greater than 50 then subtract multiples of 30 until the resulting new
value of D is less than 51.
If D is greater than 48 subtract 1 from it.
Calculate E = (Y + Y 4
  + D + 1) mod 7.



74
Calculate Q = D + 7 – E.
If Q is less than 32 then Easter is in March. If Q is greater than 31 then Q – 31
is its date in April.
_______________________________________________________________
6.2 Final remark
Given that Easter is related to the date of the vernal equinox and the age of the
moon, the date for Easter could have been determined astronomically, even at
the time of the Julian calendar. However, this has not been done because the
exact time of any astronomical event depends on the local time of the
observer. Furthermore, from the institution of leap days in the Julian calendar,
these caused the date assigned to the vernal equinox to oscillate around the
actual event.
Quoting Johannes Kepler, “Easter is a feast, not a planet.” Since the adoption
of a notional sun and moon, the determination of Easter Sunday has been more
mathematical than astronomical. The algorithms highlighted in the previous
section demonstrate the convenience brought about by mathematics.
Mathematical manipulation may make one algorithm seem vastly different
from another. Yet in general, these algorithms share the same basic principles
of calculation and the same set of tools. Significant differences in them could
arise in their presentations if they have been based on different calendars or
admit exceptions. Hence, in using any Easter algorithm, it is important to be
clear about its underlying method, calendar and validity period.
Finally, in general, the date of Easter slips back by about eight days each year
until it hops forward again. Its regularity follows the algorithms discussed
previously. However we should note that even though the found algorithms
are designed to date Easter correctly forever, they would still slip into error
after a very long period of time. This is because the rules on which these
algorithms are based do contain residual imperfections. Furthermore, the
astronomical lengths of the month and day are slowly changing due to tidal
friction.



75
Appendix A: Contents page of the second edition of the Book of Common Prayer
(extracted from [10])
THE CONTENTS OF THIS BOOK.
i. A PREFACE.
ii. Of ceremonies, why some be abolished and some retayned.
iii. The ordre howe the Psalter is appointed to be read.
iv. The Table for the order of the Psalmes to be sayd at Mornyng and Evening prayer.
v. The order how the rest of holy Scripture is appointed to be read.
vi. Propre Psalmes and Lessons at Morning and Evening Praier, for certayne feastes and dayes.
vii. An Almanack.
viii. The Table and Kalendar for Psalmes and Lessons, with necessarie Rules apperteynyng to the same.
ix. The order for Mornyng Prayer and Eveninge Praier throughout the yere.
x. The Letanie.
xi. The Collectes, Epistles, and Gospels, to be used at the ministracion of the holy Communion, throughout the yere
xii. The order of the ministracion of the holy Communion.
xiii. Baptisme both publique and private.
xiv. Confirmacion, where also is a Catechisme for children.
xv. Matrimonie.
xvi. Visitacion of the sicke.
xvii. The Communion of the sicke.
xviii. Burial.
xix. The thanksgiving of women after childe-birth.
xx. A Comminacion against sinners, with certain praiers to be used divers tymes in the yere.
xxi. The fourme and maner of makyng and consecrating of Bischoppes, Priestes, and Deacons.



76
Appendix B (Extracted from [10])
General Tables for Finding the Dominical or Sunday Letter, And the places of the Golden Numbers in the Calendar
Table I
6543210
BCDE FGA 1600 1700 1800
1900
2000 2100 2200 2300
2400 2500 2600 2700
2800
2900 3000 3100
3200 3300 3400 3500
3600 3700
3800 3900
4000 4100 4200 4300
4400 4500 4600
4700
4800 4900 5000 5100
5200 5300 5400 5500
5600
5700 5800 5900
6000 6100 6200 6300
6400 6500
6600 6700
6800 6900 7000 7100
7200 7300 7400
7500
7600 7700 7800 7900
8000 8100 8200 8300
8400
8500 &c.
O find the Dominical or Sunday Letter for any given Year of our Lord, add to the year its fourth part, omitting fractions, and also the number, which in Table I. standeth at the top of the column, wherein the number of hundreds contained in that given year is found: Divide the sum by 7, and if there is no remainder, then A is the Sunday Letter; but if any number remaineth, then the Letter, which standeth under that number at the top of the Table, is the Sunday Letter.



77
Table II
O find the Month and Days of the Month to which the Golden Numbers ought to be prefixed in the Calendar, in any given Year of our Lord, consisting of entire hundred years, and in all the intermediate years betwixt that and the next hundredth year following, look in the second column of Table II. for the given year consisting of entire hundreds, and note the number or cypher which stands against it in the third column; then, in Table III. look for the same number in the column under any given Golden Number, which when you have found, guide your eye side-ways to the left hand, and in the first column you will find the Month and Day to which that Golden Number ought to be prefixed in the Calendar, during that period of one hundred years.
The Letter B prefixed to certain hundredth years in Table II. denotes those years which are still to be accounted Bissextile or Leap-Years in the New Calendar; whereas all the other hundredth years are to be accounted only common years
I. II. III. I. II. III.
Years of
Our Lord
Years of
Our Lord
1600 0 5200 15
1700 1 5300 16
1800 1 5400 17
B
1900 2
B
5500 17
2000 2 5600 17
2100 2 5700 18
2200 3 5800 18
B
2300 4
B
5900 19
2400 3 6000 19
2500 4 6100 19
2600 5 6200 20
B
2700 5
B
6300 21
2800 5 6400 20
2900 6 6500 21
3000 6 6600 22
B
3100 7
B
6700 23
3200 7 6800 22
3300 7 6900 23
3400 8 7000 24
B
3500 9
B
7100 24
3600 8 7200 24
3700 9 7300 25
3800 10 7400 25
B
3900 10
B
7500 26
4000 10 7600 26
4100 11 7700 26
4200 12 7800 27
B
4300 12
B
7900 28
4400 12 8000 27
4500 13 8100 28
4600 13 8200 29
B
4700 14
B
8300 29
4800 14 8400 29
4900 14 8500 0
5000 15
B
&c.
B
5100 16



78
Table III
Paschal Sunday Full Letters. The Golden Numbers.
Moon. 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19
Mar. 21 C 8 19 0 11 22 3 14 25 6 17 28 9 20 1 12 23 4 15 26
Mar. 22 D 9 20 1 12 23 4 15 26 7 18 29 10 21 2 13 24 5 16 27
Mar. 23 E 10 21 2 13 24 5 16 27 8 19 0 11 22 3 14 25 6 17 28
Mar. 24 F 11 22 3 14 25 6 17 28 9 20 1 12 23 4 15 26 7 18 29
Mar. 25 G 12 23 4 15 26 7 18 29 10 21 2 13 24 5 16 27 8 19 0
Mar. 26 A 13 24 5 16 27 8 19 0 11 22 3 14 25 6 17 28 9 20 1
Mar. 27 B 14 25 6 17 28 9 20 1 12 23 4 15 26 7 18 29 10 21 2
Mar. 28 C 15 26 7 18 29 10 21 2 13 24 5 16 27 8 19 0 11 22 3
Mar. 29 D 16 27 8 19 0 11 22 3 14 25 6 17 28 9 20 1 12 23 4
Mar. 30 E 17 28 9 20 1 12 23 4 15 26 7 18 29 10 21 2 13 24 5
Mar. 31 F 18 29 10 21 2 13 24 5 16 27 8 19 0 11 22 3 14 25 6
April 1 G 19 0 11 22 3 14 25 6 17 28 9 20 1 12 23 4 15 26 7
April 2 A 20 1 12 23 4 15 26 7 18 29 10 21 2 13 24 5 16 27 8
April 3 B 21 2 13 24 5 16 27 8 19 0 11 22 3 14 25 6 17 28 9
April 4 C 22 3 14 25 6 17 28 9 20 1 12 23 4 15 26 7 18 29 10
April 5 D 23 4 15 26 7 18 29 10 21 2 13 24 5 16 27 8 19 0 11
April 6 E 24 5 16 27 8 19 0 11 22 3 14 25 6 17 28 9 20 1 12
April 7 F 25 6 17 28 9 20 1 12 23 4 15 26 7 18 29 10 21 2 13
April 8 G 26 7 18 29 10 21 2 13 24 5 16 27 8 19 0 11 22 3 14
April 9 A 27 8 19 0 11 22 3 14 25 6 17 28 9 20 1 12 23 4 15
April 10 B 28 9 20 1 12 23 4 15 26 7 18 29 10 21 2 13 24 5 16
April 11 C 29 10 21 2 13 24 5 16 27 8 19 0 11 22 3 14 25 6 17
April 12 D 0 11 22 3 14 25 6 17 28 9 20 1 12 23 4 15 26 7 18
April 13 E 1 12 23 4 15 26 7 18 29 10 21 2 13 24 5 16 27 8 19
April 14 F 2 13 24 5 16 27 8 19 0 11 22 3 14 25 6 17 28 9 20
April 15 G 3 14 25 6 17 28 9 20 1 12 23 4 15 26 7 18 29 10 21
April 16 A 4 15 26 7 18 29 10 21 2 13 24 5 16 27 8 19 0 11 22
April 17 B 5 16 27 8 19 0 11 22 3 14 25 6 17 28 9 20 1 12 23 April 17 B
18 C 6 17 28 9 20 1 12 23 4 15 26
7 18 29 10 21 2 13 24
April 18 C 7 18 29 10 21 2 13 24 5 16 27 8 19 0 11 22 3 14 25



79
Bibliography
Books and publications:
[1] Briggs, Asa (Editor-in-chief) The Longman Encyclopedia 1st Edition. Columbia University Press, 1989.
[2] Chambers’ Encyclopaedia (new edition) Vol. II. London: George Newnes Limited, 1959.
[3] Heilbron, J. L. The Sun in the Church: Cathedrals as Solar Observatories. Cambridge: Harvard University Press, 1999.
[4] Knuth, D.E. “The Calculation of Easter” in Communications of the ACM, Vol. 5, No. 4, 1962, pg 209 – 210.
[5] Knuth, D.E. Fundamental Algorithms, 2nd Edition, in The Art of Computer Programming, Vol.1. Reading: Addison-Wesley Publishing Co., 1973, pg 155 – 156.
[6] O’Beirne, T.H. “Chapter 10 Ten Divisions Lead to Easter” in Puzzles and Paradoxes. London: Oxford University Press, 1965.
[7] Reingold, E.M. & Dershowitz, N. Calendrical Calculations – The Millenium Edition. Cambridge: Cambridge University Press, 2001.
[8] Richards, E.G. Mapping Time: The Calendar and its History. New York: Oxford University Press, 1998.
[9] Stewart, Ian. “Easter is a Quasicrystal” in Scientific American March 2001.
Websites:
[10] Anglican Resource Collection: The Book of Common Prayer, Nov 1998. http://justus.anglican.org/resources/bcp/
[11] GM Arts Homepage: Easter dating, June 2000. http://users.chariot.net.au/~gmarts/easter.htm
[12] Henk Reints. Easter date algorithms, 1999. http://members.brabant.chello.nl/~h.reints/easter/index.htm
[13] Hill, Bonnie L. Calendar FAQ v1.6 – Part 1, October 2002. http://www.webspace4me.net/~blhill/pages.aux/astrology/cal.FAQ.1.html
[14] Howell, Lynda M. The Book of Common Prayer. http://www.eskimo.com/~lhowell/bcp1662/index.html



80
[15] Mallen, Ronald W. Astronomical Society of South Australia: Easter Dating Method, April 2002. http://www.assa.org.au/edm.html#Method
[16] Meyer, Peter. The Julian and Gregorian Calendars. http://serendipity.magnet.ch/hermetic/cal_stud/cal_art.htm
[17] Robert Harry van Gent. A Bibliography on Easter, the Computus and Easter Algorithms. April 2002. http://www.phys.uu.nl/~vgent/easter/easterbibliography.htm
[18] Ross, Kelley L. The Determination of Easter, on both the Julian and Gregorian Calendars, 1999. http://www.friesian.com/easter.htm
[19] Royal Observatory Greenwich: The Date of Easter. http://www.rog.nmm.ac.uk/
[20] The Catholic Encyclopaedia Online Edition: Dominical Letter, Dec 2002. http://www.newadvent.org/cathen/05109a.htm
[21] Tobin, Paul N. The Rejection of Pascal’s Wager: The Last Supper, 2000. http://www.geocities.com/paulntobin/lastsupper.html
[22] Tondering, Claus. Frequently Asked Questions about Calendars Version 2.4, 28 October 2001. http://www.tondering.dk/claus/calendar24.html
[23] US Naval Observatory http://aa.usno.navy.mil/