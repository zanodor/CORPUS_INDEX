---
master_file: "[[@ReveszPeterSumeriana]]"
---
# Index for Révész Péter – Sumerian Contains Dravidian and Uralic Substrates Associated with the Emegir and Emesal Dialects.pdf

Sumerian Contains Dravidian and Uralic Substrates Associated with the Emegir and Emesal Dialects
PETER Z. REVESZ Department of Computer Science and Engineering University of Nebraska-Lincoln Lincoln, NE 68588-0115 USA revesz@cse.unl.edu, http://cse.unl.edu/~revesz/
Abstract: - Data mining the Sumerian vocabulary reveals a dichotomy of the cognate associations of the Emeĝir and the Emesal dialects, with the former having mostly Dravidian and the later mostly Uralic cognates, indicating that Sumerian arose by the combination of two languages from those language families. The data mining also reveals a distribution pattern of Proto-Uralic, Proto-Finno-Ugric, Proto-Ugric and Proto-Hungarian cognates that indicates that Sumerian is farther than Minoan from Hungarian, although all are West-Ugric.
Key-Words: - computational linguistics, data mining, Dravidian, language family, Emesal, Sumerian, Uralic
1 Introduction
Some early Sumerologists (Lenormant, Oppert, Rawlinson) already noted similarities between Sumerian and Hungarian [55]. That line of work was extended by Badinyi [3], Baráth [4], Bobula [8], Csőke [10], Gosztonyi [19], Götz [20] and Tóth [46]. Unfortunately, they largely ignored Uralic linguistics in their work [23]. Simo Parpola [34] recently presented Uralic etymologies for over three thousand Sumerian words. Parpola’s idea of adding Sumerian to the Uralic language family is more credible. However, he did not consider the possibility that Sumerian is not only a Uralic language. The idea that Sumerian may belong to several language families is inspired by our earlier work on the Minoan language, whose vocabulary was to a large extent adopted by the ancient Greek language. We analyzed the ancient Greek vocabulary by looking for cognates in the following layers established by Uralic linguists [26]:
1. Uralic 2. Finno-Ugric 3. Ugric 4. Proto-Hungarian
The comparison yielded 22, 31 and 91 cognate ancient Greek words that belong to the Uralic, Finno-Ugric and Ugric layers, respectively. Beekes [5, 6] regarded most of those ancient Greek words as Pre-Greek, indicating that they could be borrowings from the earlier Minoan language in the
Aegean area. The Minoan language was written in the previously undeciphered Cretan Hieroglyph and Linear A scripts [12, 13, 14, 17, 18, 30, 31, 32, 33, 51, 52, 53] from which the earliest Greek script called Linear B developed [9, 49]. The surmised vocabulary, grammatical analysis, and some similarities within the Cretan Script Family [37], which includes the Minoan scripts, the Carian alphabet [2] and the Old Hungarian alphabet (called rovásírás in Hungarian) [15, 24, 43, 48], allowed the translation of over twenty texts (Revesz [38, 39, 40, 41]) with contents that fit into the Minoan cultural context [28]. Our translations suggested that Minoan, Hattic and Hungarian belong to a common (West)-Ugric branch of the Uralic language family [41]. Our work also implied that Greek is a descendant of two language families, i.e., both Indo-European and Uralic (see Fig. 3). That duality explains some of Greek’s unique features with respect to other Indo-European languages. The example of Greek raised the possibility that Sumerian may also be a language that belongs to several language families. That would explain why Sumerian has some word similarities with many languages. For example, Muttarayan [29] found many word similarities between Sumerian and Tamil. The rest of this paper is organized as follows. Section 2 presents an analysis of Sumerian and Uralic cognates that fall within the Uralic, FinnoUgric, Ugric and Proto-Hungarian layers. While doing the linguistic layer analysis, we discovered an interesting novel pattern. This pattern is that the Emesal dialect of Sumerian contains a
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 8 Volume 16, 2019



disproportionate number of the cognate words. Section 3 of this paper compares the Emesal and the Emeĝir dialects of Sumerian. The significant differences between these two dialects suggest an incomplete integration of two language families, namely, Dravidian and Uralic. The natural question that arises is which of the two language families existed earlier in Mesopotamia and which came later to the area. Section 4 considers this question by analysis of the vocabulary of the Euphratic language, which was suggested by Whittaker [50] and others as a substrate of Sumerian. Section 5 considers Sumerian and Hungarian phonetic correspondences. Section 6 considers Minoan and Hungarian language similarities and a parser for a subset of the Minoan language. Section 7 discusses the results and related work. Finally, Section 8 presents some conclusions and directions for future work.
2 Sumerian and Uralic Cognates
We collected possible Hungarian and Sumerian cognates by looking up the meaning of all the words that are listed as Uralic or Finno-Ugric by Zaicz [54] or are listed as Ugric by Honti [21] in the ePDS, the online version of the Pennsylvania Dictionary of Sumerian [44]. We also crosschecked all candidate cognates with the etymological dictionaries of Parpola [34] and Zaicz [54], the Mansi Dictionary of Munkácsi and Kálmán [27], the ancient Greek etymological dictionary of Beekes [5, 6], and the Hungarian-Greek dictionaries of Aczél [1] and Varga [47]. Table 1 shows the cognate groups that were collected. In Table 1 and in the rest of this paper, when x and y are words, then the notation x ~ y indicates that words x and y are cognates, x > y indicates a derivation from x to y and *x indicates a hypothetical form that is not attested in writing. The notation xL (m) denotes that x occurs in language L and means m in English. The similar consonant sounds are highlighted in red, inserted glide consonants are highlighted in blue, and omitted sounds are indicated by underscores. The third column in Table 1 is based on Parpola [34] and Zaicz [54] while the fourth column is based mostly on Beekes [5, 6] with a few minor additions. Our additions include in the row for ‘three’ the word háromszorHungarian (thrice) and its Mansi connection based on [27], and in the row for ‘sword’ its connections, including a possible borrowing of this word from Ossetian based on [54]. We also added a row for ‘lady, woman’ based on [27], although it is commonly thought to be a
borrowing from Alan language [54]. Finally, we also added the row for ‘breeze’ because the Hungarian and the Estonian words show a remarkable similarity, although Zaicz [54] claims that the Hungarian word is onomatopoeic in origin. In the Ugric group (shown by yellow color in Table 1), we extended Honti’s list by the row for ‘cry, yell.’ Each number in the last column of Table 1 refers to the Sumerian entry number in Parpola [34]. The dash --- indicates that no corresponding entry was found in Parpola [34]. Such dashes were rare in the Uralic and the Finno-Ugric entries and tended to be more frequent in the Ugric entries, indicating that the Ugric part of Parpola’s dictionary could still be significantly extended. The presence of the fourth column for ancient Greek adds a corroborative element because Greek has borrowed many Pre-Greek words from the Minoan language, which we already identified as an Ugric language. The Greek and Sumerian word pairs in Table 1 do not indicate direct borrowings from Sumerian to Greek but parallel borrowings from a Uralic substrate that preexisted in Anatolia and near by regions before the arrival of Sumerians in Mesopotamia and Greeks in the Aegean area. Table 2 and Fig. 1 compare the number of Hungarian and Sumerian cognates that were found with the number of Hungarian and ancient Greek or presumed Minoan cognates that were found in [41]. The total number of cognates found was nearly the same with 144 and 173, respectively. However, the ratio of Sumerian cognates divided by ancient Greek cognates showed an interesting pattern for the different layers They were 2.18 for the Uralic, 2.56 for the Finno-Ugric and only 0.51 for the Ugric layer. At the same time, we found a few Hungarian words with unknown origin that may be cognate with Sumerian words or ancient Greek or Minoan words. We did not gather statistics on these because a systematic search would need to consider a huge set of words, that is, much more than the few hundred well-established words that belong to the Uralic, Finno-Ugric and Ugric layers. However, the number of words that are not shared also with the Ob-Ugric group of Khanty and Mansi languages suggests that there was a West-Ugric language that was a common origin of Proto-Hungarian, ProtoMinoan and Proto-Sumerian. This West-Ugric hypothesis seems initially puzzling in light of the sharp drop of percentages shown in Table 2. It suggests a different survival rate for the words in various layers. Discovering the reasons for this differentiated survival was a major motivation for the experiments described in Sections 3 and 4.
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 9 Volume 16, 2019



Table 1. Uralic (blue), Finno-Ugric (green), Ugric (yellow), Greek and Sumerian cognate words.
English Hungarian Other Uralic or Finno-Ugric Greek Sumerian # slaughter _arat (harvest) širZyrian (cut, shear) šar2 --father atya ättäFinnish ad-da 39 mother anya anZyrian (husband’s mother) ἀμμά ama 102 hide (n.) bőr (skin) parvaFinnish (leather coat), pěrKhanty βυρσα bar 259 drop, drip csorog ćorkMansi, šoroFinnish (gurgle) sur 2277 water eső (rain) < esik (fall) isMansi (come down), äsSelkup (fall) ὕσμα eš 715 tree fa puuFinnish, pōSelkup mu 1927 back, rear, tail far peräFinnish _ουρα bar 241 trim with axe farag pārMansi, pārgeSelkup bar 255 eye, face fej (head) uopĭKhanty (look), vopMansi ὄψ < *ὄπις i-bí 1209 axe fejsze päćtMansi, pīčiSelkup pa-a-šu --fear (v.) fél pělKhanty, pelkääFinnish bu-luh 356 half, half-liquid fél pälMansi, palUdmurt πέλανος bar 269 box, chest fészek (nest) pesäFinnish pisaĝ 1998 blow (wind) fúj pŏγKhanty, powMansi πνειν bu7 346 saw (n.) fúr (drill) > fűrész puraFinnish (drill) πριων bùru (drill) 379 braid, weave1 fon pǎnKhanty (yarn), panne Saami (spin) υφαινειν1 pan 1952 bend fordul porjalVotyak (spin) bùru 377 wave hab (foam) kumpKhanty, kopMansi κυμα gúb (snow) 867 destroy hal (die) kălaKhanty, kālMansi, kouleFinnish (die) εκλειπειν hulu 1164 fish hal kouleFinnish, koleNganasan, kulZyrian ἰχθύς ku6 1423 walk, go halad koγelKhanty, kulkeFinnish kul 1446 three háromszor > *hármuszor > *ammusz (thrice)
χūrėm śosMansi (thrice) _am3-mu-uš --
boy here (scrotum) karKhanty (male) κορος ĝuruš 1092 raven, eagle1 holló kolākMansi kuléSelkup _ὄρνις hurin1 1192 length measure hosszú (long) košewMansi (long), kuźZyrian (length) _éše 712 urine húgy χǒsKhanty kaš3 --lie down huny (rest, close eye) kŏńKhanty, końMansi (close eyes) κοιμάω huna 1183 two két kitMansi, kaksiFinnish kad 1300 stone kő kawMansi kín 1392 sinew _ín tεnMansi, suoniFinnish τενων sa 2054 piece mar (bite) murtaFinnish (break) μερος mir 1083 go menni mińMansi, munZyrian, meneFinnish βαινειν ma --spouse meny (bride) meńKhanty, mińMansi (wife, bride) mudna --what mit (‘t’ is accus. suffix) mitäFinnish, midaEstonian _ta 2460 egg mony munujSelkup ωον nunuz --wash (hand) mos (wash) > mosdik moškaMari νιζειν maš (purify) 1654 woman, bride1 nő, néné (elder sister) nīMansi, naineEstonian νυμθη1 nu-nus 1917 kiss száj (mouth) sūpMansi (mouth), suuFinnish (mouth) še su-ub --run szalad suotiFinnish sar --eye, e. makeupS szem silmäFinnish οφ-θαλμος šembi --heart szív sěmKhanty, šämMansi ša-ab 2286 sting szúr survaaFinnish (stab) sa --gather talál (find) tolaMari (come) dul --sea tó (lake) < tavu tuZyrian (rise), tulisZyrian (spring) θαλασσα idim --to fly toll (feather) tēlMansi, toYurak (feather, wing) dal 425 road, street út āχtMansi, ηutYurak οδος tilla2 --be wide vas (iron) > vastag (thick) vaskiFinnish (copper), bazaKamas (iron) peš 1961 gift, present ad (give) antaFinnish (give), andoMordvinian (feed) at-ta 52 old person _agg šoηγeMari šu-gi 2422 brain agy anzêlMari εγ-κεφαλος ugu 2696 sleep ágy (bed) āηkuSamoyed ù_ 2633 a stand _áll (to stand) ľūľiMansi (to stand) _ud-da --sleep álo-m udo-moMordvinian ù-di 2673
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 10 Volume 16, 2019



