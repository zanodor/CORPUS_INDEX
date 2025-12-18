---
master_file: "[[@ReveszPeterComputerAided]]"
---
# Index for Révész Péter – A Computer-Aided Translation of the Phaistos Disk.pdf

Abstract—This paper presents a novel semi-automatic translation method for the Phaistos Disk that had no convincing translation for over a century. The method uses for a recently discovered connection between the Phaistos Disk symbols and other ancient scripts, including the Old Hungarian alphabet. The connection between the Phaistos Disk script and the Old Hungarian alphabet suggested the possibility that the Phaistos Disk language may be related to Proto-Finno-Ugric, Proto-Ugric, or Proto-Hungarian. Using words and suffixes from those languages, it is possible to translate the Phaistos Disk text as an ancient sun hymns that are connected to a winter solstice ceremony and a mythological explanation of the perceived daily route of the Sun in the sky. Keywords—Acrophonic principle, Cretan Hieroglyph, Linear A, Linear B, Phaistos Disk, Proto-Finno-Ugric, Proto-Hungarian
I. INTRODUCTION
uigi Pernier discovered a fired clay flat round object with an archaic form of writing at the Phaistos palace on the island of Crete in 1908. The object called the Phaistos Disk (also spelled Phaistos Disc) was the subject of several decipherment or translation attempts that did not yield any convincing results. For example, in their decipherment attempts, Faucounau [8] and Fisher [9] assume an archaic form of Greek, Aartun [1] assumes a Semitic language, Achterberg et al. [2] assume Luwian, Kovar [14] uses Proto-Slavic, Kvashilava [10] assumes Georgian, and Owens [15] assumes some Indo-European language. Duhoux [5] is a critique of previous decipherment attempts. Not only does the language of the Phaistos Disk remain unknown, but even its authenticity was questioned by some reserchers [5]. However, most researchers agree with Duhoux [4] that the Phaistos Disk is a Bronze Age Minoan artifact created between 1850 B.C. and 1600 B.C. on the island of Crete. The symbols on the disk have numerous connections to other native Cretan writings, which were first classified by Arthur Evans, the explorer of Knossos Palace, as Cretan Hieroglyph, the Linear A and the Linear B scripts [7]. In 1952 Michael Ventris gave a decipherment of Linear B as described in Chadwick [3]. Hooker [12] gives a good introduction to Linear B. The Cretan Hieroglyph [24] and the Linear A scripts are also not deciphered.
Peter Z. Revesz is with the Department of Computer Science and Engineering, University of Nebraska-Lincoln, Lincoln, NE 68588, USA (revesz@cse.unl.edu). A preliminary version of this paper was presented at the AMCSE conference in Agios Nikolaos, Crete, Greece in October 2015 [19].
Most decipherment attempts relied heavily on the acrophonic principle, which is the taking of the first sound of a word referred to by an object. The acrophonic principle has several problems. First, a symbol may be interpreted as denoting many different objects. Second, the depicted object could have many synonyms in the native language. Third, each of the synonym words may have gone through a linguistic development where the initial sound changed. The combination of these three problems almost guarantees that we can derive by the acrophonic principle numerous beginning sounds for each symbol. In this paper we give a translation of the Phaistos Disk. Unlike previous decipherment attempts, our decipherment relies only minimally on the acrophonic principle. Instead, we use the already established correspondences between Cretan writing symbols and other ancient scripts with known sound values [18]. These other ancient scripts include the Phoenician [22], the South Arabic [23], the Greek and the Old Hungarian (see Forrai [11] and Varga [21]) alphabets. Our approach to the translation of the Phaistos Disk is guided by our previous study of biological evolution [16], [17], [20]. The sound changes within a word are similar to genetic mutations. While many mispronunciations of words are possible, certain mispronunciations are easier to produce than others spread more easily. Similarly, while many types of mutations could occur on a genome, only the beneficial mutations are likely to spread to successive generations of descendants. This paper is organized as follows. Section II outlines a semi-automatic translation method. Section III describes a transliteration of the Phaistos Disk text. Section IV describes a basic dictionary of Proto-Finno-Ugric and Proto-Hungarian words and suffixes and their consonant base representation. Section V presents the translation of the Phaistos Disk using the dictionary. Finally Section VI gives some conclusions and directions for future work.
II. THE TRANSLATION METHOD
We outline below a five-step translation method for the Phaistos disk.
1. Transliterate the symbols on the Phaistos disk using the sound correspondences recently identified in [18]. Some symbols with unknown sound values are not transliterated but are denoted by numbers.
A Computer-Aided Translation of the Phaistos
Disk
Peter Z. Revesz
L
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 94



