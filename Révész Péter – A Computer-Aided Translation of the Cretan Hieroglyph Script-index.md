---
master_file: "[[@ReveszPeterComputerAideda]]"
---
# Index for Révész Péter – A Computer-Aided Translation of the Cretan Hieroglyph Script.pdf

A Computer-Aided Translation of the Cretan Hieroglyph Script
PETER Z. REVESZ Department of Computer Science and Engineering University of Nebraska-Lincoln Lincoln, NE 68588 USA revesz@cse.unl.edu http://cse.unl.edu/~revesz
Abstract: - This paper presents a computer-aided translation of the Cretan Hieroglyph script. The sound values of Cretan Hieroglyph symbols are identified by matching the Cretan Hieroglyph symbols to Phaistos Disk symbols with already known sound values. The matching of pairs of symbols is checked by computer software that finds numerous matches between short Cretan Hieroglyph inscriptions and the Phaistos Disk text. As a result, several Cretan Hieroglyph inscriptions can now be deciphered with a high confidence.
Key-Words: - Computational Linguistics, Cretan Hieroglyphs, Decipherment, Cryptography, Data Mining and Analytics, Relational Databases, SQL
1 Introduction
For over a century, the various writings of the ancient Minoans were unreadable, including Linear A, the Cretan Hieroglyphs, and the Phaistos Disk. Our recent translation of the Phaistos Disk [1] provides a basis of translating Cretan Hieroglyph documents because of the numerous similarities between the Phaistos Disk and the Cretan Hieroglyph scripts [2]. In spite of the similarities, there are also some great differences. Foremost, the Phaistos Disk is a remarkably long text with a length of 241 symbols, whereas most Cretan Hieroglyph writings are rather short .In fact, a significant number of the Cretan Hieroglyph documents are seals with only two or three symbols. The Phaistos Disk has some unique characters that are not found on any of the seals or other inscriptions with the exception of the Arkalochori Axe. The unique features of the Phaistos Disk led some researchers to speculate that it may be a forgery [3]. However, we believe that its novel features are simply due to it being a late form of Cretan Hieroglyphs and the nature of being stamped into clay character-by-character rather than carved into some hard stone. Current research considers the so called Archanes script from 21st century BC to be the earliest Cretan Hieroglyph writing, while the Phaistos Disk is dated by Duhoux [4] to between 1850 and 1600 B.C., although some researchers assign an even later date to the disk. Hence there could be centuries of difference between most Cretan Hieroglyph
inscriptions and the Phaistos Disk. The Phaistos Disk was found together with a Linear A document. That suggests that whatever date the disk was made, it was made at a time when Linear A was already starting to replace Cretan Hieroglyphs. The fact that many Cretan Hieroglyph seals continued to be used for generations after their creation implies that the date of creation of many of the seals may be centuries older than the archeological layer in which they were found. This also implies that there may be a large time difference between most Cretan Hieroglyph documents and the Phaistos Disk. The Phoenician alphabet is known to have gone through much change over the centuries. Keeping that history in mind, one cannot be surprised by some development of the original Cretan Hieroglyph script to the Phaistos Disk script. The length of the Phaistos Disk text assures that any claimed translation of it can be evaluated to be false or true based on internal consistency and grammatical correctness because it is impossible to provide an internally consistent and grammatically correct but false translation for such a lengthy text. For example, Duhoux [5] points out grammatical inconsistencies in the translation attempt of Faucounau’s [6]. Similar comments may be made about other translations. The numerous incorrect translations of the Phaistos Disk led many experts to automatically reject any translation and claims. However, that natural skepticism may change as our earlier translation of the Phaistos Disk forms a basis in this paper to a similar translation of some Cretan Hieroglyph inscriptions.
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 127 Volume 1, 2016