Table 1. continued
English Hungarian Other Uralic or Finno-Ugric Greek Sumerian #
ebb (s.) apály šupalZyrian (dry out) παλιρροια šub 2405 father-in-law após opMansi, appiFinnish πενθερος ab (old man) 29 cut, slaughter1 csap (hit) čapaFinnish σφαζω1 ša-ab 2292 snatch csen sandaMordvinian zi-in-zi-in 2991 shine (v.) csillog šŭlpĭKhanty, śülγMansi σελας zalag 2926 bowl csupor ćipišZyrian zabar --wide dagad (swell) dundiZyrian (swell) da-ma-al 420 a bird (crane) daru (crane) tareγKhanty, tarewMansi, turiZyrian dur --copulate dug (push into) tongoMordvinian <ĝeš> dug --gleam ég saχMansi (to be scorched) αυγη šeĝ6 2340 mongoose egér (mouse) hiiriFinnish (mouse) gilim 820 word ének (song) ääniFinnish (sound, noise) e-ne-èĝ 1264 watercourse _ér (brook, vein) soraFinnish (melting ice) sùr 2280 new year fest. év jákkeSami (year), ikäFinnish (age) akiti --wall, brick1 fal pălKhanty (fish sieve) πλινος1 ba-ar 1759 boy fiú püwMansi παις ibila --take captive fog pekatKhanty, vangatFinnish pag 1941 harvest fürt (bunch <of grapes>) perVotyak (bunch <of grapes>) buru14 --onion plot hagyma kośemMansi ki-šum-ma --to lie down hál kōlMansi, kelVotyak ku --ant hangya kaškējMansi kiši 1417 tail, rear hanyatt (backward) kuntstMordvinian (on back) kun --angry harag (anger) χorMansi (quarrel) χαλεπος _úrgu 2818 bite harap kurććiZyrian χαραγμα kur8 1476 home, dwell1 ház kotaFinnish οἴκησις1 gùd 875 to be dark homály χomχatasMansi, kimerZyrian (cloud) kana6 --scratch horzsol karśelMansi, kuralZyrian hur --vulva hölgy (lady) kalMansi (female) gal4-la --twenty húsz kosMansi εἴκοσι i-iz (many) --ewe juh _uuhiFinnish _ὄις (ram) _u8 2644 sword kard < kardOssetian kērMansi (iron), kärkiFinnish (blade) ĝiri 1079 rare, valuable kell (need) kelMari, kolZyrian (need) καλός (good) kal 1317 bread oven, pottery
kenyér keńirVotyak kerKhanty, küörMansi κεραμoς
gar3 gir4-mah
--
to bend kerül (go around) kieräFinnish gur8 --hand kéz kötKhanty, kätMansi kišib 1420 sickle könyök (elbow) könηiKhanty (elbow) kin 1391 smith kovács, cf. szép seppäFinnish (clever, smith) simug 2192 tunic köt (tie) > kötény (apron) kätiMansi (tie) χιτον kad (tie) 1302 dwell lak (dwelling) lakkEstonian, lakkaFinnish (attic) lug 1600 soul, breeze lélek lělMansi, lolZyrian lil 1574 beat, kick1 lök (push, shove) lykkääFinnish (push) λακτιζειν1 lah 2477 big, great magas (tall), nagy (big) naźZyrian (proud), mägiEstonian (mount) μεγας mah 1628 twin más (another) mātMansi (another), medZyrian (image) maš 1656 lord menny (sky) meńelMordvinian (sky), jumoMari (god) umun 652 measure mér määrittaFinnish mur-ra 1787 watch, guard őriz ursMansi uraš 2810 lower body segg (buttock) säηMansi(groin) sig-ba 2155 help segít čangodeMordvinian saĝ 2078 grass sövény (hedging) säwMansi (tress) šu-mu-un --hasten, hurry sürög šurkalaMari sar 2112 dense, thick sűrű sūräMansi, suuriFinnish sir-ra 2197 dry (adj.) száraz sorKhanty ξηρος šarag (v.) 2310 border szeg śakKhanty, čekMari zag 2897 split, slit szel silMansi, sali Finnish (cut into pieces) sil 2164
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 11 Volume 16, 2019



Table 1. continued
English Hungarian Other Ugric Greek Sumerian #
good szép (clever, beautiful) seppäFinnish (clever, smith) ze-eb 2945 scold szid šudalaMari, sättiFinnish στοβέω šid 2381 lance, spear szigony (harpoon) śoχri Mansi (pointed knife) šugur 2426 leather strap szíj sowMansi (leather), sääFinnish zà 2895 split, cleave szil > szilánk (shred) sil Mansi, saliFinnish sil 2164 dirge sír (cry, lament) surFinnish (mourn) zarah --breeze sziszeg (hiss) susisemaEstonian (hiss) sisig --kindle, excite szít sŏtat Khanty zid 2961 hunger szomjas (thirsty) śumemVotyak (hungry) išim --suck szopik sipγMansi, šupšaMari sub --border szoros (strait) sărtKhanty (narrow land strip) sur --pitch szurok śirZyrian sar 703 level, lay flat tapos (trample) tapteMari (hammer flat) tab 2466 winter storm tél (winter) talviFinnish (winter) dal 429 put, sit down1 tesz täįMansi (weave) τιθεναι tuš1 2617 base (of plant) tő teηMari ten 2512 axe > tyrant1 tőr (dagger) tirVotyak τυραννος1 dur 598 pierce tövik täwMansi, töykkiFinnish te_ 2505 ibex türök/tülök (horn) teuraFinnish (deer) durah 600 shoulder váll _olkaFinnish murgu2 --be való (exists) wălKhanty, velZyrian ma-al --slice vés väntKhanty, vezZyrian peš6 --palm frond vessző (twig) wazeMari (twig) peš 1967 voice, noise zúg šakteMari (play music) σιγμός (hiss) šeg12 --meadow alom (bed of straw) ilemKhanty (grass in shoe) λειμων hirim (grass) --father apa opKhanty, opMansi (father in law) abba 28 flood _ár larKhanty (floodplain) Ιλισός illu 1239 daughter girl, slave girl1
ara (daughter-in-law) årMansi (maternal relative)
κορη
ur5
kiraš1
2805 --
lady, woman asszony ~ χsīnAlan khåusä nēMansi (whimsical w.) ka-ša-an --axe fokos poγKhanty (needle’s eye) πελεκυς bulug (needle) 350 needle fúl (sting, prick) pulpMansi (cork) bulug 350 hot, heat hamu kolemMansi kúm --mound hant χomesKhanty, khåmśelMansi χωμα gan (rack) 751 split (v.) hasad kün-kaśmātMansi δι-χοστατειν haš 1129 a bird hattyú (swan) kotaηMansi (swan) gud-du7 --fat (adj.) hízik (fatten) katemKhanty γαστρωδης geš 1045 lift, carry hord kartMansi gur3-ru --drag húz kåtMansi (pluck, pull at) gid --heir ifjú (young man) äjKhanty (small)+püwMansi (boy) ibila < bil --barley köles (millet) kolasMansi (millet) κριθη kiraši 1407 joint, with1 íz jäsenFinnish, jötKhanty συν1 sa (sinew) 2054 watch les lāśiKhanty, läćMansi φυλασσειν igi la --sprout maláta βλαστημα mu (grow) 1728 wet (v.) márt (dip) măraKhanty, murMansi (sink) βρεχειν mar 1645 burn meleg (warm) mäliMansi (warm) bil2 --deep (adj.) mély mělKhanty, mälMansi βαρυς burud 379 cowherd mén (horse), ménes (herd) vāntMansi (herd) munu --bride, spouse1 menyül (as a bride) meńKhanty, mińMansi νυμθη mudna1 --ladle mer (scoop v.) mĕretKhanty (sink) emerah --lead, tin _ólom _olnaKhanty, wōlemMansi μολυβδος anna 124 cry, yell rí räššiMansi ri --squeeze sajtol (squeeze) šojleKhanty (goes down) θλιβειν zaĝa --dark, black sötét šätepMansi (get dark) σκοτος zud 3009 fall into pit süpped (sink) šēpMansi (sink, drawn) šub 2406
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 12 Volume 16, 2019



