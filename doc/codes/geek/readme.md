# The Geek Code 4.1.0

The geek code attempts a concise description of your being in ‘geek space’, spanning key dimensions using a small set of categories and quantifying them with qualifiers ( or qualifying them with quantifiers, as you wish).

The code consists of a set of alphabetic identifiers indicating the various categories (and subcategories), and qualifiers + and – following the identifiers indicating amount/size/level of proficiency/etc. These qualifiers can be stacked, e.g s+++ indicates a person of extreme height (the s indicating size).

The rules for identifiers are:

* They are case sensitive
* They may not have numbers or special symbols
* They must be latin characters
  * Specifically, the regular expression `[a-zA-Z]` defines the acceptable set.
* They may, at most, be five letters long
* lower case symbols could be anyone, upper case symbols specifically refer to geeks (or whatever a derivative refers to, otherwise)

In general, they should strive to work in a similar sense to dewey decimal, where each subsequent character leads to more specific data with the minimum length possible. This is not strictly enforced, however.

The qualifiers `+` and `-` can be subject to run length compression. `++++` can also be expressed as `+4`; `-7` would mean `-------`. Zero (or, rather, the absence of qualifiers) is always given a positive sign. (Whether or not such compression is even used is up to the user or implementer, ultimately, but one should strive for either consistency or space optimization.) An exact value (where relevant) may be indicated with `=` followed by that value. If a sign does not preface the value, it should be considered to be that value, literally, as opposed to signifying one with a sign. (In most cases, the equals sign can and should be left out because it means the same thing as just writing it without it; however, in the case of the `age` field, for example, it can be used to indicate exact value for age.)

There are only - at most - 19 possible values for any given qualifier set. This is both to control how absurd some of these have gotten over the years, and limit how absurd they can conceivably get. Those values, on a number line, run the integers from -9 to +9. They do not all need to be specified; interpolation should be assumed, or the implication of some magnitude without a specific denotation.

The broad categories encoded are: Wetware, Computers, Politics, Entertainment, Lifestyle. Most have subcategories and you can answer at any level of detail desired, thus eg. U++ indicates someone highly interested/proficient in Unix, while ULDU++ indicates someone into unix-linux-debian-ubuntu. Multiple subcategories can be indicated with a forward slash, e.g GH/C indicates a Geek of Humanities and Classics.

Some categories will be irrelevant, so ignore them. Some of the qualifiers will not match with you exactly, so choose that qualifier that most closely matches you.

Given a set of category/qualifier strings for any of the above (skip anything you dont want to answer/not relevant/classified/unknown/indeterminate/etc) it’s time to assemble your code for displaying to the world. Take the substrings and concatenate with a space between. When completed, it will look something like the following:

```
GS/CS/J a+ b-- c- d+:- C+ ULDU+$   LC+/p+  FE- BE+ H+ PGP+ E+ P++/PS++/PSG++ TR&M+ B+ kX e++++ h++ r++ y+
```

Subject to optimal run length encoding, that would look  like:

```
GS/CS/J a+ b-- c- d+:- C+ ULDU+$   LC+/p+  FE- BE+ H+ PGP+ E+ P++/PS++/PSG++ TR&M+ B+ kX e+4 h++ r++ y+
```

A GEEK CODE BLOCK similar to the output created by PGP attempts to universalize how you will see the Geek Code around the net and looks like the following:
```
—–BEGIN GEEK CODE BLOCK—–
Version: 4.0.1
GS/CS/J a+ b-- c- d+:- C+ ULDU+$   LC+/p+  FE- BE+ H+ PGP+ E+ P++/PS++/PSG++ TR&M+ B+ kX e++++ h++ r++ y+
—–END GEEK CODE BLOCK—–
```
### Special characters

A few special characters allow for the (ultimately wrong but practically useful) notion that geeks can seldom be strictly quantified.

@

for this variable, said trait is not very rigid, may change with time or with individual interaction. For example, Geeks who happen to very much enjoy Star Trek: The Next Generation, but dislike the old 60’s series might list themselves as t++@.

()