2. Set up a Proto-Finno-Ugric and Proto-Hungarian dictionary. The dictionary needs to include the most common and oldest prefixes and suffixes. 3. For each word in the dictionary find its consonant base. 4. Find matches between the transliterated text and the words in the dictionary. In the match only the consonant bases are used and vowels are ignored. Each symbol with an unknown sound value can be matched to any consonant or vowel sound, but it has to take the same (or similar) sound value at each of its occurrence. Choose between alternatives based on grammatical correctness. 5. Form sentences and translate them into a modern form.
In the above method, Step 1 can be computerized because it is a simple symbol substitution problem. Step 4 can be also partially computerized because the matching between the Phaistos Disk text and the dictionary requires string searching. We can simply take each word in the dictionary and search for all of its occurrences in the text. We used a simple string searching computer program facilitate this matching process. However, the selection of the best-fit word to each location of the text requires some human judgment and grammatical understanding. Some grammatical knowledge can be built into computer software, like grammar checkers, but we did not have anything available for Proto-Finno-Ugric and Proto-Hungarian, which we presumed to be close relatives to the Phaistos Disk language because of the connection between the Phaistos Disk symbols and the letters of the Old Hungarian alphabet [18].
III. A TRANSLITERATION OF THE PHAISTOS DISK
Arthur Evans [7] gave an enumeration of the forty-five Phaistos Disk symbols, which are listed according to his order in Figure 1. Below his enumeration, we added the putative sound values based on a recent study of the similarities between the Phaistos Disk symbols and some ancient script symbols whose sound values are already known [18]. That study did not include the sound value of symbol 28. We assume that symbol 28 has a sound value of /l/ because it shows a leg, which would be in Proto-Finno-Ugric *lu, from which derives both Finnish luu (bone) and Hungarian láb (leg). In addition, [18] assumed /r/ for symbol 9 in analogy with Phoenician and South Arabic. However, the rhotacism /n/ à /r/ occurs in many languages such as Aramaic. Hence we assume that symbol 9 was /n/ originally. Given the enumeration and the known sound values in Figure 1, side A of the Phaistos Disk can be converted into the following sequence when reading from the center to the edge of the disk:
f-3-͡ts m-13 u*-k-n-ʃ-ʃ-j*-k f-3-͡ts n-t-d m-13-j*-k j*-p-ɲ t-17-s-ɒ ʃ-s-l-m-ʃ-j*-k p-ɲ-j*-k m-l s-d-͡ts-o-ʃ-k p-ɲ-j*-k d-h u*-k-n-ʃ-ʃ-j*-k p-ɲ-j*-k m-l s-d-͡ts-o-ʃ-k i-ʒ f-d-l-j*-k v-40-͡ɟʝ-m n-t-͡ɟʝ-j*-k n-p-ɲ s-ɒ-j*-k ɛ-44-ʃ j*-v- ͡cç-ʃ h-40-4-j*-k m-j-j v- ͡cç-j j*-40-z s-m-13-j*-k
Similarly, side B can be converted into the following:
v- ͡cç o-d-m-j v-d-n-ɒ-k v-s-ʒ-b-n ɛ-v-r-j-g z-s-d-v v- ͡cç-v n-s-v o-d-m-ʃ ɛ-v-r-j-g v- ͡cç -j 13-ɛ-j ɛ-v-r-j m-ʃ-n-k h-ʒ-l-n-ɒ m-h-j s-m-16 n-20-z-z-j m-f-o-ʃ 40-r-p-k n-40-z-v o-42-k-g s-m-13-v-s h-ʒ-m-13 43-s-d-16 j*-20-z-h ʃ-o-g
5-d-k-k n-v- ͡cç-ʃ v-40-g-j*-k
In the above, we highlighted in gray the words or phrases that are repetitions of earlier words or phrases. These highlighted parts of the text do not need a separate translation. We also highlighted in bold the first letter of the words that have below them a slash mark on the disk. The slash seems to be added to the symbols by hand. When we break the text up into lines such that the new lines start with the bold letters, then we get in most lines three words or phrases, assuming that each block of the disk is a word or short phrase. The repetitions highlighted in gray tend to be exactly below their earlier occurrences. Some of the repetitions may be refrains. The structured gray repetitions and the relatively equal lengths of the lines suggest that the text may be a poem or a song.
1
/m/
2
/k/
3 4 56
/ɒ/
7
/v/
8
/ɛ/
9
/n/
10
/͡ts/ 11
/i/
12
j*
13 14
/m/
15
/s/
16 17 18
/s/
19
/t/
20
21
u*
22
/g/
23
/d/
24
/z/
25
/o/
26
/p/
27
/ʃ/
28
/l/
29
/j/
30
/b/
31
/ɲ/
32
/l/
33
/h/
34
/m/
35
/n/
36
/r/
37
/k/
38
/f/
39
/ʒ/
40
/u/
41
/͡ɟʝ/
42 43 44 45
/ ͡cç/
Fig. 1 Each element in this matrix lists from top to bottom the following corresponding triplet: A. Evan’s numbering, Phaistos disk symbol, and IPA sound symbol. These associations are from [18] except for symbol 28, which is new. Here j* means /j/, /jom/ or /jon/, and u* means /u/ or /uz/.
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 95