Table 1. continued
English Hungarian Other Ugric Greek Sumerian #
boil, cook sül < süt šitMansi σιτοποιειν zil 2981 wedge szeg (nail, spike) säηkMansi σφην saĝ 2072 side, edge szél sēlMansi us --dry up (field) szik śäχMansi (salt) ισχναινειν šeĝ 2340 song szó (word) săwMansi ασμα šumun-ša --extract szül (give birth) sēlMansi (get, seak) zal --bowl tál tūlMansi útul 2884 bury temet tåwMansi túm 2597 space, chamber1 telek (farm) tarimtKhanty (lies on ground) θαλαμος1 dal-ba-na --lamp (oil) tidó tujtMansi (moon) δολος itid (moon) 1278 needle tű tūγerKhanty, tālMansi (twig) dálla 433 torch tűz (fire) tütKhanty, tāwtMansi δας dal 430 lord, ruler _úr śåpėrMansi (big, powerful) še-er --woman ük (ancestor w.) ēkeMansi γυνη, Γαια gi-in (w. worker) --female (s.) üsző (cow) ěsKhanty (female animal) θηλεια eze (sheep) 723 bury, hide zug (nook, hiding place) suηKhanty (corner, nook) σχιζειν zé-èg --
Table 2. Statistical summary of cognate words.
Uralic Finno-Ugric Ugric Total
Ancient Greek 22 31 91 144
Sumerian 48 79 46 173
Sumerian
Ancient Greek 2.18 2.56 0.51 1.2
Fig. 1 The number of Uralic, Finno-Ugric and Ugric cognates with Ancient Greek and Sumerian
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 13 Volume 16, 2019



Table 3. Emesal and Hungarian (Uralic) cognates and Emeĝir and Tamil (Dravidian) cognates.
English Hungarian or Uralic Emesal # Tamil or Dravidian Emeĝir # slave ara (daughter-in-law) ere --- arad lady asszony ka-ša-an --- peṇ nin 1915 shepherd csaba ~ çobanTurkish su-ba --- kāpariTelegu gabar --wide dagad (swell) da-ma-al 420 paranta barag (spread) 297 word ének (song) e-ne-èĝ 1264 pāṭal (song) bala (converse) 1264 tree fa mu 1927 kāṭu (forest) ĝeš 1046 wall fal ba-ar 1759 gōḍaTelegu egar 633 eye fej (head) i-bí 1209 kaṇ (eye) igi 1220 three háromszor am3-mu-uš --- mūḍuTelegu peš 1961 bring hoz, húz ga 750 tīsukuniTelegu de --bring iramlik (go fast) ir --- tappiyōṭa (flee) de --bird madár mu-tin 1803 paṟavai buru4 385 y. woman manó (dwarf) mutin 1803 koosuKannada (child) kisikil --scorpion mar (bite) mir 1083 koruku ĝír 1083 cowherd mén (horse) > ménes (herd) munu --- māṭu (cow) unud --go menni (go) ma --- naṭa du, (ĝen) 516 lord menny (sky) umun 652 āṇ (man) en 652 spouse meny (bride) mudna --- thandhai (father) dam 434 determine mér (measure) mara 1648 aĝ2 --what mit (mi+’t’ accusative suffix) _ta 2460 eṉṉa ana 115 lord nem (breed) > nemes nam2
Emegir ? --- āṇ (man) na (man) 1809 woman nő nu-nus 1917 peṇ munus 1770 lament sír a-še-er --- kaṇṇīr (tears) anir --grass sövény (hedging) šu-mu-un --- pul bur --kiss száj (mouth) še su-ub --- muttam ne sub --good szép (beautiful) ze-eb 2945 nalla mu --heart szív ša-ab 2286 /tʃaŋk!/Malayalam šag --clear tiszta, šåliMansi (thin, clean) šadi --- melliya (thin) na deg --sheep üsző (young cow) eze 723 āṭukaḷ udu 2678 be való (exists) ma-al --- unikilōTelegu ĝal 1005 bury, hide zug (nook, hiding place) zé-èg --- mūlai ab-lal3 (nest) --
Table 4. Uralic (blue), Finno-Ugric (green), Ugric (yellow), uncertain origin (white), Euphratic and Tamil or Dravidian cognates.
English Hungarian Euphratic # Tamil or Dravidian dark red deres (grayishbrown) < dér (frost) darah < duru (wet) 442 civappu herd of wild a. gulya (cattle herd) gilim --- muṅgisaTelegu bull, ox gida (kid, deer calf) gud --- kāḷai fish hal ku 1423 min raven holló, kaarneFinnish hurin (eagle) 1192 kaḻukuTelegu (eagle) ruddy, furious hús (meat) huc --- civanta an animal liba (goose) irib --- vāttu (goose) ewe juh _u8 2644 āṭukaḷ (sheep) a pot korsó (jar) ukur --- pāṉai dog kutya ku --- nāy male, man nőstény (female) nitah 1901 āṇ ladle mer (scoop v.) emerah --- karaṇṭiyāl lance, spear szigony (harpoon) šugur 2426 īṭṭi dirge sír (cry, lament) zarah --- iṟutiyañcali ibex türök/tülök (horn) durah 600 malaiyāṭṭu needle tű dálla 433 sūdiTelegu lord _úr še-er --- kaṭavuḷ be wide vas (iron) > vastag (thick) peš 1961 paranta
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 14 Volume 16, 2019



Fig. 2 The number of Euphratic, Emesal and Emeǧir cognates with Hungarian or Uralic and Tamil or Dravidian
Table 5. Common suffixes between Hungarian and Sumerian.
English Hungarian Suffix Sumerian Suffix #
-g (frequentative) -g, ĝ
word ääniFinnish (sound) ének (song) < *éneg mu7 (make sound) e-ne-èĝ 1264 shine (v.) csill-an (gleam) csillog zalag 2926 needle fúl (sting, prick) bulug 350 breeze susisemaEstonian (hiss) sziszeg (hiss) sisig --dry (adj.) szár-az šarag (v.) 2310 smith szép (clever) simug 2192 voice, noise; breath szip (sniff) szipog zi-pa-aĝ2 --
-k (adjective former) -h
dark red dér (frost) duru (wet) darah 442 male nőst-ény (female) nitah --ladle mer (scoop v.) emerah --dirge sír (cry, lament) zarah --ibex tű türök/tülök (horn) dálla (needle) durah 600
-mány/mény, -vány/vény
(noun former) -mun
lord jumoMari (god) menny (sky) < *um-vány an (sky) umun 652 grass sző (weave) sövény (hedging) šu-mu-un --
-r (frequentative) -r
herd csokor, ćukerZyrian šah2 (pig) --bowl csepp (drop of water) csupor zabar --lance, spear szeg (spike, nail)
szig-ony (harpoon) saĝ (wedge) šugur 2426
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 15 Volume 16, 2019



Table 6. Regular consonant sound correspondences within the West-Ugric group of languages: Minoan as shown by borrowings in Greek, Hungarian, and Sumerian. The West-Ugric consonant is the likely common origin. The reconstruction also needs to consider the context of other vowels and consonants. See the text for details. # West
Ugric Greek Hungarian Sumerian Initial Medial Final
1 š /ʃ/ τ - s τενων ~ ín ~ sa
- š /ʃ/ αυγη ~ ég ~ šeĝ6
2 /tʃ/ σ cs /tʃ/
s csorog ~ sur
š /ʃ/ σφαζω ~ csap ~ ša-ab
z σελας ~ csillog ~ zalag
3s
σ s /ʃ/ š σκοτος ~ sötét ~ šuš ὕσμα ~ eső ~ eš más ~ maš
z σιτοποιειν ~ sül ~ zil
σ sz /s/
s szalad ~sar sziszeg ~ sisig
š /ʃ/ στοβέω ~ szid ~ šid hosszú ~ éše
θ z szeg ~ zag θηλεια ~ üsző ~ eze
σz
s συν ~ íz ~ sa
š /ʃ/ σιγμός ~ zúg ~ šeg kéz ~ kišib
z σχιζειν ~ zug ~ zé-èg
4 d λ, τ d d daru ~ dur δολος ~ tidó ~ itid στοβέω ~ szid ~ šid
5 t τ t τυραννος ~ tőr ~ dur két ~ kad
t τιθεναι ~ tesz ~ tuš
ty /c/ d atya ~ ad-da
6 β β b b βυρσα ~ bőr ~bar
7 mp μ κυμα ~hab ~ gúb
8p
π, - f b πριων ~ fúr ~ bùru παις ~ ifjú ~ ibila
φ p υφαινειν ~ fon ~ pan
p b apa ~ abba szép ~ ze-eb
9h χ
h
- χαλεπος ~ harag ~ úrgu
κ, - h κοιμάω ~ huny ~ huna
10 k
χ g χωμα ~ hant ~ gan
κ ĝ /ŋ/ κορος ~ here ~ ĝuruš
χ k χαραγμα ~ harap ~ kur8
g g szigony ~ šugur zúg ~ šeg12
ĝ /ŋ/ segít ~ saĝ szeg ~ saĝ
γ, κ k g κεραμoς ~ kenyér ~ gar3 γυνη ~ ük ~ gi-in lak ~ lug
k καλός ~ kell ~ kal
11 l λ l l lak ~ lug σελας ~csillog ~ zalag toll ~ dal
ρ r ὄρνις ~ holló ~ hurin fal ~ ba-ar
12 r λ, ρ r rí ~ ri χαλεπος ~ harag ~ úrgu βυρσα ~bőr ~bar
13 m
β m b βαρυς ~ mély ~ burud
μ m μερος ~ mar ~ mir hamu ~ kúm alom ~ hirim
ny /ɲ/ ἀμμά ~ anyu ~ ama
14 n ν n n νυμθη ~ néné ~ nu-nus ménes ~ munu υφαινειν ~fon ~ pan
μ ny /ɲ/ κοιμάω ~ huny ~ huna menny ~ umun
15 v v m való ~ ma-al sövény ~ šu-mu-un tavu ~ idim
p vas ~ peš
16 - - j - ὄις ~ juh ~ u8 szíj ~ zà
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 16 Volume 16, 2019