for indicating “cross-overs” or ranges. Geeks who go from C+ to C— depending on the situation (i.e. mostly “C+”) could use C+(—). @ is different from () in that () has finite limits within the category, while @ ranges all over.

'>'

for ‘wannabe’ ratings. Indicating that while the geek is currently at one rating, they are striving to reach another. For example, C++>$ indicating a geek that is currently computer savvy, but wants to someday make money at it.

$

Indicates that this particular category is done for a living. For example, UL+++$ indicates that the person utilizes Unix and gets paid for it. Quite a lucky geek, for sure.

?

Unless stated otherwise within the specific category, the ? is placed after the category identifier and indicates that the geek has no knowledge about that specific category. For example, a person that has never even heard of Babylon 5, would list their Babylon 5 category as [FIXME]?

!

Placed BEFORE the category. Unless stated otherwise, indicates that the person refuses to participate in this category. This is unlike the ? variable as the ? indicates lack of knowledge, while the ! indicates stubborn refusal to participate. For example, !E would be a person that just plain refuses to have anything to do with Emacs, while E? would be a person that doesn’t even know what Emacs is.

## The categories

```
an alphabetic (unordered) shorthand

Note that this is just a short reference, and does not indicate the intended or mandatory ordering.

G - "Geek of..."


==============================================================
### G – Geek of - training/degree/interest/job

To start a code, a geek must declare himself or herself to be a geek. To do this, we start the code with a “G” to denote “GEEK”, followed by one or two letters to denote the geek’s occupation or field of study. Multi-talented geeks with more than one vocational training should denote their myriad of talents with a slash between each vocation (example: GCS/MU/TW).

```
GB — Geek of Business
GC — Geek of Classics
GCA — Geek of Commercial Arts
GCM — Geek of Computer Management
GCS — Geek of Computer Science
GCC — Geek of Communications
GE — Geek of Engineering
GED — Geek of Education
GFA — Geek of Fine Arts
GG — Geek of Government
GH — Geek of Humanities
GIT — Geek of Information Technology
GJ — Geek of Jurisprudence (Law)
GLS — Geek of Library Science
GL — Geek of Literature
GMC — Geek of Mass Communications
GM — Geek of Math
GMD — Geek of Medicine
GMU — Geek of Music
GPA — Geek of Performing Arts
GP — Geek of Philosophy
GS — Geek of Science (Physics, Chemistry, Biology, etc.)
GSS — Geek of Social Science (Psychology, Sociology, etc.)
GTW — Geek of Technical Writing
GO — Geek of Other. Some types of geeks deviate from the normal geek activities. This is encouraged as true geeks come from all walks of life.
GU — Geek of ‘Undecided’. This is a popular vocation with incoming freshmen.
G! — Geek of no qualifications nor interests; likely, cannot exist
GAT — Geek of All Trades. For those geeks that can do anything and everything. GAT usually precludes the use of other vocational descriptors.
```

### a – Age

The only way to become a true geek is through practice and experience. To this end, your age becomes an important part of your geekiness. Use the qualifiers below to show your age (in Terran years). Base 10 , wise guys.

```
a+9  120 and up
a+8  110-119
a+7  100-109
a+6   90- 99
a+5   80- 99
a+4   70- 79
a+3   60- 69
a+2   50- 59
a+    40- 49
a     30- 39
a-    25- 29
a–2   20- 24
a—3   15- 19
a—4   10- 14
a—5    0-  9

? immortal
! it’s none of your business how old I am