IV. A PROTO-FINNO-UGRIC AND PROTO-HUNGARIAN WORD AND SUFFIX DICTIONARY
We collected a set of Proto-Finno-Ugric, Proto-Ugric and Proto-Hungarian words using the etymological dictionary [25]. Each word was represented by a consonant base, which was obtained by omitting the vowels. We also use the convention of putting a star symbol before any word that is a hypothetical proto word in any language. When it is necessary, we indicate the source of each word by adding to the word the name of the language in a superscript. For example, the Proto-Ugric word *mälɛ (warm) was represented by the consonant base m-l. The following table gives some examples from the dictionary.
Base Cognate or Proto Word
Hungarian Word
Meaning
-͡ts -ci diminutive suffix d-h düh anger d-s *ipsɛ édes sweet, dear d-͡tʃ dicső glorious f-j *päŋɛ fej > fő head > chief h-l *kalɛ hálo fishing net h-j hajó ship h-j *kajɛ haj-ol to bend h-s *kojćɛ húsz twenty h-z hätistääFinn űz chase h-z *kupɛ-tɛ húz pull j *eje éj night j-n *jäŋɛ jön come j-n-k -junk 1st person plural verb suffix, present tense j-v-t *jomɛ jó, javít good, improve, help k-g *kućɛ húgy star k-n-d k-n-z
kende kenėz
ruler judge l-n lány girl m m-t
maaFinnish
mataaFinnish mászik
earth crawl m-l *mälɛ meleg warm m-l *melɛ mély deep m-n-d mind all m-ʃ *mu más other m-ʃ-t most now n-v-s nousu *növ > nő ascentFinnish, grow n-p nap sun n-t *jomɛ indít make sm start > plead n-t ümetölMansi ünöt int
protect caution n-z *näke néz watch ŋ anya mother ŋ-l *ŋele nyel swallow ŋ-l *ŋōle nyíl arrow p-d-l *pentɛlɛ fedél cover, protector p-j *päjɛ fejér, light, white
p-ŋ fény r-p rop-og crackle r-p r-p
räpyttäFinnish rep-ūl röp-ke
to fly flying ʃ és, s and ʃ *ićä ős ancestor ʃ-b seb-es fast ʃ-d-r sodor drift ʃ-t šitMansi süt bake, shine ʃ-t est evening s-k *śakkɛ szak part, piece s-l *śalkɛ szál rod, thread s-m *śomɛrɛ szomorú sad t-m tuupataFinnish tomb-ol push, jump t-v-s tūjeMansi tulisPermi
tavasz spring
v-l-g *βalkɛ villog virrad világ
to shine to rise (Sun) light, world v-s *βiγe visz to take v-s vissza back, backward
v-t *βete
wiťMansi
víz water
v-t wootMansi veivataFinnish
wind
z izzó hot z az that, the -z *-t -z verb forming suffix
Unfortunately, the symbols used to describe the word pronunciations in [25] do not follow the standard IPA (International Phonetic Alphabet). Hence we changed some of the vowel symbols in [25] to the corresponding IPA symbol. Since the consonant symbols in [25] correspond much better to the IPA, we left them intact in the table.
V. A TRANSLATION OF THE PHAISTOS DISK
A. Sound Changes
The Proto-Finno-Ugric language is assumed to have undergone several sound changes in reaching the Proto-Ugric and the Proto-Hungarian stage of language development. We presume that the language of the Phaistos Disk is close to Proto-Hungarian. Therefore, the language of the Phaistos Disk shares some of the common sound changes that have been identified between Proto-Finno-Ugric and Hungarian. Some of the common sound changes include the following:
p >f
ŋ>j>i
͡tʃ > ͡ts
z >ʒ
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 96