3 Emesal Ugric and Emeĝir Dravidian
This section presents a dialect analysis of the Sumerian language. The Sumerian language is known to have two major dialects, namely the Emeĝir dialect and the Emesal dialect, which differ on several important words. The existence of several words for the same concepts commonly results from borrowing words from another language. For example, English is a Germanic origin language with an extensive borrowing from Romance languages due to its developmental history. As a result English has many word pairs for the same concept, such as freedom and liberty, food and aliment etc. Hence the question naturally arose whether Emeĝir and Emesal manifest a similar phenomenon or do the same. Table 3 shows that many Emesal words have Uralic cognates. For example, maEmesal (to go) seems cognate with menniHungarian (to go), while duEmeĝir (to go) is not cognate with Uralic words. However, duEmeĝir (to go) may be cognate with naṭaTamil (to go). Similarly, muEmesal (tree) seems cognate with puuFinnish (tree), while ĝešEmeĝir (tree) may be cognate with kāṭuTamil (forest). Table 3 shows a total of 31 Emesal-Emeĝir word pairs that show the same distribution. The Emesal words are all cognate with Hungarian words while the Emeĝir words are all cognate with Tamil or other Dravidian words. The finding in Table 3 explains why Sumerian is difficult to classify. Sumerian seems to be a language that inherited features from both the Uralic and the Dravidian language families, which is a combination that is not seen in other languages. In addition, Sumerian is known only from writing, and most of the extant Sumerian writing was done not by the Sumerians themselves but by Akkadians and Babylonians, who may have conformed some Sumerian words to their own preferred pronunciations. Therefore, it is rather remarkable to detect the emergent pattern in Table 3. It is probably difficult to identify with complete confidence what words are of Dravidian and Uralic origin because these two languages were already fairly well integrated in Sumerian society. However, some words by their meaning may be more naturally associated with the north than with the Indian subcontinent. For example, durSumerian (a bird) may be cognate with daruHungarian (crane). Cranes are migrating birds and Uralic people from the north would have been familiar with them and could have brought their name to Mesopotamia. Similarly, the word dérHungarian (frost), which describes a condition that is rare in Mesopotamia,
may have become duruSumerian (wet). Similarly, the words su-baEmesal (shepherd) and munuEmesal (herd) are commonly associated with the herding large groups of animals on the Eurasian Steppe and not with the agricultural life along the riverbeds of Mesopotamia. Hence their Hungarian etymologies are not surprising. Nor is it surprising that subaEmesal (shepherd) may be cognate with çobanTurkish (shepherd) because some Turkic people may have shared the Eurasian Steppe shepherding lifestyle. As another example, šu-mu-unEmesal (grass) is cognate with sövényHungarian (hedging), which is derived from szőHungarian (weave) and vényHungarian (noun forming suffix). It is possible that this ‘grass’ was hemp or some other crop, whose fibers were used to weave cloth. Such plants may have been planted at the edge of fields as hedging. A Sumerian word related to cooking is ki-šummaSumerian (onion plot), which may be cognate with kośemMansi (onion) + mø̄ Mansi (land) and maaFinnish (land). The hemp and onion plants also may have come to Mesopotamia from the north. Metallurgy was more developed in the mountain regions of the north, where metals could be mined. Therefore, the Sumerians may have borrowed simugSumerian (smith) from the people in the north, and it is likely cognate with seppaFinnish (clever, smith) as also described in item 2192 of Parpola [34].
4 Euphratic is an Ugric Language
Since Sumerian apparently resulted from a combination of two language families, it raises the question of when the two languages arrived to Mesopotamia. What was the original language of Mesopotamia? Whittaker [50] identified an early substrate language within Sumerian that he called Euphratic. The Euphratic language vocabulary seems to be a set of words that occur in the earliest extant Sumerian texts and share certain characteristic endings and morphologies. We have considered the set of Euphratic words as identified by Whittaker [50]. Table 4 and Fig. 2 show that at least eighteen Euphratic words have Uralic etymologies. We also considered whether these eighteen words have Dravidian etymologies, but we found some resemblance only in three cases. The case for ‘eagle’ being a cognate is weakened by the fact that it is not found in Tamil but only in Telegu. Moreover, there is a mismatch between the /n/ in hurinEuphratic and the /k/ in kalukuTelegu. The word hollóHungarian seems to omit an earlier /n/ ending as suggested by kaarneFinnish. In āṇTamil the similarity is only one letter. Finally, the gudEuphratic and kāḷaiTamil may indeed be cognate. Cattle were
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 17 Volume 16, 2019



likely introduced from one area to the other. Hence the name for cattle may be a trade word that spread widely at the earliest stages of cattle domestication. Therefore, even if these words are cognate, they are more likely to be associated with the movement of cattle as a trade good than with the movement of a large number of people. We also made some effort to identify the other Euphratic words in Whittaker [50] as either Dravidian or Uralic but failed to find more cognates. Hence, Euphratic is most likely Uralic.
5 Sumerian and Hungarian Regular Phonetic Correspondences
Parpola [34] did not present regular phonetic correspondences. Below we give a reconstruction of West-Ugric phonetics and show regular phonetic correspondences among three of its members: Hungarian, Minoan and Sumerian. It is only appropriate to talk about phonetic correspondences, denoted by ~, among those three, while it is possible to talk about phonetic changes, denoted by >, from West Ugric to them. Table 6 summarizes the sixteen main phonetic correspondences among Greek words with PreGreek, that is Minoan origin, and Hungarian and Sumerian based on the cognates collected in Table 1. We reconstructed the West-Ugric phonemes by considering all members, the Ob-Ugric forms, and the assumed phoneme repertoire at the beginning of the Proto-Hungarian period [26]. Table 6 gives the International Phonetic Alphabet notation, where the pronunciation may not be obvious. Each row of Table 6 can be taken as a separate correspondence rule between Hungarian and Sumerian and two derivation rules, one from WestUgric to Hungarian and another from West-Ugric to Sumerian. Rule (1): The following triplets in Table 1 demonstrate that West-Ugric preserved the word initial /ʃ// as did Sumerian, while Hungarian lost it:
_aggHungarian ~ šoηγeMari ~ šu-giSumerian
_aratHungarian ~ širZyrian ~ šar2
Sumerian
_érHungarian ~ soraFinnish ~ sùrSumerian
_ínHungarian ~ suoniFinnish ~ saSumerian
_úrHungarian ~ śåpėrMans ~ še-erSumerian
It may be supposed from the third and fourth examples that in West-Ugric and Sumerian even the world initial /s/ could have been preserved. In that case those /s/ had to change to /ʃ/ before the Hungarian sound change sequence /ʃ/ > /h/ > /_ / began.
Rule (2): West-Ugric word initial /͡tʃ/ was likely preserved in Hungarian, changed to /s/, /ʃ/, or /z/ in Sumerian and to σ in Greek. Rule (3) West-Ugric word initial /s/ Hungarian, changed to /s/, /ʃ/, or /z/ in Hungarian and Sumerian and to σ or may be θ in Greek. Rule (4): The West-Ugric /d/ is preserved in both Hungarian and Sumerian. Rule (5): The West-Ugric word initial /t/ is always preserved in Hungarian. It is also preserved in Sumerian when the following consonant is a bilabial /b/, /p/, /v/ or a nasal /m/ or /n/:
taposHungarian ~ tapteMari ~ tabSumerian
temetHungarian ~ tåwMansi ~ túmSumerian
tövikHungarian ~ täwMansi ~ te_Sumerian
tőHungarian ~ teηMari ~ tenSumerian
Sumerian changes the West-Ugric word initial /t/ to /d/ when the following consonant is /l/ or /r/:
találHungarian ~ tolaMari ~ dulSumerian
télHungarian ~ talviFinnish ~ dalSumerian
telekHungarian ~ tarimtKhanty ~ dal-ba-na Sumerian
tollHungarian ~ tēlMansi ~ dalSumerian
tőrHungarian ~ tirVotyak ~ durSumerian
türökHungarian ~ teuraFinnish ~ durahSumerian
tűHungarian ~ tālMansi ~ dállaSumerian
If an initial vowel is inserted, then the /t/ does not change in Sumerian even if the following consonant is /l/ or /r/:
tálHungarian ~ tūlMansi ~ útulSumerian
tidóHungarian ~ tujtMansi ~ itidSumerian
A West-Ugric word medial /t/ undergoes palatalization to /c/ in Hungarian:
atyaHungarian ~ ättäFinnish ~ ad-daSumerian
hattyúHungarian ~ kotaηMansi ~ gud-du7
Sumerian
In the first example the gemination is preserved even as /t/ changes to a /d/. In the second example the West-Ugric and the Ugric forms probably had also a geminate /t/, which is preserved in both Hungarian and Sumerian. A West-Ugric final /t/ is preserved in Hungarian and changes to /d/ in Sumerian:
kétHungarian ~ kitMansi ~ kadSumerian
sötétHungarian ~ šätepMans ~ zudSumerian
or changes to a fricative /ʃ/ or /z/ in Hungarian or both:
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 18 Volume 16, 2019



húzHungarian ~ kåtMansi ~ gidSumerian
kézHungarian ~ kätMansi ~ kišibSumerian
The last example suggests either an incipient word final /t/ to fricative change in West-Ugric, which was continued only in Hungarian, or more likely an influence from the ibSumerian (hips; middle) suffix. While kézHungarian normally means the palm of the hand, kišibSumerian more likely meant the wrist or forearm. Rule (6): West-Ugric word initial *β is preserved in both Hungarian and Sumerian:
bőrHungarian ~ pěrKhanty ~ bar
The presence of word initial /b/ not only in the Hungarian and Sumerian words but also in the cognate ancient Greek work βυρσαGreek, suggests that the change from /p/ to /b/ already occurred West-Ugric and it was not a separate event in Hungarian and Sumerian. Rule (7): The West-Ugric word final consonant cluster /mp/ changes to /b/ in both Hungarian and Sumerian:
habHungarian ~ kumpKhanty ~ gúbSumerian
Rule (8): The West-Ugric word initial /p/ always changes to /f/ in Hungarian, while in Sumerian it changes to /b/ if the consonant following it is a liquid /l/ or /r/:
falHungarian ~ pălKhanty ~ ba-arSumerian
farHungarian ~ peräFinnish ~ barSumerian
faragHungarian ~ pārMansi ~ barSumerian
félHungarian ~ pälMansi ~ barSumerian
félHungarian ~ pělKhanty ~ bu-luhSumerian
fokosHungarian ~ poγKhanty ~ bulugSumerian
fordulHungarian ~ porjalVotyak ~ bùruSumerian
fúlHungarian ~ pulpMansi ~ bulugSumerian
fürtHungarian ~ perVotyak ~ buru14
Sumerian
The West-Ugric word initial /p/ is preserved in other cases:
faHungarian ~ puuFinnish ~ paSumerian
fejszeHungarian ~ päćtMansi ~ pa-a-šuSumerian
fészekHungarian ~ pesäFinnish ~ pisaĝSumerian
fogHungarian ~ pekatKhanty ~ pagSumerian
fonHungarian ~ pǎnKhanty ~ panSumerian
The Hungarian change from /p/ to /f/ occurs only word-initially, except in compound words:
ifjúHungarian = iHungarian (young) + fiúHungarian (male)
A version of the above compound word could have been formed even in West-Ugric, that is, before the Hungarian word initial /f/ to /p/ change took place. Therefore, it looked like the following:
*ipiuWest-Ugric
In the above word the medial /p/ would have changed to /b/ in Sumerian, which is a regular phenomemnon:
apaHungarian ~ opKhanty ~ abbaSumerian
csuporHungarian ~ ćipišZyrian ~ zabarSumerian
ifjúHungarian ~ *ipiuWest-Ugric ~ ibilaSumerian
The West-Ugric word final /p/ also changes regularly to /p/ in Hungarian and /b/ in Sumerian:
süppedHungarian ~ šēpMansi ~ šubSumerian
szépHungarian ~ seppäFinnish ~ ze-ebSumerian
szopikHungarian ~ sipγMansi ~ subSumerian
taposHungarian ~ tapteMari ~ tabSumerian
Rule (9): West-Ugric word intitial /h/ is either preserved or omitted. The omission seems more common in longer words.
halHungarian ~ kălaKhanty ~ huluSumerian
háromszorHungarian~χūrėmśosMansi~_am3-mu-ušSum.
hollóHungarian ~ kolākMansi ~ hurinSumerian
horzsolHungarian ~ karśelMansi ~ hurSumerian
hosszúHungarian ~ košewMansi ~_éšeSumerian
hunyHungarian ~ kŏńKhanty ~ hunaSumerian
All of the above examples are from the ProtoUralic layer except horzsolHungarian, which is from the Finno-Ugric layer. That suggests that the initial /k/ already underwent lenition to /h/ in Proto-WestUgric. Moreover, in the second example the Mansi word also underwent partial lenition. An alternative would be to assume that WestUgric words did not have an initial /h/ but only an initial /k/. In that case, they underwent lenition idependently in Hungarian and Sumerian as discussed in the next rule. Rule (10): The West-Ugric initial /k/ has underwent various degrees of lenition. In Hungarian, word initial /k/ changes to /h/ when it followed by a back vowel:
habHungarian ~ kumpKhanty ~ gúbSumerian
hagymaHungarian ~ košemMansi ~ ki-šum-maSumer.
halHungarian ~ kouleFinnish ~ kuSumerian
hálHungarian ~ kōlMansi ~ kuSumerian
haladHungarian ~ koγelKhanty ~ kulSumerian
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 19 Volume 16, 2019