In addition, if you wish to give your exact age, you can place the number itself after ‘a=’. For example: `a=42`
```

### b – beardliness/facial hair
As facial hair plays some sort of role in geek space, serving as an expression of style, countercultural proclivities, etc. etc. and [unix beards](http://www.usenix.org.uk/content/unix_beards.html) being a thing we give it a category here despite its irrelevance to some fraction of the population. Also it lets us start off with ‘abcd’ for age/beard/clothing/dimensions

```
b – beard
bm – mustache
bs – sideburns
bb – bushy eyebrows
```
Thus b+9/bm+9 means impressive beard with equally consequential mustachio. Leave blank for no facial hair.

The `b` value (for beard) should be interpreted as more-or-less compliant with the 1.9.1 bear code, and thus can be specifically interpreted as the following (taken shamelessly from the Bear Code):

`b` - Little to no beard, or incredibly sparse. Such a beard is the absolute minimum that could ever be classified as a beard. We're talking 5-o'clock shadow, here!

`b+` - Very slight beard - this is the kind of beard that people have who want to grow a beard, but can't grow one. Or someone who is constantly at the 1-week phase.

`b+2` - Slight beard - A beard kept VERY short at all times, or thinned out.

`b+3` - Thin Beard - a beard in all respects but kept thin and short.

`b+4` - Mostly full - a beard that is full except for a few noticable bald spots, or kept trimmed.

`b+5` - Full beard - A full beard not generally trimmed, although not generally bushy. May have a few bald spots on inspection. Usually full and roundish beards fall into this category.

`b+6` - Very full - A full beard, not trimmed. May be slightly bushy but very full.

`b+7` - Longish/Bushy beards - A full beard or slightly thin beard with longish fhair. This beard is not trimmed and does come away from the chin.

`b+8` - Very long beards - These beards  are usually very bushy and haven't seen clippers for a very long time.

`b+9` - Belt buckle grazing long beards - The prototype is ZZ Top. Need one say more?

### c – Clothing
```
c++  I tend to wear conservative dress such as a business suit or worse, a tie.
c+  Good leisure-wear. Slacks, button-shirt, etc. No jeans, tennis shoes, or t-shirts.
c  I dress a lot like those found in catalog ads. Bland, boring, without life or meaning.
c-  I’m usually in jeans and a t-shirt.
c–  My t-shirts go a step further and have a trendy political message on them.
c—  Punk dresser, including, but not limited to, torn jeans and shirts, body piercings, and prominent tattoos.
cx  Cross Dresser
c?  I have no idea what I am wearing right now, let alone what I wore yesterday.
!c  No clothing. Quite a fashion statement, don’t you think?
cpu  I wear the same clothes all the time, no matter the occasion, forgetting to do laundry between wearings.
```
### d – dimensions
Geeks come in many shapes and sizes. The dimensions for a geek are divided into two parts - `dh` and `dw` - for height and weight. They are centered near what appears to be fairly average values of 100 kg and 170 cm. (If one must explain why it's in metric or how to convert, you may not be a geek.) (Well, okay, average global weight is about 70 kg, but I had to fit it into the chart and wanted 10 kg increments.)

#### dh - height

```
dh - height

dh-9    0 - 125 cm
dh-8  126 - 130 cm
dh-7  131 - 135 cm
dh-6  136 - 140 cm
dh-5  141 - 145 cm
dh-4  146 - 150 cm
dh-3  151 - 155 cm
dh-2  156 - 160 cm
dh-   161 - 165 cm
dh    166 - 170 cm
dh+   171 - 175 cm
dh+2  176 - 180 cm
dh+3  181 - 185 cm
dh+4  186 - 190 cm
dh+5  191 - 195 cm
dh+6  196 - 200 cm
dh+7  201 - 205 cm
dh+8  206 - 210 cm
dh+9     >= 211 cm

!dw - my height is none of your business!

You may specify your height in centimeters after `dh=`, such that `dh=120` would indicate a height of 120 centimeters.
```

#### dw - weight

```
dw - weight

dw-9    0 -  10 kg
dw-8   11 -  20 kg
dw-7   21 -  30 kg
dw-6   31 -  40 kg
dw-5   41 -  50 kg
dw-4   51 -  60 kg
dw-3   61 -  70 kg
dw-2   71 -  80 kg
dw-    81 -  90 kg
dw     91 - 100 kg
dw+   101 - 110 kg
dw+2  111 - 120 kg
dw+3  121 - 130 kg
dw+4  131 - 140 kg
dw+5  141 - 150 kg
dw+6  151 - 160 kg
dw+7  161 - 170 kg
dw+8  171 - 180 kg
dw+9     >= 181 kg

!dw - my weight is none of your business!