Table 1. The Phaistos Disk and Cretan Hieroglyph symbol correspondences with sound values based on [1] and [2]. A consonant sound value may be followed by an optional vowel. Here j* means /j/, /jom/ or /jon/, and u* means /u/ or /uz/.
1
A
/m/
2
B
/k/
^
3
3
C
N
2
i
44
4
D
~
1
5
E
6
F
/ɒ/
o
4
7
G
/v/
A
53
157
8
H
/ɛ/
O
8
W
58
9
I
/n/
∑
26
46
10
J
/͡ts/
a
49
n
50
11
K
/i/
x
57
12
L
j*
ß
75
13
M
14
N
/m/
g
34
15
O
/s/
§
308
16
P
e
56
17
Q
18
R
/s/
H
7
19
S
/t/
95
20
T
s
54
21
U
u*
c
42
22
V
/g/
93
23
W
/d/
Q
62
24
X
/z/
X
37
25
Y
/o/
J
40
26
Z
/p/
G
6
l
28
88
27
a
/ʃ/
t
41
28
b
/l/
V
10
29
c
/j/
30
d
/b/
p
11
∂
18
31
e
/ɲ/
M
20
w
92
32
f
/l/
®
52
85
33
g
/h/
h
19
∫
39
34
h
/m/
22
35
i
/n/
E
25
36
j
/r/
≈
24
u
29
37
k
/k/
b
70
38
l
/f/
C
5
39
m
/ʒ/
m
23
j
31
40
n
/u/
Ï
153
41
o
/͡ɟʝ/
66
42
p
43
q
L
72
44
r
45
s
/ ͡cç/
f
38
Y
69
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 128 Volume 1, 2016



This paper is organized as follows. Section 2 presents the correspondence table between Cretan Hieroglyph and Phaistos Disk script symbols and their sound values. Section 3 describes the matches found between Cretan hieroglyph inscriptions and the Phaistos Disk text using a MySQL relational database representation and SQL queries. Section 4 presents a translation of some Cretan Hieroglyph inscriptions. Finally, Section 5 gives some conclusions and directions for future work.
2 Cretan Hieroglyph Script Sound Values
The most important step in the decipherment of any script is the establishment of a correspondence between script symbols and sound values. Table 1 lists the 45 different script symbols of the Phaistos Disk according to the ordering of Arthur Evans [7]. Each entry of Table 1 shows on top Evans’ order number, a Phaistos Disk symbol, the corresponding sound value based on [1], the corresponding Cretan Hieroglyph symbol based on [2] and the CHIC numbering of those symbols based on [9]. When there are other candidate correspondences, the optional sixth and seventh lines in an entry give the alternative Cretan Hieroglyph symbol and its CHIC number, respectively. If there are still more candidate correspondences, then the above pattern is further repeated for the optional eight and ninth lines. The correspondences between the Cretan Hieroglyph and the Phaistos Disk symbols are based on visual similarities. It needs to be mentioned that while the Phaistos Disk symbols are completely uniform throughout the text, the Cretan Hieroglyph symbols vary considerably in shape and size just as any other handwritten characters can be expected to do. Sometimes the same object is depicted in different ways. For example, an object can be shown in a symmetric form with left and right sides reversed. There are three observations regarding the table. The first observation is that some objects are denoted in several variations. For example, the Phaistos Disk glove symbol can be depicted as
either the Cretan Hieroglyph W symbol or O symbol. There are some Phaistos Disk signs with three possible Cretan Hieroglyph equivalents. For example, the Phaistos Disk horn symbol can be depicted as any of the following Cretan Hieroglyph symbols:
G
, l or
Unfortunately, all of these variations or polymorphisms may further complicate the translation of Cretan Hieroglyph texts. The second observation is that some symbols are not single sounds or syllables but logograms. For example the symbol is considered a logogram meaning ‘cat.’ This logogram is not assigned a CHIC number by [9]. The third observation is that the script is an abjad instead of a syllabary. That is, each consonant may be followed by an optional vowel. Such an abjad if regularized may evolve into a syllabary, and what we considered consonantal polymorphisms in the second observation may in fact be different CV type syllables with the same consonantal beginning.
3 Matches between Cretan Hieroglyph Inscriptions and the Phaistos Disk Text
If the Phaistos Disk is a form of Cretan Hieroglyphs, then it can be expected that several words or phrases of the Phaistos Disk text will match the other Cretan Hieroglyph inscriptions. Section 3.1 describes computer software that searches for matches. Section 3.2 presents the list of matches that were found.
3.1 Data Source and Software
We created Table 2, a correspondence table between CHIC numbers and Evans’s numbers. Table 2 shows leading zero symbols as is common in the CHIC enumerations. Table 2 represents a many-to-one function because, as we saw in Table 1, several different Cretan Hieroglyph symbols may encode the same Phaistos Disk symbol. John Young’s online Cretan Hieroglyphs page contains a lexicon of all the words found in the known Cretan Hieroglyphs inscriptions. We took from Young’s lexicon the CHIC encoding, the word, the source, and added the equivalent Evans encoding based on Table 2. The result is shown in Table 3. We only used words that included at least two symbols, although Young’s lexicon included some words with only one symbol. We also translated teach block of the Phaistos Disk into an Evans encoding as shown in Table 4. The Phaistos Disk is read side A then Side B from the innermost symbol towards the edge of the disk. The block numbers are according to this reading. We omitted blocks that are repetitions of earlier blocks. For example, we omitted block 4 from Table 4 because it is identical to block 1.
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 129 Volume 1, 2016