hamuHungarian ~ kolemMansi ~ kúmSumerian
hanyattHungarian ~ kuntstMordvin ~ kunSumerian
hangyaHungarian ~ kaškējMansi ~ kišiSumerian
harapHungarian ~ kurććiZyrian ~ kur8
Sumerian
hattyúHungarian ~ kotaηMansi ~ gud-du7
Sumerian
házHungarian ~ kotaFinnish ~ gùdSumerian
hereHungarian ~ karKhanty ~ ǧurušSumerian
homályHungarian ~ χomχatasMansi ~ kana6
Sumerian
hordHungarian ~ kartMansi ~ gur3-ruSumerian
hölgyHungarian ~ kalMansi ~ gal4-laSumerian
húgyHungarian ~ χǒsKhanty ~ kaš3
Sumerian
húzHungarian ~ kåtMansi ~ gidSumerian
In all of the above examples, the middle column has always a back vowel. In addition, at least either the Hungarian or the Sumerian cognate also has a back vowel after the word intitial consonant. These suggest that their Proto-West-Ugric ancestors also had a back vowel after the word initial /k/. The deep vowel nature of the West-Ugric word for hereHungarian is further confirmed by the cognate κοροςGreek.
In addition, the ki-šum-maSumerian (onion plot) probably derives from:
kośemMansi (onion) + mø̄ Mansi (plot, land)
because the Mansi forms seems to preserve well the original West-Ugric forms. It is likely that the later Sumerians did not understand that in the above compound word the syllable mø̄ meant ‘plot, land.’ Instead, they were expecting the beginning of the word to mean land, which is kiSumerian (place). Therefore, by folk etymology the following change could have occurred:
*kośem+mø̄ > *kiśem+mø̄ > ki-šum-maSumerian
There is no lenition of /k/ in Hungarian when it is followed by a front vowel:
kézHungarian ~ kätMansi ~ kišibSumerian
kellHungarian ~ kelMari ~ kalSumerian
könyökHungarian ~ könηiKhanty ~ kinSumerian
Rule (11): The West-Ugric word initial /l/ is always preserved. However, the West-Ugric word medial and final /l/ could either stay /l/ or change to an /r/. Here are a few examples for the latter:
falHungarian ~ pălKhanty ~ ba-arSumerian
félHungarian ~ pälMansi ~ barSumerian
hollóHungarian ~ kolākMansi ~ hurinSumerian
szaladHungarian ~ suotiFinnish ~ sarSumerian
vállHungarian ~ _olkaFinnish ~ murgu2
Sumerian
In the fourth example, there is a /t/ for the Finnish word, but a Finnish medial /t/ often corresponds to an Ugric /l/. Hence it can be assumed that the Proto-West-Ugric form also had a /l/ sound. Rule (12): The West-Ugric /r/ is always preserved in Hungarian and Sumerian, although it could change to a λ in Greek:
aratHungarian ~ širZyrian ~ šar2
Sumerian
bőrHungarian ~ pěrKhanty ~ bar Sumerian
csuporHungarian ~ ćipišZyrian ~ zabarSumerian
daruHungarian ~ tarewMansi ~ durSumerian
érHungarian ~ soraFinnish ~ sùrSumerian
farHungarian ~ peräFinnish ~ barSumerian
faragHungarian ~ pārMansi ~ barSumerian
fordulHungarian ~ porjalVotyak ~ bùruSumerian
fürtHungarian ~ perVotyak ~ buru14
Sumerian
harapHungarian ~ kurććiZyrian ~ kur8
Sumerian
hereHungarian ~ karKhanty ~ ǧurušSumerian
hordHungarian ~ kartMansi ~ gur3-ruSumerian
merHungarian ~ měretKhanty ~ emerahSumerian
tőrHungarian ~ tirVotyak ~ durSumerian
türökHungarian ~ teuraFinnish ~ durahSumerian
úrHungarian ~ śåpėrMans ~ še-erSumerian
Rule (13): The West-Ugric word initial /m/ can be preserved or changed to /ɲ/ in Hungarian, and it can be preserved or changed to /b/ in Sumerian when the following consonant is a liquid:
melegHungarian ~ mäliMansi ~ bil2
Sumerian
Rule (14): The West-Ugric word initial /n/ can be preserved or changed to /ɲ/ in Hungarian, and it is always preserved in Sumerian. Rule (15): The West-Ugric word initial /v/ is always preserved in Hungarian, and it can change to either /m/ or /p/ in Sumerian. The change from /v/ to /b/ occurs when the following consonant is a liquid /l/ or /r/ or a nasal /m/ or /n/:
sövényHungarian ~ säwMansi ~ šu-mu-unSumerian
vállHungarian ~ _olkaFinnish ~ murgu2
Sumerian
valóHungarian ~ wălKhanty ~ ma-alSumerian
Rule (16): A West-Ugric word initial or word final hiatus, that is a lack of consonant, is preserved in Sumerian but may be filled in by /j/ in Hungarian. For example:
juh Hungarian ~ uuhiFinnish ~ u8
Sumerian
szíjHungarian ~ sowMansi ~ zàSumerian
Rules (1-16) give a convincing proof that there
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 20 Volume 16, 2019



are regular phonetic correspondences between Sumerian and Hungarian. Next we give more detailed arguments that show that Hungarian, Minoan and Sumerian belong to the West-Ugric group of languages.
5.1 Finno-Ugric η > Ugric ηk > West-Ugric g
Honti [22] lists the Finno-Ugric η > Ugric ηk change as item 4 among the evidences for a common Ugric language. The ηkUgric > gHungarian change occurs regularly. Below we show some examples that suggest that Minoan and Sumerian also shared the ηk > g change with Hungarian. Hence this change occurred in Proto-West-Ugric.
*äηɛFinno-Ugric > *äηkɛUgric
> jaηlelKhanty (burn)
> *ägɛWest-Ugric
> αυγηGreek (torch) > égHungarian (burn)
*šiηereFinno-Ugric > *šiηkereUgric
> täηkerMansi (mouse)
> *šegérWest-Ugric
> ζεγέριεςGreek (mouse) > egérHungarian (mouse) > gilimSumerian (mongoose ?)
*suηɛFinno-Ugric > *suηkɛUgric
> suηKhanty (crack) > *sugɛ > σχιζεινGreek (crack, v.) > zugHungarian (crack, n.) > zé-ègSumerian (bury, hide)
*θäηɛFinno-Ugric > *θäηkɛUgric
> tawMansi (bough)
> jaγiKhanty (bough)
> *ägɛWest-Ugric
> ἀκρέμωνGreek (bough) > ágHungarian (bough)
In each of the above four examples, the ancient Greek and Sumerian words are closer to the Hungarian words than to the Khanty and Mansi words because they also contain /g/ or the similar phonemes /k/ or /x/. Furthermore, the ancient Greek and Sumerian words preserve some archaic features that probably existed in West-Ugric but were lost in Hungarian. These archaic features include the presence of an ending vowel in αυγηGreek and the initial fricative consonant in ζεγέριεςGreek. These support the
hypothesis of a West-Ugric branch within the Finno-Ugric family that included both Minoan (from which ancient Greek borrowed the above words) and Hungarian.
5.2 Finno-Ugric lm > Ugric m = West-Ugric m
Honti [22] lists the lmFinno-Ugric > mUgric change as item 5 among the evidences for a common Ugric language.
*ćolmeFinno-Ugric
> solmuFinnish (knot)
> *ćomeUgric, West-Ugric
> ἁμμαGreek (knot) > csomóHungarian (knot)
The lm > m change did not occur in some ObUgric words perhaps because of a vowel insertion between the /l/ and the /m/, but it occured in the West-Ugric words. Here is an example:
*kuδ’mɛFinno-Ugric
> kuloνMordvinian (ash)
> kōlemMansi (ash)
> *kumɛWest-Ugric
> κόνιςGreek (dust) > hamuHungarian (ash) > kúmSumerian (hot, heat)
5.3 The Ugric -kVj Suffix
Honti [22] lists the Ugric -kVj suffix as item 19 among the evidences for a common Ugric language. This suffix appears in the word for woodpecker.
*karɛ-kVjUgric (woodpecker) > kar-kājMansi > *karɛ-kVjWest-Ugric
> κραυ-γόςGreek (woodpecker) > har-kályHungarian (woodpecker)
6 West-Ugric Grammar Similarities
The Sumerian grammar is already described in several textbooks, for example by Foxvog [16], Gosztonyi [19] and Thomsen [45]. Among those authors, Gosztonyi [19] gives a detailed comparison between Sumerian and the Hungarian grammars. While Sumerian clearly does not fit neatly into the Uralic family tree, Gosztonyi’s list of similarities supports the hypothesis that Sumerian is a mixed Dravidian and Uralic language. The Dravidian and Sumerian grammatical comparisons also need to be
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 21 Volume 16, 2019