You may specify your weight in kilograms after `dw=`, such that `dw=120` would indicate a weight of 120 kilograms.
```


### e - Education
All geeks have a varying amount of education.

```
e+9 Considered the forefront expert
e+8 Considered more an expert than Doctors
e+7 finished Doctoral Degree
e+6 finished Master's Degree
e+5 finished Bachelor's Degree
e+4 finished Associate's Degree
e+3 finished 12th grade
e+2 finished 11th grade
e+  finished 10th grade
e   finished 9th  grade
e-  Finished 8th  grade
e-2 Finished 7th  grade
e-3 Finished 6th  grade
e-4 Finished 5th  grade
e-5 Finished 4th  grade
e-6 Finished 3rd  grade
e-7 Finished 2nd  grade
e-8 Finished 1st  grade
e-9 Finished Kindergarten

!e I never even went to school!

Equivalencies, for alternative programs or
expressions:

e-5 Finished Grade School
e-8 Finsihed Middle School
e+3 Finished High School
e+3 Finished GED Certification
e+4 Finished Apprenticeship
e+5 Finished Journeyman's
e+6 Finished Master Craftsman's

There are likely other programs I'm missing.
```

### h - Housing

Tell us about your geeky home.

```
h+6 Living in a cave with 47 computers and an Internet feed, located near a Dominoes pizza.

h+3 Living alone, get out once a week to buy food, no more than once a month to do laundry. All surfaces covered.

h Friends come over to visit every once in a while to talk about Geek things. There is a place for them to sit.

h-3 Living with one or more registered Geeks.

h-5 Living with one or more people who know nothing about being a Geek and refuse to watch Babylon 5.

h-7 Married, (persons living romantically with someone might as well label themselves h-8, you’re as good as there already.)

h-8 Married with children – Al Bundy can sympathize.

!h I am stuck living with my parents!

h? I’m not sure where I live anymore. This lab/workplace seems like home to me.
```

### k – Books

In addition (or maybe on the other hand), many geeks have lives that revolve around books.

```
B+8 I read a book a day. I have library cards in three states. I have discount cards from every major bookstore. I’ve ordered books from another country to get my Favorite Author Fix.

B+6 I consume a few books a week as part of a staple diet.

B+3 I find the time to get through at least one new book a month.

B+ I enjoy reading, but don’t get the time very often.

B I read the newspaper and the occasional book.

B- I read when there is no other way to get the information.

B-8 I did not actually READ the geek code, I just had someone tell me.
```

### l – Languages

Languages are divided into two categories as of now - `ln` : natural languages (spoken ones, generally) and `lP` : programming languages.

In general, the language qualifiers mean:

```
+9 - I invented the language!
+8 - I'm considered a forefront expert
+7 - I'm fluent at a high native level
+6 - I'm fluent at a modest native level
+5 - I'm fluent at a poor native level
+4 - I'm fluent as a high-level non-native
+3 - I'm fluent as a modest-level non-native
+2 - I'm fluent as a poor-level non-native
+1 - I'm just barely fluent enough to hold a conversation
+0 - I just barely can hold a conversation, but I wouldn't call myself "fluent" by any stretch.
-1 - I can hold a conversation in mildly limited tenses and/or within the 1000 most used words
-2 - I can hold a conversation in just a few tenses and/or within the 500 most used words
-3 - I can hold a conversation in one tense and/or within the 100 most used words
-4 - I can sort of read it, relying on cognates and familiar structures and terms
-5 - I cannot really read it, but a word or two comes through when I look at it
-6 - When I look at it, nothing makes sense to me.
-7 - I frequently make a fool of myself by mistaking it for another language entirely
-8 - I frequently make a fool of myself by pretending I know the language and then saying utterly gibberish
-9 - I have been told that what I call my level of proficiency is offensive to native speakers, who see me as a pretentious liar.

? - I didn't even know this was a language.

