# Keyboard layouts

## Letter frequency

English, from [wikipedia](https://en.wikipedia.org/wiki/Letter_frequency).

```
a 8.167%
b 1.492%
c 2.202%
d 4.253%
e 12.702%
f 2.228%
g 2.015%
h 6.094%
i 6.966%
j 0.153%
k 1.292%
l 4.025%
m 2.406%
n 6.749%
o 7.507%
p 1.929%
q 0.095%
r 5.987%
s 6.327%
t 9.356%
u 2.758%
v 0.978%
w 2.560%
x 0.150%
y 1.994%
z 0.077%
```

`TODO: markdown extension/preprocessing to render keyboard diagrams`
Для этого можно использовать http://www.keyboard-layout-editor.com/ и внутреннее представление раскладок в нем. У него открытые исходники.

### Links

* [LetterFrequency.org](http://letterfrequency.org/) дает информацию по частотности для разных корпусов текста английского и разных языков. Нет процентного соотношения. Список наиболее частых слов в английском.
* [Статья на википедии](https://en.wikipedia.org/wiki/Letter_frequency) с процентами по английскому и некоторым другим языкам, основанным на латинице
* [Частотность в английскомы для криптографии](http://pi.math.cornell.edu/~mec/2003-2004/cryptography/subs/frequencies.html) на 40000 слов с процентами
* [Частотность символов в целом, не только букв, а также ди-три-графов и слов](https://mdickens.me/typing/letter_frequency.html) в английском с примешиванием исходников программ.

## Layout design principles

* rolling fingers inwards/outwards
* same hand sequences or alternating?

## Layouts

* Colemak
  * [Colemak Mod-DH](https://colemakmods.github.io/mod-dh/)
* [Norman](https://normanlayout.info/)
* [RSTHD](https://xsznix.wordpress.com/2016/05/16/introducing-the-rsthd-layout/), designed for ergodox

## Quotes from internet about keyboard layout design

> Some things to note:
> 1) E and T just have to be under the middle fingers on the home row in any comfortable layout.
> 2) T and H need to be adjacent.
> 3) Vowels on one side, consonants on the other side of the home row. Keep the home row's Scrabble score to a minimum.

[pklausler at hn](https://news.ycombinator.com/item?id=11883938)

> Just as you did, I came to some specific conclusions about comfortable layout:
> * E & T must be under the middle fingers on the home row.
> * T & H need to be adjacent.
> * Vowels on one side, most important consonants on the other.

[jboy at hn](https://news.ycombinator.com/item?id=11884365)

> Some notes based on my own experience:
> * If you can touch type very well in Qwerty already, you may have a much easier time picking up a layout than the average typist. And you may have an easier time retaining more than one layout.
> * What you're typing (context) is important with regards to adjusting to a layout. For example, if you learn Colemak and decide to try using the Terminal some time after you've become proficient, you might find it awkward - at first. I personally haven't found the type of physical keyboard you use to matter much with regards to this..
> * When I was at the state where I could type in both layouts very poorly (due to muscle memory being confused), I realized I took many things for granted that eliminate needing to type quickly altogether like auto-suggestion/completion - and a lot about software development is about automating tasks.
> * When I started to become proficient at Colemak and started to lose my proficiency at Qwerty, I developed a justification and bias that Colemak is way more comfortable for my daily usage.
> * The most effort I ever put into typing was ironically typing tests, not programming =P. And those can be really tiring if you do them frequently regardless of layout.
> 
> Maybe I find these days that colemak is marginally more comfortable. Maybe I just don't type that much though, although I use the computer a lot. Software developers certainly don't type nearly as much as a "typist job" (if those still exist) in any case. If I lose my ability to type in Colemak, I don't think it will effect me that much. All in all, I can't say my transition was worth my time. 

[zZorgz at hn](https://news.ycombinator.com/item?id=11884228)

> I'm proficient in Qwerty, Dvorak, and RSTHD [1]. I also learned Colemak at one point and was proficient at it, but learning RSTHD replaced my Colemak muscle memory (which in itself is odd and interesting). Right now I use RSTHD when I have my ErgoDox, Dvorak on a standard keyboard, and Qwerty on mobile. Some additional things I've found:
> * It's possible to be proficient in multiple layouts at a time as long as you use all of them on a regular basis.
> * Furthermore, it's possible to separate your muscle memory for a layout from your muscle memory for the physical keyboard enough to be able to switch between keyboard layouts basically at will.
> * Getting used to moving around punctuation is much harder than getting used to moving around normal letters for some reason.
> * If you use different keyboard form factors (for me, ErgoDox vs. standard keyboard), your muscle memory for the layout is tied to your muscle memory of the physical keyboard itself. I can't type Qwerty on an ErgoDox but I can just fine on a standard keyboard.
> 
> [1] https://xsznix.wordpress.com/2016/05/16/introducing-the-rsthd-layout/

[xsznix at hn](https://news.ycombinator.com/item?id=11886928)

> I too found Colemak lacking. IMO it's because the most relevant keyboard layout metrics are
> 1) how well words break down into same hand "finger rolls", which help typing accuracy and to lesser extend speed
> 2) how often the same finger has to type multiple characters in succession
> 3) how often the same hand has to reach for the more awkward middle keys (y and b in qwerty) while also doing something with the middle finger
>
> Finger travel distance is irrelevant. Common characters ought to be on the home row because your fingers can't roll across the top and bottom row.
>
> Dvorak optimizes these very well. Workman seems to split bigrams across two hands, which prevents rolls. I would also recommend binding alt-gr to control in addition to making caps lock backspace. 

[htns at hn](https://news.ycombinator.com/item?id=11883673)

## Links

* [carpalx](http://mkweb.bcgsc.ca/carpalx/)
* [white keyboard layout](https://github.com/mw8/white_keyboard_layout) - An optimized personal keyboard layout and the tools to create your own
* [keyboard layout analyzer](http://patorjk.com/keyboard-layout-analyzer/) - See which layout is best for your input text
* [ErgonomicNotes](https://github.com/melling/ErgonomicNotes/) from some github user with load of links