Table 2. Encoding correspondence table.
CHIC Number for Cretan Hieroglyph
Evans’ Number for Phaistos Disk
001 04
002 03
003 02
004 06
005 38
006 26
007 18
008 08
......
Table 3. Cretan Hieroglyph words from the lexicon of John Young at http://people.ku.edu/~jyounger/Hiero/.
CHIC
Encoding Word Source Evans
Encoding
005-019 Ch CHIC 112a 38-33
005-044-049 Cia CHIC 276g 38-03-10
006-041 Gt CHIC 246b 21-27
... ...... ...
Table 4. The Evans encoding of the Phaistos Disk.
No
. Block Evans
Encoding
1 l C J 38-03-10
2 A M 01-13
3 U k i a a L B 21-37-35-27-27-12-02
5 i S W 35-19-23
...... ...
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 130 Volume 1, 2016



3.2 Textual Matches Found
We represented Tables 3 and 4 leaving out the Word and the Block columns, respectively, as MySQL relational database tables. Next we used a simple SQL database query to find all pairs from the two tables where the Evans encoding of Table 3 is included in the Evans encoding of Table 4. The matches found are listed in the second column of Table 5 with the matched part highlighted in bold. For sake of clarity, we add to Table 5 in the first column the Cretan Hieroglyph word and in the third column the Phaistos Disk block that were matched.
The high number of matches between Cretan Hieroglyph inscriptions and the Phaistos Disk text shown in Table 5 is a strong indication that our reading direction of the Phaistos Disk is correct. Previously even the reading direction was a debated topic. Duhoux [5] states that only a reading from the edge of the disk towards the center of the disk can be valid. On the other hand, the vast majority of the Cretan Hieroglyph inscriptions are written from left-to-right, and a left-to-right reading of the Phaistos Disk would imply reading it from the center to the outside.
Table 5. This table shows the matches found between the Cretan Hieroglyph Inscriptions and the Phaistos Disk. In all cases the Cretan Hieroglyph inscription is embedded into one of the Phaistos Disk blocks. The middle column shows the Evans encoding of the Phaistos Disk with the embedded Cretan Hieroglyph part highlighted in bold face.
Cretan Hieroglyph Inscription
Evans Encoding of Phaistos Disk Block with Cretan Hieroglyph match in bold
Phaistos Disk Block
Cia 38-03-10 L C J
cbE 21-37-35-27-27-12-02 U k i a a L B
gt 27-18-32-14-27-12-02 a R f N a L B
lw 26-31-27-02 Z e L B
t^ 18-23-10-25-27-02 R W J Y a B
Qh 23-33 W g
xm 11-39 K m
JQ 25-23-34-29 Y W h c
mp 07-18-39-30-09 G R m d I
∂ 07-18-39-30-09 G R m d I
OA 08-07-36-29-22 H G j c V
JQ 25-23-34-27 Y W h a
ge 18-14-16 R N P
^ 40-36-26-02 n j Z B
§ 18-01-13-07-15 R A M G O
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 131 Volume 1, 2016