! - I refuse to acknowledge this language as legitimate, let alone discuss how well I speak in it.
```

Most natural languages people speak will have to be +5 or more. Most programming languages will wildly vary.

#### ln - natural languages

These codes are derived primarily from ISO-639-1. Please maintain consistency, as such. I have selected ones that I believe cover the vast majority of the world. As I am an ignorant, white American, I likely know nothing of the world, and I apologize in advance.

```
lnaf  - Afrikaans
lnbg  - Bulgarian
lncs  - Czech
lnde  - German
lnel  - Greek (modern)
lnen  - English
lnena - Australian English
lnenb - British English
lnenu - American English
lneo  - Esperanto
lnes  - Spanish/Castilian
lnet  - Estonian
lnfi  - Finnish
lnfr  - French
lnhe  - Hebrew
lnhi  - hindi
lnhr  - Croatian
lnhu  - Hungarian
lnid  - Indonesian
lnit  - Italian
lnja  - Japanese
lnjbo - Lojban
lnko  - Korean
lnlg  - Ganda
lnlo  - Lao
lnnl  - Dutch/Flemish
lnno  - Norweigian
lnnv  - Navaho
lnpl  - Polish
lnpt  - Portuguese
lnro  - Romanian
lnru  - Russian
lnzh  - Chinese
```

#### lP - programming, scripting, and markup languages

These are based on the 8+3 file extensions for each language listed in Pygments documentation. Where conflicts arise, a best attempt at something sensible has been made.

```
lPahk - AutoHotKey
lPasm - Intel/8086 Assembly
lPb   - Limbo
lPbbc - BBC Basic
lPbas - QBasic
lPbf  - Brainfuck
lPcbl - COBOL
lPc   - C
lPcl  - Common Lisp
lPcpp - C++
lPcs  - C#
lPerl - Erlang
lPf   - Fortran
lPfrt - Forth
lPgd  - GDScript
lPgo  - Go
lPhs  - Haskell
lPhtm - HTML
lPhx  - Haxe
lPinf - Inform 6 source
lPino - Arduino
lPjav - Java
lPjs  - Javascript
lPm   - Matlab
lPmd  - Markdown
lPobc - Objective C
lPpas - Pascal/Delphi
lPphp - PHP
lPpl  - Perl
lPpy  - Python
lPr   - R
lPrb  - Ruby
lPrs  - Rust
lPrst - reStructuredText
lPsql - SQL
lPtex - TeX/LaTeX
lPts  - Typescript
lPvb  - Visual Basic
lPxml - XML
````

### m - comics and manga

Use this to offer your opinion on comics and manga.

The prefixes should not be used alone, but should help in categorizing these a little better. (Actual valid identifiers follow this listing.)

* `mm` - manga

  * `mmjm` - Manga serialized in a Jump publication, which forms much of America's manga and anime exposure.

   * `mmkd` - Manga serialized in a Kondasha publication, because some of my favorites turn out to come from there

   * `mmyk` - Manga serialized in a Young King publication.

* `mc` - comics

    * `mcac` - comics from Archie Comics

    * `mcdc` - comics from DC, best known for Justice League and Teen Titans

    * `mcuf` - comics from United Features Syndicate, best known for newspaper comics

* `mv` - visual novels

* `mw` - webcomics

The list of valid identifiers follows.

```
mcufd - Dilbert
mmjma - Assasination Classroom
mmjmb - Bleach
mmjmd - Dragon Ball (and Z/Super)
mmjmf - Fist of the North Star
mmjmg - Barefoot Gen
mmjmh - YuYu Hakusho
mmjmj - Jojo's Bizarre Adventure
mmjml - Death Note
mmjmn - Naruto
mmjmo - One Piece
mmjmr - Rurouni Kenshin
mmjms - Saint Seiya / Knights of the Zodiac
mmjmv - Video Girl Ai
mmjmy - Yu-Gi-Oh
mmkda - Akira
mmkdc - Cyborg 009
mmkdf - FLCL
mmkdg - Ghost in the Shell
mmkdl - Love Hina
mmkdo - The Big O
mmkds - Sailor Moon
mmkdt - Attack on Titan
mmkdw - Wolf's Rain
mmykh - Hellsing
mmykt - Trigun/Trigun Maximum
mwxkc - XKCD
```

This list should be considered incomplete. I'm literally just sick of punching in entries for it at this moment.

### o - orientation

This should be considered a position on the Kinsey Scale, with `+0` on this scale centered at `3` on the traditional Kinsey scale. Thus negative numbers are increasingly heterosexual (with `-9` being strictly heterosexual) and positive numbers are increasingly homosexual (with `+9` being strictly homosexual)