developed and listed in a similar manner to [19] before being able to decide which language family’s grammatical features are present and to what degree. Complicating the picture somewhat is the fact that Dravidian and Uralic languages are both agglutinative and share some other features. For these common features one cannot decide whether they are inherited from one or the other language family. To strengthen the proposal of a West-Ugric branch of the Uralic language family [41], we list some of their grammatical similarities. We focus on the similarities between Minoan and Hungarian because the Sumerian grammar is already compared with Hungarian as noted before.
6.1 West-Ugric is an Agglutinative Language
Sumerian [19] and the Uralic languages [26] are agglutinative, that is, they append suffixes to word roots without changing those roots. Duhoux [12] already identified Minoan to be also an agglutinative language. As further evidence, in Table 6 we display some blocks of the Phaistos Disk and the Arkalochori Axe that reveals an agglutinative structure, in particular the following:
1. There are eight different endings that each occurs at least two different times.
2. Some endings are apparently optional. For
example, L B is optional because it occurs in block 6 but does not occur in block 2.
Similarly, V is optional because it occurs in block 36 but not in block 44.
3. Some endings are replaceable with another ending. For example, blocks 29 and 38 have the
same apparent root but end with c and G, respectively. Similarly, blocks 33 and 40 have
the same apparent root but end with c and a, respectively.
4. Whenever the endings are attached to a root, the root does not change. Table 6 indicates by red some of the apparent roots.
6.2 Minoan has a CVCV Root Structure
Linear B, the immediate descendant of Linear A, has a mostly syllabic writing with CV type syllables, where C is a consonant and V is a vowel [9, 49]. Hence Linear A was expected to have a similar structure as was verified in [41]. The CV type syllables fit well with Proto-Uralic word roots
that generally have two syllables with a CVCV structure [26] as shown by the following examples:
*kala > hal (fish) *käte > kéz (hand) *mete > méz (honey)
Words with a CVCV structure can be written down conveniently using two CV syllabic symbols, which may have influenced the Linear A script to develop as a syllabic script. Table 6 already shows several roots that contain two Linear A symbols,
including A M and Z e and G s.
6.3 The -g Frequentative Suffix
Table 5 shows that Hungarian and Sumerian words share the –g suffix, which suggests that the Euphratic language also had this suffix. The –g suffix is a frequentative suffix that derives from a Finno-Ugric *ŋk suffix (Zaicz [54]). Here are some examples:
szipogHungarian (sniff) ~ zi-pa-aĝ2
Sumerian (breath)
sziszegHungarian (hiss) ~ sisigSumerian (breeze)
6.4 The -k Adjective Former Suffix
Table 5 shows that Hungarian and Sumerian words share the –k adjective former suffix, which can be traced back to a *-k Finno-Ugric suffix. In some early written documents in Hungarian, this suffix appears as –h, although it later changed to an –ó/ő suffix by assimilation to the vowels at the end of root words (Zaicz [54]). It is possible that the following two words are cognate:
tűHungarian (needle) ~ dállaSumerian (needle)
The above suggests that the Hungarian word was originally either *tűr or *tűl. It probably meant not only needle but horn too. The ibex is an animal that is notable for its large horn. Hence a synonym for ibex may be horny, with a literal meaning of having a prominent horn. That explains the following word pairs:
türökHungarian (horn) ~ durahSumerian (ibex)
6.5 The -mány/-mény Noun Former Suffix
Table 5 shows that Hungarian and Sumerian share the –mány-/mény, noun former suffix, which can also appear in the form of -vány/vény, as shown by the following examples:
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 22 Volume 16, 2019