4 Translation of Cretan Hieroglyph Texts
In this section, we consider the translation of some Cretan Hieroglyph texts. At first, we can start with the observation that since some Cretan Hieroglyph words match exactly a piece of the Phaistos Disk text, they can be translated as the same ProtoFinno-Ugric or Proto-Hungarian word as we gave before in [1]. For example, in [1], the first Phaistos Disk block
lCJ
was translated as “chief god.” That block is now shown to be equivalent to:
Cia.
Hence we can translate this also as “chief god.” In fact, a closer observation shows that the pair:
ia
is a frequent Cretan Hieroglyph combination that follows a number of different symbols. Therefore, it seems likely that this pair of symbols means “god,” and the symbol before it specifies the type of god that is meant. In this case, the Phaistos Disk rosette symbol and the Cretan Hieroglyph symbol with the emanating rays, that is,
l and C respectively, fairly clearly refer to the Sun. Therefore the “chief god” is really the “Sun god.” The two concepts may have been used as synonyms in the Minoan culture given the central importance of the Sun goddess [9]. In addition, our translation of the Phaistos Disk [1] reveals a prayer to a Sun goddess. As another example, consider the Cretan Hieroglyph inscription CHIC 172, which is simply the following text of three symbols written with a left-to-right direction:
lwV
The above can be transliterated as /p/ /ɲ/ /l/. Assuming the text is some type of abjad script where the vowels need to be filled in, and assuming a /p/ > /f/ sound change, there is the following Proto-Hungarian [10] possibility: fénylő (shining). The above translation is supported by the fact that the first two symbols occur in one of the blocks of the Phaistos Disk, where it was translated as as the Hungarian word: fény (light). Note that –lő is a Hungarian suffix that modifies nouns into adjectives. A general method is cryptography is to concentrate on the most frequently occurring words or symbols and try to decipher them before the
others. The most frequently occurring words in the Cretan Hieroglyphs could be some common names of persons, gods, objects etc. Hence as a third example of deciphering some inscription apart from the ones that trivially follow from the Phaistos Disk matches, consider the following frequently occurring triplet of symbols that occur in CHIC 169, CHIC 195, etc.:
fVj
Using Table 1, the sounds of the above triplet can
be transliterated as / ͡cç/ /l/ /ʒ/.
Assuming the consonant sound changes / ͡cç/ > /θ/ and /ʒ/ > /ʃ ʃ/, we obtain the word Thalassa. That is the Greek word for ‘sea,’ and it is considered to be a Minoan word that was borrowed by ancient Greek. The word Thalassa has no IndoEuropean etymology, but it may be related to Hungarian tó (lake) [10]. For the sake of brevity, we will present more sample translations of Cretan Hieroglyph inscriptions only in another extended version of this paper.
5 Conclusions and Future Work
We are currently working on the translation of other Cretan Hieroglyph texts. We have a tentative translation of some longer inscriptions that we plan to present in the journal version of this paper. It still remains an interesting open problem to correlate the Cretan Hieroglyph and the Phaistos Disk scripts with Linear A texts. Our method seems to be applicable to Linear A scripts too, but we need to proceed carefully because the Linear A script is more distant from the Phaistos Disk script than the Cretan Hieroglyph is to the Phaistos Disk. Hence a solid translation of all the Cretan Hieroglyph texts may be necessary before fruitfully attempting a translation of Linear A texts.
References:
[1] Peter Z. Revesz, A computer-aided translation of the Phaistos Disk, International Journal of Computers, Vol. 10, No. 1, 2016, pp. 94-100, [2] Peter Z. Revesz, Bioinformatics evolutionary tree algorithms reveal the history of the Cretan script family, International Journal of Applied Mathematics and Informatics, Vol. 10, No. 1, 2016, pp. 67-76. [3] Jerome M. Eisenberg, The Phaistos Disk: One hundred year old hoax?, Minerva, July/August 2008, pp. 9-24.
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 132 Volume 1, 2016



[4] Yves Duhoux, Le Disque de Phaestos, Leuven, 1977. [5] Yves Duhoux, How not to decipher the Phaistos Disc, American Journal of Archaeology, Vol. 104, No. 3, 2000, pp. 597600.
[6] Jean Faucounau, Le Déchiffrement du Disque de Phaistos: Preuves et conséquences. L'Harmattan, Paris/Montreal 1999.
[7] Arthur J. Evans, Scripta Minoa: The Written Documents of Minoa Crete with Special Reference to the Archives of Knossos, Volume II, Classic Books, 1909. [8] Jean-Pierre Olivier, Louis Godard, in collaboration with J.-C. Poursat, Corpus Hieroglyphicarum Inscriptionum Cretae (CHIC), De Boccard, Paris 1996)
[9] Nanno Marinatos, Minoan Kingship and the Solar Goddess: A Near Eastern Koine, University of Illinois Press, 2010. [10] Gábor Zaicz, chief editor, Etimológiai Szótár: Magyar Szavak és Toldalékok Eredete, (Etymological Dictionary: Origin of Hungarian Words and Affixes), Tinta Könyvkiadó, 2006.
P. Z. Revesz
International Journal of Signal Processing http://iaras.org/iaras/journals/ijsp
ISSN: 2367-8984 133 Volume 1, 2016