A mapping of key values follows, where "KS" means "Kinsey scale". The value on the left is for the Geek Code; the value on the right is for the equivalent in the Kinsey Scale.

```
-9 KS 0
-6 KS 1
-3 KS 2
+0 KS 3
+1 KS 4
+6 KS 5
+9 KS 6

! My sexual orientation is none of your business!
? My orientation doesn't fit properly on a Kinsey Scale
```

### p – politics

The last few years has seen the rise of the political geek. This phenomena is little understood, but some theorize that it has come about because of the popular media’s attempts to demonize the Internet and computer use in general, and the government’s willingness to go along with it. Others propose that the aging geek population has simply started taking an interest in the world around them. Some support the “Sun Spot” theory.

Politics, here, are divided in two ways, which summarize two popular political tests.

The first test summarizes the political compass. This test is available here:
https://www.politicalcompass.org/

[TODO: blurb, explanation]

The second test summarizes [what?]:
https://8values.github.io/

[TODO: blurb, explanation]


### r - relationships

[TODO: Update]

While many geeks are highly successful at having relationships, a good many more are not. Give us the gritty details.

```
r+++ Found someone, dated, and am now married.
r++ I’ve dated my current S.O. for a long time.
r+ I date frequently, bouncing from one relationship to another.
r I date periodically.
r- I have difficulty maintaining a relationship.
r– People just aren’t interested in dating me.
r— I’m beginning to think that I’m a leper or something, the way people avoid me like the plague.
!r I’ve never had a relationship, OR not for public consumption
r* signifying membership in the SBCA (Sour Bachelor(ette)’s Club of America). The motto is ‘Bitter, but not Desperate’. First founded at Caltech.
r% I was going out with someone, but the asshole dumped me.
```

```
### s - sex

[TODO: Update]

Geeks have traditionally had problems with sex (ie, they never have any). Because geeks are so wrapped up in their sexuality (or lack of sexuality for that matter), it is important that the geek be willing to quantify their sexual experiences.

This code also is used to denote the gender of the geek. Females use ‘x’ in this category, while males use ‘y’. Those that do not wish to disclose their gender can use ‘z’. For example:
```
x+ — A female who has had sex
y+ — A male who has had sex.
z+ — A person (gender undisclosed) who has had sex.
!z neither my sex nor my sex life are any of your beeswax
```

### t – TV shows/series/movies

[TODO: Update]

List what you think of a given series

```
TD – doctorwho
TR&M – rick&MORTY
TF – firefly
TS – stargate
TTBB – the big bang
TB – Babylon5
TI – ‘In search of…’ with Leonard Nimoy
TM – monty python (series/films)
TMM – mad max
TSW – star wars franchise
TG – game of thrones
TLOTR – lord of the rings
TL – lost
Tt – star trek
````

### v - Video Games

[TODO: Create Section, restore Doom]


==============================================================

### C- COMPUTERS

There is a record of geeks that don’t use computers. Unfortunately, they are all dead, having lived in an era of no computers. All modern geeks have some exposure to computers. If you don’t know what a computer is, you need to go back into your shell.

Computers
Most geeks identify themselves by their use of computers and computer networks. In order to quantify your geekiness level on computers, consult the following (consider the term ‘computers’ synonymous with ‘computer network’). This category represents “general” computer aptitude. Categories below will get into specifics.

```
C+4 I’ll be first in line to get the new cybernetic interface installed into my skull.
C+3 You mean there is life outside of Internet? You’re shittin’ me! I haven’t dragged myself to class in weeks.
C+2 Computers are a large part of my existence. I code in at least one language
C+ Computers are fun and I enjoy using them. 
C Computers are a tool, nothing more. I use it when it serves my purpose.
C- Anything more complicated than my calculator and I’m screwed.
C-2 Where’s the on switch?
C-3 If you even mention computers, I will rip your head off!
```
#### U – UNIX
It seems that a Unix-based operating system is the OS of choice among most geeks. In addition to telling us about your Unix abilities, you can also show which specific Unix OS you are using. To accomplish this, you include a letter showing the brand with your rating. For example: UL++++ would indicate a sysadmin running Linux.