sövényHungarian (hedging) ~ šu-mu-unSumerian (grass)
As mentioned above, the Hungarian word derives from sző (weave) and sövény may have meant some grassy plant, whose fibers were used for weaving. Another example is the pair:
mennyHungarian (sky) ~ umunSumerian (lord)
The mennyHungarian may derive from *um-vány, where the /v/ assimilates to the preceding /m/ and yields umunSumerian. The original meaning may be god, who is assumed to dwell in the sky, that is, a heavenly person. Later this was generalized to mean lord, which is the dictionary entry for Sumerian word.
6.6 The -r Frequentative Suffix
Table 5 also shows that Hungarian and Sumerian also words share the –r frequentative suffix, which can be traced back to an *-r Finno-Ugric suffix. For example:
csupor Hungarian (bowl) ~ zabar Sumerian (bowl)
The above apparently derives from cseppHungarian (drop of water). Hence csuporHungarian initially meant a bowl that collected drops of water, perhaps rain drops. A nail and a spear are similar to each other in both having a pointed end. A nail is normally used only once during a construction of something. In contrast, a spear is used several times. Hence it needs a frequentative suffix:
szegHungarian (spike, nail) ~ šugurSumerian (spear)
Similarly, a Sumerian word that means a single pig can be put together with a Hungarian word that means herd as follows:
csokor Hungarian (herd) ~ šah2
Sumerian (pig)
Since csokorHungarian is cognate with ćukerZyrian, the word derives from West-Ugric to Sumerian and not vice versa. That makes sense because pigs were first domesticated in Anatolia and not in Mesopotamia.
6.7 Other Suffixes Ending with /k/
A problem with a pure syllabic script is that many suffixes do not fit into a CV structure. For example, consider the following Hungarian suffixes that end with a /k/ phoneme. We also give some examples,
as they appear in the earliest Hungarian language documents. One of the frequently consulted documents is the 12th century Halotti Beszéd (Funeral Sermon) [7], which will be referenced as HB below.
1. /-ak, -ek, -ok/ are for the plural of words that end in a consonant. The vowel is chosen according to vowel harmony rules. Some examples are hal-ak (fishes) and kez-ek (hands) and ablak-ok (windows).
2. k/ is the plural of words that end in a vowel. For example, falu-k (villages) or kapu-k (gates).
3. /-k/ is the 1st person singular present tense verbal suffix in the indeterminate case.
4. /-juk, -jük/ is the 1st person plural present tense verbal suffix in the determinate case. For example, tümet-jük (we bury) appears in HB. As another example, present Hungarian uses számol-juk a pénzt (we count the money).
5. /-juk/ is also the 3rd person plural possessive suffix. For example: kutyá-juk (their dog).
6. /-muk/ is the 1st person plural present tense verbal suffix in the indeterminate case. This appears as vogy-muk in HB. This suffix appears to be simply the composition of the /-om, em/ first person singular verbal suffix in the determinate case and the plural /-k/, ex: olvasunk (we read a book).
7. /-nak, -nek/ is the third person plural present tense verbal suffix in the indeterminate case, for example, esz-nek (they eat).
8. /-nak, -nek/ is also a marker of the possessor of an object. For example, a ló-nak a lába (the horse's leg).
9. /-nak, -nek/ is also a lativus suffix. For example, fal-nak megy (goes to a wall), hegy-nek fordul (turns towards a mountain).
10./-omk/ is the 1st person plural possessive suffix, which appears as uromc [ur-omk] (our lord) in HB. Etymologically, this suffix appears to be simply the composition of the first person possessive /-om, -am, -em/, as in ház-am (my house) and the plural /-k/. Today, this suffix appears as /-unk, -ünk/, as in ház-unk (our house).
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 23 Volume 16, 2019



Table 7. Some blocks of the Phaistos Disk and the Arkalochori Axe inscriptions arranged to reveal repeatedly used suffixes and word roots. The Arkalochori Axe symbols are transliterated into the Phaistos Disk symbols using [39]. Block Possible Root (red) Possible Suffix (blue) Block Possible Root (red) Possible Suffix (blue)
12 R W JY a B
45 A a I B
51 n j Z B
59 E W k B
Ark. 3 W F S B
3 Ukiaa LB
6 AM LB 2 AM
9 aRfNa LB
10 Z e L B 7 L Z e
20 l W f L B
22 i S o L B
24 R F L B
27 g n D L B
61 G n V L B
34 G W i F B
Ark. 1 S N m J i F B
28 h c c
29 G s c 38 G s G
33 Y W h c 40 Y W h a
43 M H c
47 A g c
49 i T X X c
37 X R W G
39 i R G
52 i n X G 30 L n X
25 H r a
26 L G s a
50 A l Y a
60 i G s a
36 H G j c V 44 H G j c
53 Y p k V
58 a Y V
Ark. 2 o Z B Y V
8 SQR F
46 g m f i F
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 24 Volume 16, 2019



The Minoan B symbol represents not a syllable but some single phoneme because it is used only at the end of the words with one exception. According to Table 7, in the Minoan language
about half of the suffixes end with a B symbol. Remarkably, about half of the suffixes end in /k/ in Hungarian. Therefore, it is tempting to associate
Minoan B with Hungarian /k/. Moreover, the above Hungarian suffixes could be grouped into three groups: (1-3), which have the form /Vk/, where the vowel V is optional, (4-5), which have the form /jVk/, and (6-10), which probably had the form /-mVk/ assuming m > n or n > m changes in some cases. These groups seem to match a natural grouping of the Minoan words into those that end
with B, with L B and with i F B, respectively. Old Hungarian contains two letters that denote
the /k/ phoneme: and . According to some researchers one letter was used only within the words and the other was used only at the end of words. When carving the symbols into wood, a diamond is a convenient simplification of a circle, which may have denoted a human head [48].
Therefore, the shapes of the Minoan B symbol
and the Old Hungarian symbol have a connection. Moreover, the Minoan symbol depicts the head of a man with prominent hair. The Mansi word for man is /kom/, while the ancient Greek word for hair was /komi/, which may have been borrowed from Minoan. This shows a /k/ or a /ko/ phonetic connection between the two symbols.
6.8 Conjunction
Table 8 shows another pair of blocks that allows us
to suspect that the symbol R is a conjunction symbol, meaning “and,” a disjunction symbol, meaning “or,” or it is some prefix. The shape of this symbol read from left-to-right suggests that it may denote two paths that merge together, that is, a conjunction. When rotated ninety degrees, the symbol also reminds one of the Old Hungarian symbol, which denotes the /ʃ/ phoneme and occurs in the Hungarian words s and és that both mean “and.”
6.9 Assimilation by Consonant Doubling
Table 9 shows the doubling of some symbols before the hypothetical suffixes. The doubling of consonants before suffixes is common in Hungarian and result from assimilation between the last
Table 8. Possible Minoan conjunction or affix. Block Conjunction or Prefix Root Suffix
6 AM LB
31 R A M L B
Table 9. Two blocks contain a doubling of some symbols right before possible suffixes.
Block Possible Root Doubling Possible Suffix
3 Uki aa B
49 i T X X c
Table 10. Hungarian assimilation with consonant doubling. Root + juk Suffix Assimilation mosjuk (we wash) /ʃ ʃ/ úszjuk (we swim) /s s/ főzjük (we cook) /z z/ hagyjuk (we let) /ɟ ɟ/ hunyjuk (we close [eyes]) /ɲ ɲ/ bátyjuk (their older brother) /c c/
Table 11 Hungarian assimilation without doubling. Root + juk Suffix Assimilation mondjuk (we say) /ɟ/ fonjuk (we weave) /ɲ/ futjuk (we run) /c/
Table 12. Minoan assimilation without doubling. Block Root Assimilation Suffix
22 i S o L B
Ark. 3 W F S B
Table 13. Minoan and Old Hungarian script similarities.
Symbol
Grammatically Identified Phoneme
Old Hungarian Letter
Old Hungarian Phoneme
B /k/ /k/
L /j/ /j/ or /λ/
R /ʃ/ /ʃ/
a /s/, /z/, /ɟ/, /ɲ/ /c/ , /s/, /ʒ/
X /s/, /z/, /ɟ/, /ɲ/ /c/ /z/
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 25 Volume 16, 2019



consonant of the root and the beginning consonant of the suffix. Table 10 shows some examples.
Therefore, the Minoan a and X symbols behave similarly to the Hungarian doubled consonants and likely denote one of the consonants that is doubled in Hungarian except /ʃ/, which we already
associated with R.
6.10 Assimilation by Palatalization
Assimilation can occur without a doubling in case of some consonants. Table 11 gives some examples from Hungarian. The palatalized sounds in Table 11 may not have been originally used in the Hungarian language within word roots, but they tend to occur naturally with the addition of suffixes that start with /j/. It is likely that in the Minoan language the palatalized sounds also first occurred as a result of assimilation. Table 12 shows that in block 22 a palatalization during assimilation can be suspected because the apparent assimilation yields a symbol that is rarely used. Moreover, it is never used at the beginning or the end of words, where palatalization is absent. It
is also noticeable that it occurs only before LB, which we already associated with the /–juk, -jük/ suffix. Compare Phaistos Disk block 22 with the Arkalochori block 3, where there is no assimilation
sound in a similar context before B which we associated with the /–Vk/ suffix. The above grammatical comparisons enable the identification of the phonetic values of some of the Phaistos Disk symbols as shown in the first two columns of Table 13. It is apparent from Table 13 that the Old Hungarian alphabet has a strong connection with the Minoan symbols. After such a realization, the logical step was the thorough comparison of all Minoan and Old Hungarian symbols to identify possible phonetic values of the Minoan symbols [37]. The script comparison was recently extended to the Indus Valley Script [11]. Fig. 3 shows our proposal [40] to place Minoan into West-Ugric branch of the Uralic language family. Fig. 3 implies that Minoan and Hungarian share not only the characteristic Ugric features but also the characteristic West-Ugric features, that is, the language innovations that occurred after the separation of West-Ugric and Ob-Ugric and before the separation of Minoan and Hungarian. Linguists call Proto-Hungarian (ősmagyar in Hungarian) the language that separated from the Ob-Ugric branch and progressed toward present day Hungarian until
the end of the 9th century [21, 26]. Hence these characteristic West-Ugric features can be none other than some of the Proto-Hungarian linguistic innovations that were previously considered to be pertinent only to the evolution of the Hungarian language. Hence the precise identification of the characteristic West-Ugric features is tantamount to dividing the ősmagyar period into an early phase, which is applicable to Minoan too, and a later phase, which is not applicable to Minoan but only to Hungarian. Below we give some features that are shared by Minoan and early Proto-Hungarian. These shared features support putting these two languages into a common West-Ugric branch of the Uralic language family.
6.11 The Ugric Root+Possessive+Case Order Finally, Honti [22] lists the word structure:
Root + Possessive + Case
order as item 20 among the evidences for a common Ugric language. The translation of the Arkalochori Axe [40] includes the word szem-jöd-nek (for your eye), which has the root+possessive+case order. Hence Minoan also has this structure. According to Foxvog [16] p. 28, Sumerian has the same structure. Hence West-Ugric probably had the same structure too.
6.12 A Parser for Minoan Possessive Phrases
Both Minoan and Hungarian possessive phrases are composed of a possessor followed by the possessed object. Both the possessor and the possessed object are indicated by suffixes. The possessor is indicated by a /-nak/ suffix, while the possessed object is indicated by an /-a/ suffix. Similarly, in Sumerian the possessor is indicated by a /-ak/ suffix (Foxvog [12], p. 39). In Minoan and Hungarian, the possessor suffix /-nak/ is optional and can be omitted. Table 14 shows that the Phaistos Disk contains two examples of this structure. Although
we identified i F B with /-nak/, the I symbol has the syllabic value /na/, hence the combination
I B is another way of writing the /-nak/ suffix. A computer program can be also written to look for adjacent pairs of blocks with the first ending in /nak/, expressed in any form, and the second ending with /-a/. A context-free-grammar [36] or a constraint query language [25] can be used to express Minoan possessive phrases. In terms of a
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 26 Volume 16, 2019



context-free-grammar the Minoan possessive phrases can be expressed as follows:
Pphrase à Possessor Possessed Possessor à Nd –nak | Nh –nek | Nd | Nh Nd à NdSingular | NdPlural Nh à NhSingular | NhPlural NdSingular à NdC | NdV NhSingular à NhC | NhV NdPlural à NdC -ak | NdV –k NhPlural à NhC -ek | NhV –k NdC à <deep vowel nouns ending in consonant> NhC à <high vowel nouns ending in consonant> NdV à <noun with deep vowels ending in vowel> NhV à <noun with high vowels ending in vowel> Possessed à PossessedSingular | PossessedPlural PossessedSingular à NdC –a | NdV –ja | NhC –e | NhV -je PossessedPlural à PossessedSingular -i
In the above grammar, the terminals are indicated by brackets < >, choices by |. Each time a possessive phrase is parsed, the grammar starts at Pphrase, which stands for “possessive phrase.” The possessive nouns can be either singular or plural. Plural possessive nouns ending with a vowel have a /-k/ suffix, while those ending with a consonant have either an /-ak/ or an /-ek/ suffix according to vowel harmony rules. Similarly, the vowel harmony rules require an /-a/ or an /-e/ to indicate being possessed. In addition, the phoneme /j/ is inserted before the last two as a gliding sound if the noun ends with a vowel. The possessed object or objects take first the /-a/ suffix, indicating belonging to the preceding possessor and then the plural marker /i/. The different plural marker and the different order with respect to the main suffixes, that is, preceding /nak/ but following /-a/ also help distinguish between possessor and the possessed object(s). For example,
to possessive phrase “embereknek házai” (people’s houses) can be parsed as follows:
Pphrase à Possessor Possessed Possessor à Nh –nek Nh à NhPlural NhPlural à NhC -ek NhC à ember Possessed à PossessedPlural PossessedPlural à PossessedSingular -i PossessedSingular à NdSingular –a NdSingular à NdC NdC à <ház>
The above gives “ember-ek-nek ház-a-i,” which is the correct parsing of this possessive phrase.
7 Related Works and Discussion
Section 1 already mentioned many of the prior researchers who worked on identifying Sumerian and Hungarian parallels. Similar to them, Aczél [1] and Varga [47] worked on Greek and Hungarian parallels, building large dictionaries. Although they also ignored Uralic linguistics, their work called for an explanation. Our earlier work [41] found an explanation by recognizing that some of the word parallels may be due to a common proto-language of Minoan and Hungarian. Now the picture of language evolution can be further completed as shown in Fig. 3. The figure explains that Minoan and the related Hattic language belong to the Uralic family tree. Moreover, Greek is a descendant from both IndoEuropean and Uralic, while Sumerian has both Dravidian and Uralic ancestors. Fig. 3 implies some modification of the chronology of Uralic language evolution because West-Ugric had to exist before Sumerian and Minoan became separate languages. The precise chronology is often one of the hardest problems to identify in comparative linguistics. A comparison of two languages tells little directly about the chronology. Róna-Tas [42] estimated the separation of the Ob-Ugric languages from the rest of the Uralic family tree to have occurred between 3000 and 2000 BC. This is somewhat farther back in time then many other linguists’ estimates, but the time may still need to be pushed back more than a thousand years to accommodate the known Sumerian and Aegean chronologies.
Table 14. Minoan possessive phrases. Each Minoan phrase consists of two blocks. The translations are in Minoan below that in English (in italics). Blocks Possessor -nak Possessed -a
7-8 Z e S Q R F
fény light’s
tavasz-a spring
45-46
Aa IB gmfi F
más-nak king’s
húsz lány-a daughter
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 27 Volume 16, 2019



The basis of Róna-Tas’ estimate is actually far more interesting than the estimate itself. Róna-Tas makes the observation that certain processes of sound change could only occur in a sequence and not in parallel. For example, the process of wordinitial /ʃ/ > /h/ > /_ / changes, that is, the gradual loss of the initial /ʃ/ must have occurred before the process of word-initial /k/ > /h/ changes, when /k/ is followed by a back vowel, started. Otherwise, the /k/ initial would have also completely disappeared. Clearly, if the first process lasted x number of years, the second process lasted y number of years, then we can conclude that the evolution of a language in which both processes occurred in a sequence took at least x + y number of years. However, we cannot derive any upper bound because there could have been some number of extra years before the first process ended and the second process started. While the elapse time of a process could be estimated relatively well, estimating the extra years seems highly uncertain. Therefore, Róna-Tas’ work implies that the separation of the Ob-Ugric languages from the rest of the Uralic family tree occurred at least 2500 BC (± 500 years for various uncertainties in estimating the duration of the sound change processes).
8 Conclusions and Future Work
It has always looked counterintuitive to have Sumerian be a language isolate given its location in Mesopotamia, which is essentially at the intersection of three continents. It turns out that instead of being a language isolate, Sumerian is actually the combination of at least two major language families. In this paper we identified Dravidian and Uralic and in particular Proto-Tamil and Proto-Hungarian, respectively within those two language families as major contributors to the development of Sumerian. It cannot be excluded currently that a third language to be still identified also contributed to Sumerian. It seems that the great difficulty in classifying the Sumerian language was not its isolation but its varied interconnections with several other languages. There still remains much work to be done to fill in the details of the picture shown in Fig. 3. In particular, as Section 9 mentioned, the chronology of the development of Sumerian and its related languages needs to be worked out in detail. It is hoped that the complete settling of the Sumerian language will shed a major light on the origins and prehistory of languages in general [35].
Fig. 3. A partial diagram showing the Dravidian (yellow), Indo-European (red) and the Uralic (blue) language families. Note that the Greek (purple) and the Sumerian (green) languages descend from two different language families.
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 28 Volume 16, 2019



Acknowledgements: The author would like to thank the J. William Fulbright Program for supporting him on two Fulbright Scholarships. First, on a visit to the University of Athens, Greece, in 2008, and second, to Budapest, Hungary, in spring 2017 to the Aquincum Institute of Technology, an affiliate of the Budapest University of Technology and Economics. An earlier version of this paper was presented in July 2018 at the 22nd International Conference on Circuits, Systems and Communications in Mallorca, Spain.
References: [1] J. Aczél, Szittya-Görög Eredetünk (Our Scythian-Greek Origin), Turán Publ., Garfield, NJ, USA, 1975. [2] I.J. Adiego, The Carian Language, Koninklijke Brill NV, Leiden, Netherlands, 2007. [3] F. J. Badinyi, New lines for a correct Sumerian phoenetics to conform with the cuneiform scripts, Proc. 29th International Congress of Orientalists, 1973. [4] T. Baráth, A Magyar Népek Őstörténete (The Prehistory of the Hungarian People), Vols. 1-5, Somogyi Publ., Franklin Park, New York, USA, 1974.
[5] R. S. P. Beekes, Etymological Dictionary of Greek, Brill NV, Leiden, Netherlands, 2009.
[6] R. S. P. Beekes, Pre-Greek Phonology, Morphology, Lexicon, Brill NV, Leiden, Netherlands, 2014.
[7] L. Benkő, Az Árpád-kor magyar nyelvű szövegemlékei, Budapest, Hungary, ELTE, Régi Magyar Irodalomtudományi Intézet, 1980. [8] I. Bobula, Sumerian affiliations; A plea for reconsideration, (manuscript), Washington D.C., USA, 1951.
[9] J. Chadwick, The Decipherment of Linear B, Cambridge University Press, 1958.
[10] S. Csőke, Szumir-Magyar Egyeztető Szótár (Sumerian-Hungarian Correspondences Dictionary), Turáni Akadémia Publishing, Buenos Aires, Argentina, 1974. [11] S. Daggumati, P. Z. Revesz, Data mining ancient script image data using convolutional neural networks, Proc. 22nd International Database Engineering and Applications Symposium, New York, ACM Press, 2018, pp. 267-272.
[12] Y. Duhoux, The Journal of Indo-European Studies, Vol. 26 (1-2), 1-38, 1998.
[13] A. J. Evans, Scripta Minoa: The Written Documents of Minoa Crete with Special Reference to the Archives of Knossos, Volume II, Classic Books, 1909.
[14] G. M. Facchetti, and M. Negri, Creta Minoica: Sulle Tracce delle più Antiche Scritture d'Europa, L.S. Olschki, Firenze, 2003.
[15] S. Forrai, The Old Hungarian Writing from Ancient Times to the Present, (in Hungarian), Antológia Kiadó, 1994. [16] D. A. Foxvog, Introduction to Sumerian Grammar, manuscript, University of California at Berkeley, 2012. [17] L. Godart and J.-P. Olivier, Recueil des inscriptions en Linéaire A (Études Crétoises 21), De Boccard, 1976. [18] C. H. Gordon, Evidence for the Minoan Language, Ventnor Publ., Ventnor, NJ, 1966.
[19] K. Gosztonyi, Dictionaire D'etymologie Sumerienne et Grammaire, De Boccard Publ., Paris, France, 1975.
[20] L. Götz, Keleten Kél a Nap (The Sun Rises on the East). Püski Publ., Budapest, Hungary, 1989.
[21] L. Honti, Az Ugor Alapnyelv Kérdéséhez, (To the Question of the Proto-Ugric Language), KEL Print, Budapest, Hungary, 1997. [22] L. Honti, Characteristic features of Ugric languages (observations on the question of Ugric unity), Acta Linguistica Academiae Scientiarum Hungaricae, Vol. 29, No. 1/2, 1979, pp. 1-26.
[23] L. Honti, ed., A Nyelvrokonságról - Az török, Sumer és Egyéb Áfium Ellen Való Orvosság, Tinta Publishing, Budapest, Hungary, 2010.
[24] G. Hosszú, Heritage of Scribes: The Relation of Rovas Scripts to Eurasian Writing Systems, Rovas Foundation Hungary, 2013. [25] P. C. Kanellakis, G. M. Kuper, P. Z. Revesz, Constraint Query Languages, Journal of Computer and System Sciences, Vol. 51, No. 1, 1995, pp. 26-52. [26] J. Kiss and F. Pusztai, eds., A Magyar Nyelvtörténet Kézikönyve (Handbook of Hungarian Language History), Tinta Publ., Budapest, Hungary, 2018. [27] Mansi Dictionary of Munkácsi and Kálmán, downloaded June 22, 2018. Available: http://www.babel.gwi.unimuenchen.de/munka/index.php
[28] N. Marinatos, Minoan Kingship and the Solar Goddess: A Near Eastern Koine, University of Illinois Press, 2010. [29] K. L. Muttarayan, Sumerian, Tamil of the First Cankam, Journal of Tamil Studies, Vol. 8, 1975, pp. 40-61. [30] G. Nagy, Greek-Like Elements in Linear A, Greek, Roman, and Byzantine Studies Vol. 4, No. 4, 1963, pp. 181-211.
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 29 Volume 16, 2019



[31] J.-P. Olivier, Cretan Writing in the Second Millennium B.C., World Archaeology, Vol. 17, No. 3, 1986, pp. 377–389. [32] J.-P. Olivier, L. Godart and J.-C. Poursat, Corpus Hieroglyphicarum Inscriptionum Cretae (Études Crétoises 31), De Boccard, 1996. [33] G. A. Owens, The Structure of the Minoan Language, Journal of Indo-European Studies. Vol. 27, No. 1–2, 1999, pp. 15–56.
[34] S. Parpola, Etymological Dictionary of the Sumerian Language, Vols. 1 and 2, Helsinki, Finnland, Foundations for Finnish Assyriological Research, 2016.
[35] G. Revesz, The Origins and Prehistory of Language, New York, Philosophical Library, 1956.
[36] G. E. Revesz, Introduction to Formal Languages, New York, McGraw Hill, 1983. [37] P. Z. Revesz, Bioinformatics Evolutionary Tree Algorithms Reveal the History of the Cretan Script Family, International Journal of Applied Mathematics and Informatics, Vol. 10, No. 1, 2016, pp. 67-76. Available: http://www.naun.org/main/UPress/ami/2016/a1 82013-133.pdf [38] P. Z. Revesz, A Computer-Aided Translation of the Phaistos Disk, International Journal of Computers, Vol. 10, No. 1, 2016, pp. 94-100. Available:http://www.naun.org/main/NAUN/co mputers/2016/a282001-455.pdf [39] P. Z. Revesz, A Computer-Aided Translation of the Cretan Hieroglyph Script, International Journal of Signal Processing, Vol. 1, No. 1, 2016, pp. 127-133. Available: iaras.org/iaras/filedownloads/ijsp/2016/0030017.pdf [40] P. Z. Revesz, A Translation of the Arkalochori Axe and the Malia Altar Stone, WSEAS Trans. on Information Science and Applications, Vol. 14, No. 1, 2017, pp. 124-133. Available: http://www.wseas.org/multimedia/journals/info rmation/2017/a285909-084.pdf [41] P. Z. Revesz, Establishing the West-Ugric language family with Minoan, Hattic and Hungarian by a decipherment of Linear A, WSEAS Transactions on Information Science and Applications, Vol. 14, No. 1, 2017, 306335. [42] A. Róna-Tas and Á. Berta, eds., West Old Turkic: Turkic Loanwords in Hungarian. Harrassowitz Verlag, 2011. [43] G. Sebestyén, Rovás és Rovásírás, Magyar Néprajzi Társaság, Budapest, Hungary, 1909.
[44] The Pennsylvania Sumerian Dictionary,
Available: http://psd.museum.upenn.edu
[45] M.-L. Thomsen, The Sumerian Language: An Introduction to its History and Grammatical Structure, Akademisk Forlag, Copenhagen, Denmark, 1984.
[46] A. Tóth, Hungarian, Sumerian and Egyptian. Hungarian, Sumerian and Hebrew: Two Addenda to the Etymological Dictionary of Hungarian, Mikes International, Hague, Neitherlands, 2007.
[47] C. Varga, Ógörög: Régies Csángó Nyelv, (Ancient Greek: Old Csango Language), Fríg Kiadó, 2006.
[48] G. Varga, Bronzkori Magyar Irásbeliség, Budapest, Irástörténeti Kutató Intézet, 1993. [49] M. Ventris, J. Chadwick, Evidence for Greek dialect in the Mycenaean archives, The Journal of Hellenic Studies, Vol. 73, 1953, pp. 84-103. [50] G. Whittaker, The case for Euphratic, Bulletin of the Georgian National Academy of Sciences, Vol. 2, No. 3, 2008, pp. 156-168.
[51] F.C. Woudhuizen, The Earliest Cretan Scripts, Innsbrucker Beiträge zur Kulturwissenschaft, 2006. [52] J. G. Younger, Linear A texts and inscriptions in phonetic transcription, downloaded July 25, 2017. Available: http://www.people.ku.edu/~jyounger/LinearA/ [53] P. Yule, Early Cretan Seals: A Study of Chronology, Marburger Studien zur Vor und Frühgeschichte, 1981. [54] G. Zaicz, chief editor, Etimológiai Szótár: Magyar Szavak és Toldalékok Eredete, (Etymological Dictionary: Origin of Hungarian Words and Affixes), Tinta Könyvkiadó, 2006. [55] A. Zakar, Sumerian-Ural-Altaic Affinities, Current Anthropology, Vol. 12, No. 2, 1971, pp. 215-216.
WSEAS TRANSACTIONS on INFORMATION SCIENCE and APPLICATIONS Peter Z. Revesz
E-ISSN: 2224-3402 30 Volume 16, 2019