k > g > ͡ɟʝ
t > ͡cç or t > z
Sometimes adjacent pairs of consonants change together in predictable way. For example, the following is a relatively common sound rule change:
*nt > nd > d > l
B. Matches between the Text and the Dictionary
The sound changes slightly influence the way we do string searches. We need to search the Phaistos Disk text to find both the exactly matches and the approximate matches where some of the consonant sound were changed using the sound change rules. We also need to search for both root words and suffixes. The suffixes are restricted to the end of the blocks into which the Phaistos Disk is divided. The blocks are clearly indicated on the disk by the scribe. Each block can be assumed to be either a single word or a phrase. Words do not run across blocks.
f-3-͡ts m-13 u* k-n-ʃ-ʃ-j*-k fő-3-ci mind az kenes-s-jün-k chief 3 all the ruler-1PL.POSS f-3-͡ts n-t-d m-13-j*-k ünöt-öd mind-jun-k chief 3 protect-2SG all 1PL j* p-ɲ t-17-s-ɒ ʃ-s-l m-ʃ-j*-k jő fény tavasz-a süssél másik come light spring-POSS shine again p-ɲ-j*-k m-l s d-͡ts-o ʃ-k fény-jenek meleg s dicső szál-ak shine-3PL warm and glorious ray-PL p-ɲ-j*-k d-h u*-k-n-ʃ-ʃ-j*-k düh shine-3PL anger the ruler-1PL.POSS p-ɲ-j*-k m-l s-d-͡ts-o-ʃ-k i-ʒ f-d-l-j*-k v-40-͡ɟʝ-m n-t-͡ɟʝ-j*-k izzó fedel-jünk villog-ni indít-jūnk hot cover-3PL.POSS rise-INF plead-1PL n-p-ɲ s ɒ-j*-k ɛ-44-ʃ napfé-ny ős anyá-nk édes sunlight ancestor mother-3PL.POSS dear j*-v- ͡cç-ʃ h-40-4-j*-k m-j-j javi-ss/javitys hálóink / hajóink mély help fishing net/ship-3PL.POSS deep v- ͡cç-j j*-40-z s m-13-j*-k víz-i jönwater-LOC go-VERBALIZER and all-1PL
Fig. 2 A translation of Side A showing the result of matching the text with proto-words from the dictionary using the consonant bases with allowance for the sound rule changes described in the text and root changes due to voice assimilation. The root words are highlighted in yellow, the suffixes in blue, the voice assimilations in green, and repeated elements in gray.
In the following, we use the following color highlighting.
Yellow – root word. Blue – suffix. Gray – repetitions of earlier words or phrases. Green – voice assimilation of the root due to suffix.
Fig. 2 shows the result of the string matches color-coded according to the above legend. We added some extra grammatical markers that are not listed in the above dictionary. For example, in the middle of the third row the –a suffix describe a possessive relationship similar to the English possessive ‘s, but while the English language marks the possessor, the Hungarian language marks the possessed object. Hence the possessive phrase “fény tavasz-a” can be translated as “light’s spring.” That phrase is meaningful if we recall that the word “tavasz” derives from a rising of lake water levels [25]. The “light’s spring” may have referred to either any sunrise or a lengthening of the days after a winter solstice. Similarly, side B can be analyzed as shown in Fig. 3.
v- ͡cç o-d-m-j v-d-n-ɒ-k víz tomb-ja woot-nak water push-3SG wind-LOC v-s ʒ-b-n ɛ-v-r-j-g z s-d-v visz sebes-en Iberia-ig az est-ve take-3SG fast-ADV Iberia-LOC the eve-ADJ v- ͡cç-v n-s-v o-d-m-ʃ ɛ-v-r-j-g víz-ve tomb-sz water-ADJ ... push-2SG Iberia- LOC v- ͡cç -j 13-ɛ-j nede-j water-3SG.POSS swallow-3SG ɛ-v-r-j m-ʃ-n-k h-ʒ l-n-ɒ mas-nak húsz lánya Iberia ....-POSS twenty girl-3SG.POSS m-h-j s-m-16 n-20-z-z-j m-f-o-ʃ meg-haj-ol szomorú néz-zi mabend sad watch-3SG earth-.... 40-r-p-k n-40-z-v o-42-k-g ...röp-ke nyilazva húgy fly-NOUNFORMER arrow-VERBALIZER-ADV star s m-13 v-s h-ʒ m-13 és mind vissza húz/űz mind and all back pull/chase all 43-s-d-16 j*-20-z-h ʃ-o-g el-sodor éj-t-szaka Ázsiá-ig away drift during night to Asia 5-d-k-k n-v- ͡cç-ʃ v-40-g-j*-k növ-ez-esz világ-unk ... ascent-VERBALIZER -2SG light-3PL.POSS
Fig. 3 A translation of side B with the same conditions and legend of notation as in Fig. 2.
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 97