```
    U – Unix
        UL – Linux
            ULR – RPM
                ULRC – cwntos
                ULRF – fedora
                ULRO – opensuse
                ULRU – urpmi
                ULRA – apt-rpm
            ULD – Debian
                ULDU – ubuntu
                ULDUX 3rd party/discontinued ubuntu
                ULDM – Mepis
                ULDK – Knoppix
            ULP – Pacman
            ULG – Gentoo
            ULS – slackware
            UL* – other
        US – Sun OS/Solaris
        UA – AIX
        UH – HPUX
        UI – IRIX
        UC – SCO Unix
        U* – Some other one not listed
some examples
```
U++++ I am the sysadmin. If you try and crack my machine don’t be surprised if the municipal works department gets an “accidental” computer-generated order to put start a new landfill on your front lawn or your quota is reduced to 4K.
U+++ I don’t need to crack /etc/passwd because I just modified su so that it doesn’t prompt me. The admin staff doesn’t know I’m here.
U++ I’ve get the entire admin ticked off at me because I am always using all of the CPU time and trying to run programs that I don’t have access to.
U+ I enjoy shell scripting and understand the fundamental importance of the difference between ‘ and `
U I have a Unix account to do my stuff in
U- I have a VMS account.
U– I’ve seen Unix and didn’t like it. DEC rules!
U— Unix geeks are actually nerds in disguise.
```



#### FE – Frontend
```
FE++
I am a java bean
FE--
I couldnt care less about the 'user experience'; users can be approximated using Bayesian techniques
```
#### BE – Backend
```
BE+++ I wrote my own database system as current performance limitations were irking me
BE--- Keep the dirty stuff under the hood, building a cool GUI is where its at
```

#### M – Macintosh
Many geeks have abandoned the character-based computer altogether and moved over to the Macintosh. It in important to give notification of your Mac rating.
```
M++  I am a Mac guru. Anything those DOS putzes and Unix nerds can do, I can do better, and if not, I’ll write the damn software to do it.
M+  A Mac has it’s uses and I use it quite often.
M  I use a Mac, but I’m pretty indifferent about it.
M- Macs suck. All real geeks have a character prompt.
M– Macs do more than suck. They make a user stupid by allowing them to use the system without knowing what they are doing. Mac weenies have lower IQs than the fuzz in my navel.
```

### E – Electronics
```
E+++  I am lady ada
E++  I have fixed broken toasters without removing the plug, such is my skill and need for speed.  
E+   I know CMOS from BJT and why a comparator is not quite equivalent to an op amp
E-- Electrons are interesting as theoretical constructs
```

#### H – Hardware
```
H+++   I smithed my own chainmail from iron I smelted with ore mined by means of steam-powered equipment I created from old car parts.
H—   I have used hammers  metaphorically far more often than literally
H--  I prefer to take my laptop to the shop when the hardware acts up 
```

### ENTERTAINMENT

Geeks love to play. No matter their age, all geeks enjoy playing. Of course, the object of this entertainment takes a myriad of different forms. What is it that pushes a geek to play? Is it simply a desire to relive their childhood? Or perhaps there is a piece of geeky genetic code that requires intellectual stimulation. Who knows, maybe it’s a Freudian thing…

In v4, tv/series are given its own category other than star trek which remains for backwards compatibility.



#### R – Role Playing
Role-playing games such as Dungeons & Dragons have long been a part of the traditional geek life. Because geeks often become so involved in their role-playing that they lose touch with reality, include one of the following role-playing codes.
```
R+++ I’ve written and published my own gaming materials.
R++ There is no life outside the role of the die. I know all of piddly rules of (chosen game). _MY_ own warped rules scare the rest of the players.
R+ I’ve got my weekly sessions set up and a character that I know better than I know myself.
R Role-Playing? That’s just something to do to kill a Saturday afternoon
R- Gosh, what an utter waste of time!
R– Role-Players are instruments of pure evil.
R— I work for T$R.
R* I thought life WAS role-playing?
```