C. The Phaistos Disk as a Poem
Instead of a word-by-word rendering of the text, in this section we give a translation of the text as a poem. From the context, there is a suspicion that symbol 3 may refer to some ancestor spirit or divinity, perhaps affectionately called with a diminutive suffix if the ending -͡ts is not part of the name. Another possibility is that the name is a variant of Päike, the name of the Sun in Estonian mythology. In fact, the text seems to be a hymn to a solar divinity to bring back (stronger) sunlight to the earth. This sun hymn on side A of the Phaistos Disk may have been said at a winter solstice ceremony. It can be translated into the following poem:
A
Chief god of all, our ruler. Chief god, you protect all of us. Come light’s spring, shine again Shine warm and glorious rays. Light up strong, our ruler.
Shine warm and glorious rays. For our hot cover, to rise we pray. Sunlight, our dear ancestor mother, Help our ships sailing on the seas And all of us.
Side B is another poem about the Sun. There are a number of observations that can be made before attempting a translation. In the first line, the “windward” direction probably means “westward” because for a large part of Europe the prevailing wind direction is from west to east. In the second line, “Ibēr” is the native name of the Iberian Peninsula, which is today’s Portugal and Spain. In the fifth line, “mas” probably means some ruler and may be translated as “king.” That name may be related to the people names Magyar, the name by which Hungarians call themselves, and Mansi, which both derive from an Ugric root *maŋćɛ, which means “man, patriarch, tribe.” In the sixth line, the meaning of “m-f-o-ʃ” can be guessed from the context in which it occurs, namely, it is something watched by the king’s daughters as the sun appears to be swallowed by the sea. Hence the word’s likely meaning is “horizon,” which is supported by the possible composition of maaFinnish (earth) + päättyäFinnish (end)” with the plausible sound changes p > f and tty > ʃ. In the seventh line, the word “o-42-k-g” seems to refer to some kind of star or star constellation. Since it is preceded by the phrase “flying shooting arrows,” it seems to refer to Sagittarius. The identification of “nyíl” (arrow) uses the same “l” sound value for symbol 40 as was used on side A. The “l” sound was the only surprise to us given our earlier established sound values presented in [18]. This unexpected result may be due to some conflation between symbol 28 and symbol 40. Some authors describe symbol 40 as “ox back” because it seems to show the behind of an ox. However, in that case, the “ox back” is nothing more than two legs. Since symbol 28 is a leg with sound value /l/, then symbol 40 would logically be a
doubling, that is /ll/ as occurs in “villog” in the seventh line of side A. In the last line, the word or phrase “5-d-k-k” is hard to interpret because it starts with symbol 5, which occurs only here. It may be related to Finnish “jatkua” (continue) with a t > d change or to Hungarian “reggel” (morning) with a plausible k > g change and an unlikely r > d change. Since the sound value of symbol 5 is still unknown, we cannot decide which word would be better in this place. Hence we indicate this word or phrase as a “...” in the translation. We also could not translate “n-s-v” in line three and dealt with it the same way. We hope that further progress in the translation will fill in these two gaps. Given the above observations, side B of the Phaistos Disk can be translated as the following poem:
B
Water flows westward. Takes you fast to Iberia by the evening. With water you ... flow to Iberia. Its water swallows you. The Iberian king’s twenty daughters Bend over and sadly watch the horizon.
Flying while shooting arrows Sagittarius And the other stars chase you back. All drift away during the night to Asia, Where you, our light, ... ascend.
Side B of the poem gives a mythological answer to the age-old question of what happens to the Sun at night. According to the poem, the Sun travels west during the day and in the evening falls into the water, probably meant here the Atlantic Ocean. According to mythology, the Atlantic Ocean was somehow connected with the heavens. The Sun temporarily dwelt with the stars and with the stars made a semicircle in the night sky to get back to the east, where it rose again in the morning.
VI. CONCLUSIONS AND FUTURE WORK
Based on recent advances in the comparative study of ancient scripts [18], we could start our translation by having a plausible sound value for the majority of the Phaistos Disk symbols. The sound values presented in [18] seem corroborated by being able to form words, phrases, and sentences with proper grammar after finding matches between the Phaistos Disk text and etymologically plausible proto words from the Proto-Finno-Ugric and the Proto-Hungarian languages [25]. Moreover, the translation yields two sun hymns, which seem to fit in Bronze Age cultural context. There are many Bronze Age cultures where the sun was worshipped. For example, there are Babylonian hymns to Shamash, their sun god, and in ancient Egypt, around 1350 B.C. Pharaoh Akhenaten also wrote several hymns to the sun. The relationship between the newly translated text and other ancient sun hymns may be an interesting direction for further study.
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 98



The Phaistos Disk can be assumed to be an example of the Cretan Hieroglyph writing, and the language of the Phaistos Disk can be assumed to be an example of the Minoan language. Since the translation of the Phaistos Disk relied mostly on Hungarian, the two languages had to have a common original in the past, as was assumed in our earlier work [18]. Fig. 4 shows for the traditional Uralic language family tree a possible extension that accommodates this new discovery. Recently, Mario Alinei proposed a linguistic relationship between Etruscan and Hungarian. It is unclear, however, where Etruscan may fit into the Uralic language
family tree if indeed it belongs there. We also suspect that Linear A is just another way of writing the Minoan language instead of the Cretan Hieroglyph writing. There would be a parallel to that situation in ancient Egypt, where the Egyptian Hieroglyphs provided a more esthetically pleasing picturesque form of writing, while at the same time scribes used the faster and simpler demonic script. In Crete, the Cretan Hieroglyph would be the more esthetically pleasing writing reserved for important occasions and text, while the common accounting tablets used the Linear A writing. These hypotheses need further investigations.
REFERENCES
[1] K. Aartun, Die minoische Schrift : Sprache und Texte vol. 1, Wiesbaden, Harrassowitz, 1992.
[2] W. Achterberg, J. Best, K. Enzler, L. Rietveld, F. Woudhuizen, The Phaistos Disc: A Luwian Letter to Nestor, Publications of the Henry Frankfort Foundation vol XIII, Dutch Archeological and Historical Society, Amsterdam 2004.
[3] J. Chadwick, The Decipherment of Linear B, Cambridge University Press, 1958.
[4] Y. Duhoux, Le Disque de Phaestos, Leuven, 1977.
[5] Y. Duhoux, “How not to decipher the Phaistos Disc,” American Journal of Archaeology, 104 (3), 2000, pp. 597–600.
[6] J. M. Eisenberg, "The Phaistos Disk: One hundred year old hoax?" Minerva, July/August 2008, pp. 9–24.
[7] A. J. Evans, Scripta Minoa: The Written Documents of Minoa Crete with Special Reference to the Archives of Knossos, Volume II, Classic Books, 1909.
[8] J. Faucounau, Le Déchiffrement du Disque de Phaistos: Preuves et conséquences. L'Harmattan, Paris/Montreal 1999.
[9] S. R. Fisher, Glyph-Breaker, Springer, 1997.
[10] G. Kvashilava, On Reading Pictorial Signs of the Phaistos Disk and Related Scripts, Ivane Javakhishvili Institute of History and Ethnology, Tbilisi, 2010.
Fig. 4 A proposed extension of the traditional Uralic language family tree. The extension assumes that the Phaistos Disk is records the Minoan language, which is grouped together with Hungarian, into a West Ugric group within the Ugric branch.
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 99



[11] S. Forrai, The Old Hungarian Writing from Ancient Times to the Present, (in Hungarian), Antológia Kiadó, 1994.
[12] J. T. Hooker, Linear B: An Introduction, Bristol Classical Press, 1980.
[13] G. Hosszú, Heritage of Scribes: The Relation of Rovas Scripts to Eurasian Writing Systems, Rovas Foundation Hungary, 2013.
[14] J. Matejka, “Translation of the Phaistos Disc,” WM Magazine, January 19, 2011.http://www.wmmagazin.cz/view.php?cisloclanku=2011010004
[15] G. A. Owens, The Phaistos Disk and related inscriptions, 2008-2014. http://www.teicrete.gr/daidalika/pages/page.php?page=phaistos_disk
[16] P. Z. Revesz, Introduction to Databases: From Biological to Spatio-Temporal, Springer, New York, 2010.
[17] P. Z. Revesz, “An algorithm for constructing hypothetical evolutionary trees using common mutations similarity matrices,” Proc. 4th ACM International Conference on Bioinformatics and Computational Biology, ACM Press, Bethesda, MD, USA, September 2013, pp. 731-734.
[18] P. Z. Revesz, “A computational study of the evolution of Cretan and related scripts,” Proc. 3rd International Conference on Applied Mathematics, Computational Science and Engineering, Agios Nikolaos, Crete, Greece, October 2015, pp. 21-25.
[19] P. Z. Revesz, “A Computational translation of the Phaistos Disk,” Proc. 3rd International Conference on Applied Mathematics, Computational Science and Engineering, Agios Nikolaos, Crete, Greece, October 2015, pp. 53-57.
[20] M. Shortridge, T. Triplet, P. Z. Revesz, M. Griep, and R. Powers, “Bacterial protein structures reveal phylum dependent divergence,” Computational Biology and Chemistry, 35 (1), 2011, pp. 24-33.
[21] G. Varga, Bronzkori Magyar Irásbeliség, Irástörténeti Kutató Intézet publication, 1993.
[22] Wikipedia, “Phoenician alphabet,” downloaded July 6, 2015. Available: https://en.wikipedia.org/wiki/Phoenician_alphabet
[23] Wikipedia, “South Arabian alphabet”, downloaded July 5 2015. Available: https://en.wikipedia.org/wiki/South_Arabian_alphabet
[24] J. G. Young, "The Cretan Hieroglyphic script: A review article," Minos 31-32 (1996-1997[1999]) 379-400.
[25] G. Zaicz, chief editor, Etimológiai Szótár: Magyar Szavak és Toldalékok Eredete, (Etymological Dictionary: Origin of Hungarian Words and Affixes), Tinta Könyvkiadó, 2006.
Peter Z. Revesz holds a Ph.D. degree in Computer Science from Brown University. He was a postdoctoral fellow at the University of Toronto before joining the University of Nebraska-Lincoln, where he is a professor in the Department of Computer Science and Engineering. Dr. Revesz is an expert in databases, data mining, big data analytics and bioinformatics. He is the author of Introduction to Databases: From Biological to Spatio-Temporal (Springer, 2010) and Introduction to Constraint Databases (Springer, 2002). Dr. Revesz held visiting appointments at the IBM T. J. Watson Research Center, INRIA, the Max Planck Institute for Computer Science, the University of Athens, the University of Hasselt, the U.S. Air Force Office of Scientific Research and the U.S. Department of State. He is a recipient of an AAAS Science & Technology Policy Fellowship, a J. William Fulbright Scholarship, an Alexander von Humboldt Research Fellowship, a Jefferson Science Fellowship, a National Science Foundation CAREER award, and a “Faculty International Scholar of the Year” award by Phi Beta Delta, the Honor Society for International Scholars.
INTERNATIONAL JOURNAL OF COMPUTERS Volume 10, 2016
ISSN: 1998-4308 100