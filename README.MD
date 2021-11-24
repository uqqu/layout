# qPhyx letter layout
## ↓ English part

> If you are able to read Russian, you should look at the [appropriate section](#-russian-part)

> This layout-part has been divided from the main project. Symbol and language layers represent a separate part, located in the [own repository](https://github.com/uqqu/qPhyx)

**qPhyx letter layout** is a phonetic biscripted keyboard layout with one of the best possible scores of typing convenience, based on the current convenience calculation (this aspect will be improved in the future).

To create an objectively comfortable layout, monogram and bigram frequency analyses were collected (and performed [own](https://github.com/uqqu/frequency_analysis)); the alphabetic part of the keyboard was divided into convenience groups; convenience typing criteria were defined.

Based on the above, the parallel positioning of the English and Russian alphabetic characters was performed.

After that, a comparison with existing standard and alternative keyboard layouts were made, based on the same input data.

All analyses, calculations, comparisons, and results are in [calculation.xlsx](https://github.com/uqqu/layout/blob/master/calculation.xlsx).


### Frequency analyses

First, various frequency analyses were found and stored with their average value *(so this is a meta-analysis?)*. A total of more than 30 analyses were selected based on different samples. All valid analyses found were taken into account.

For English, the following analyses were included in the final view for the base letter frequency:

  * [norvig.com](http://norvig.com/mayzner.html)
  * [core.ac.uk](https://core.ac.uk/download/pdf/231084615.pdf)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/english-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/en/multiUN)
  * [macfreek.nl](http://www.macfreek.nl/memory/Letter_Distribution)
  * [viviancook.uk](http://www.viviancook.uk/SpellStats/SingleLetterFrequencies.htm)
  * [fitaly.com](http://www.fitaly.com/board/domper3/posts/136.html)
  * [sttmedia.com](https://www.sttmedia.com/characterfrequency-english)
  * [mathstats.uncg.edu](https://mathstats.uncg.edu/sites/pauli/112/HTML/secfrequency.html)
  * [pi.math.cornell.edu](http://pi.math.cornell.edu/~mec/2003-2004/cryptography/subs/frequencies.html)
  * [math.ucsd.edu](http://www.math.ucsd.edu/~crypto/Projects/MarshaMoreno/TimeComparisonFrequency.pdf)
  * [cs.wellesley.edu](http://cs.wellesley.edu/~fturbak/codman/letterfreq.html)
  * [en.algoritmy.net](http://en.algoritmy.net/article/40379/Letter-frequency-English)

For Russian, the following analyses were included for the base letter frequency:

  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/multiUN)
  * [dict.ruslang.ru](http://dict.ruslang.ru/freq.php?act=show&dic=freq_letters)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/russian-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/annot_opcorpora)
  * [lg--web.chat.ru](http://lg--web.chat.ru/texts.html)
  * [sttmedia.com](https://www.sttmedia.com/characterfrequency-russian)
  * [dpva.ru](https://dpva.ru/Guide/GuideUnitsAlphabets/Alphabets/FrequencyRuLetters/)
  * [simia.net](http://simia.net/letters/index.html)
  * Яглом А.М., Яглом И.М., Вероятность и информация, М.: Наука, 1973 / с.238

For English, the following bigram analyses were selected for paired letter frequency:

  * [gist.github.com/lydell](https://gist.github.com/lydell/c439049abac2c9226e53)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/english-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/en/multiUN)
  * [link.springer.com](https://link.springer.com/content/pdf/10.3758/BF03201360.pdf)
  * [homepages.math.uic.edu](http://homepages.math.uic.edu/~leon/mcs425-s08/handouts/char_freq2.pdf)
  * [joyofdata.de](https://www.joyofdata.de/blog/frequency-of-character-combinations/)

For Russian, the following bigram analyses were selected for paired letter frequency:

  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/multiUN)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/russian-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/annot_opcorpora)
  * [joyofdata.de](https://www.joyofdata.de/blog/frequency-of-character-combinations/)
  * [statistica.ru](http://statistica.ru/local-portals/data-mining/analiz-tekstov/)

### Selection of convenience criteria

To objectively evaluate the ease of use of the layout, it is necessary to allocate the appropriate criteria. They are:
  * hand alteration (the probability that both hands will be used to type any random pair of letters)
  * minimum chance to double sequentially usage of the same finger (bearing in mind base key repeating)
  * even hand and finger load
  * maximum usage on the most convenience groups

For the latter criteria letter-part of default non-ergonomic keyboard were divided into 6 groups by convenience:

Despite the fact that such a division itself is somewhat subjective, the allocation of the first group does not cause any questions – these are home finger positions, where you do not need to make any movements, only pressing. In future scores, the focus of this criterion will be on the first group, as the most objective.


### Layout creation

Past points have been systematized and automated in [.xlsx](https://github.com/uqqu/layout/blob/master/calculation.xlsx) to further create the layout.
> You can also try to change the current layout or create your own in this file. All scores change dynamically, depending on the current view.

Many variations have been tried for both languages. Some were extremely successful, and are still on the sheet <code>[en/ru] archive</code>. However, the final form of layouts must skillfully balance between all criteria. And also, in view of the original purpose of the phonetic layout, it is necessary to take into account the phonetic dependence of the layouts of the two languages. After much ordeal, such a double layout became the following parts:

![En layout](https://github.com/uqqu/layout/blob/master/readme_images/en_letters.png "Letter layout")
![Ru layout](https://github.com/uqqu/layout/blob/master/readme_images/ru_letters.png "Letter layout")

The name of the layout was composed, with a slight stylization, by the first characters of the upper row – «qPhyx».

### Result numbers

I'll list it all:
  * hand alteration – 70.58% (en) and 71.26% (ru)
  * chance to double sequentially usage of the same finger – 2.55% and 4.48%
  * hand load – 48.36/51.64% and 52.30/47.70%
  * "home" group usage – 64.95% and 58.60%
<br><sub>and also a nice look and mnemonic rows</sub>

### Existing alternative layouts


<details>
  <summary>qwerty (en)</summary>
  <ul>
    <li>hand alteration – 52.60%</li>
    <li>chance to double sequentially usage of the same finger – 7.08%</li>
    <li>hand load – 58.69/41.31%</li>
    <li>"home" group usage – 25.70%</li>
  </ul>
</details>
<details>
  <summary>workman (en)</summary>
  <ul>
    <li>hand alteration – 55.96%</li>
    <li>chance to double sequentially usage of the same finger – 2.91%</li>
    <li>hand load – 51.49/48.51%</li>
    <li>"home" group usage – 63.71%</li>
  </ul>
</details>
<details>
  <summary>colemak (en)</summary>
  <ul>
    <li>hand alteration – 58.64%</li>
    <li>chance to double sequentially usage of the same finger – 1.26%</li>
    <li>hand load – 48.38/51.62%</li>
    <li>"home" group usage – 64.95%</li>
  </ul>
</details>
<details>
  <summary>dvorak (en)</summary>
  <ul>
    <li>hand alteration – 70.67%</li>
    <li>chance to double sequentially usage of the same finger – 2.61%</li>
    <li>hand load – 43.30/56.70%</li>
    <li>"home" group usage – 58.92%</li>
  </ul>
</details>
<details>
  <summary>qwpr (en)</summary>
  <ul>
    <li>hand alteration – 58.64%</li>
    <li>chance to double sequentially usage of the same finger – 4.04%</li>
    <li>hand load – 48.38/51.62%</li>
    <li>"home" group usage – 62.53%</li>
  </ul>
</details>
<details>
  <summary>йцукен (ru)</summary>
  <ul>
    <li>hand alteration – 54.78%</li>
    <li>chance to double sequentially usage of the same finger – 18.17%</li>
    <li>hand load – 53.50/46.37% (without "ё")</li>
    <li>"home" group usage – 33.40%</li>
  </ul>
  <sub>An interesting fact: two-thirds of all presses in the йцукен are on the index fingers. And such a grouping of the most popular characters as a result leads to the fact that and every fifth press will be performed by the same finger. What kind of "ten-finger typing" can we talk about in this situation?</sub>
</details>
<details>
  <summary>яверты (ru)</summary>
  (** only the letters of the main letter block were taken into account)
  <ul>
    <li>hand alteration – 48.36%</li>
    <li>chance to double sequentially usage of the same finger – 8.85%</li>
    <li>hand load – 50.69/46.63%</li>
    <li>"home" group usage – 25.41%</li>
  </ul>
</details>
<details>
  <summary>диктор (ru)</summary>
  <ul>
    <li>hand alteration – 73.63%</li>
    <li>chance to double sequentially usage of the same finger – 3.01%</li>
    <li>hand load – 45.71/54.11%</li>
    <li>"home" group usage – 53.21%</li>
  </ul>
</details>
<details>
  <summary>раскладка Зубачёва (ru)</summary>
  <ul>
    <li>hand alteration – 75.02%</li>
    <li>chance to double sequentially usage of the same finger – 2.25%</li>
    <li>hand load – 46.40/53.47%</li>
    <li>"home" group usage – 48.99%</li>
  </ul>
</details>


#### Result
As you can see, <code>qwerty</code> and <code>йцукен</code> are frankly bad, to put it mildly. Any existing alternative layout (including the ones not listed) is much better. If you look at the opposite result, <code>dvorak</code> and <code>раскладка Зубачёва</code>, according to the main points, take the lead in their languages.
I will not fully compare <code>dvorak</code>/<code>раскладка Зубачёва</code> and <code>qPhyx</code>, because this comparison is not correct. However even for a general idea you can note that on the whole the numbers of the topic-starter if not better, then at least at the level of the leaders.


### Hanging questions

* reducing the load on the little fingers
* reviewing the importance of certain criteria
* design of criteria "accordness" (typing several keys with a single consecutive motion of the fingers of one hand */how do account for it?/*)
* summarizing all the criteria into a single final score


---


## ↓ Russian part

> Эта раскладка была отделена от основного проекта. Символьные и языковые слои теперь являются самостоятельной частью и расположены в [собственном репозитории](https://github.com/uqqu/qPhyx)

**Клавиатурная раскладка qPhyx** – фонетическая двускриптовая клавиатурная раскладка с одними из лучших возможных показателей удобства печати, на основе текущих расчётов удобства (будут пересмотрены и улучшены в будущем).

Для создания объективно удобной раскладки были собраны (и проведены [собственные](https://github.com/uqqu/frequency_analysis)) анализы базовой и биграммной частотностей; буквенная часть клавиатуры была разделена на группы удобства; были выделены критерии удобства набора.

На основе вышеперечисленного было выполнено параллельное позиционирование буквенных символов на английской и русской раскладках.

После были проведены сравнения с существующими стандартными и альтернативными клавиатурными раскладками, основываясь на одних входных данных.

Все анализы, расчёты, сравнения и результаты находятся в [calculation.xlsx](https://github.com/uqqu/layout/blob/master/calculation.xlsx).


### Анализы частотности

Первым делом были отобраны различные анализы частотностей букв для интересующих языков, из которых были выведены средние значения *(получается, метаанализ)*. Всего было отобрано более 30 анализов, основанных на разных выборках. Учитывались все достоверные найденные анализы.

Для английского языка для базовой буквенной частотности в финальный вид были включены следующие анализы:

  * [norvig.com](http://norvig.com/mayzner.html)
  * [core.ac.uk](https://core.ac.uk/download/pdf/231084615.pdf)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/english-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/en/multiUN)
  * [macfreek.nl](http://www.macfreek.nl/memory/Letter_Distribution)
  * [viviancook.uk](http://www.viviancook.uk/SpellStats/SingleLetterFrequencies.htm)
  * [fitaly.com](http://www.fitaly.com/board/domper3/posts/136.html)
  * [sttmedia.com](https://www.sttmedia.com/characterfrequency-english)
  * [mathstats.uncg.edu](https://mathstats.uncg.edu/sites/pauli/112/HTML/secfrequency.html)
  * [pi.math.cornell.edu](http://pi.math.cornell.edu/~mec/2003-2004/cryptography/subs/frequencies.html)
  * [math.ucsd.edu](http://www.math.ucsd.edu/~crypto/Projects/MarshaMoreno/TimeComparisonFrequency.pdf)
  * [cs.wellesley.edu](http://cs.wellesley.edu/~fturbak/codman/letterfreq.html)
  * [en.algoritmy.net](http://en.algoritmy.net/article/40379/Letter-frequency-English)

Для русского языка для базовой буквенной частотности были включены следующие анализы:

  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/multiUN)
  * [dict.ruslang.ru](http://dict.ruslang.ru/freq.php?act=show&dic=freq_letters)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/russian-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/annot_opcorpora)
  * [lg--web.chat.ru](http://lg--web.chat.ru/texts.html)
  * [sttmedia.com](https://www.sttmedia.com/characterfrequency-russian)
  * [dpva.ru](https://dpva.ru/Guide/GuideUnitsAlphabets/Alphabets/FrequencyRuLetters/)
  * [simia.net](http://simia.net/letters/index.html)
  * Яглом А.М., Яглом И.М., Вероятность и информация, М.: Наука, 1973 / с.238

Для английского языка для парной буквенной частотности были отобраны следующие биграммные анализы:

  * [gist.github.com/lydell](https://gist.github.com/lydell/c439049abac2c9226e53)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/english-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/en/multiUN)
  * [link.springer.com](https://link.springer.com/content/pdf/10.3758/BF03201360.pdf)
  * [homepages.math.uic.edu](http://homepages.math.uic.edu/~leon/mcs425-s08/handouts/char_freq2.pdf)
  * [joyofdata.de](https://www.joyofdata.de/blog/frequency-of-character-combinations/)

Для русского языка для парной буквенной частотности были отобраны следующие биграммные анализы:

  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/multiUN)
  * [practicalcryptography.com](http://practicalcryptography.com/cryptanalysis/letter-frequencies-various-languages/russian-letter-frequencies/)
  * [github.com/uqqu](https://github.com/uqqu/frequency_analysis/tree/master/examples/ru/annot_opcorpora)
  * [joyofdata.de](https://www.joyofdata.de/blog/frequency-of-character-combinations/)
  * [statistica.ru](http://statistica.ru/local-portals/data-mining/analiz-tekstov/)

### Отбор критериев удобства

Для объективной оценки удобства использования раскладки необходимо выделить соответствующие критерии. Ими стали:
  * чередование рук (вероятность, с которой для набора любой случайной пары букв будут задействованы обе руки)
  * минимизация вероятности использования одного пальца на два набора подряд (с учётом базовой вероятности повтора одной буквы)
  * равномерная нагрузка рук
  * максимальное использование наиболее удобных групп

Для последнего критерия буквенная часть стандартной не эргономичной клавиатуры была разделена на 6(7) групп по удобству.

Несмотря на то, что само подобное разделение является несколько субъективным, выделение первой группы не вызывает никаких вопросов – это домашние позиции пальцев, где вам не нужно совершать никаких движений, только нажатие. В будущей оценке основное внимание на этот критерий будет обращено именно на первую группу, как на самую объективную.


### Создание раскладки

Прошлые пункты были систематизированы и автоматизированы в [.xlsx](https://github.com/uqqu/layout/blob/master/calculation.xlsx), для дальнейшего создания раскладки.
> Вы также можете попробовать изменить текущую раскладку или создать свою в данном файле. Все оценки изменяются динамически, в зависимости от текущего вида.

Было опробовано множество вариантов для обоих языков. Некоторые оказались крайне удачными, и до сих пор хранятся на листе <code>[en/ru] archive</code>. Однако финальный вид раскладок должен умело балансировать между всеми критериями. А также ввиду изначальной цели создания фонетической раскладки, необходимо учитывать фонетическую зависимость раскладок двух языков. Спустя многие мытарства такой двойной раскладкой стали следующие части:

![Ru layout](https://github.com/uqqu/layout/blob/master/readme_images/ru_letters.png "Letter layout")
![En layout](https://github.com/uqqu/layout/blob/master/readme_images/en_letters.png "Letter layout")

Название раскладки составилось, с небольшой стилизацией, по первым символам верхнего ряда – «qPhyx».

### Так что же, Веничка, что же всё-таки с цифрами? Нам страшно интересно...

Да ведь я понимаю, что интересно. Сейчас, сейчас перечислю:
  * чередование рук – 70.58% (en) и 71.26% (ru)
  * вероятность "чистого" повторного нажатия одним пальцем – 2.55% и 4.48%
  * равномерность нагрузки рук – 48.36/51.64% и 52.30/47.70%
  * использование "домашней" группы – 64.95% и 58.60%
<br><sub>а ещё приятный внешний вид и мнемонические ряды</sub>

### Так-так-так, – говорите вы, – а альтернативные раскладки? Ведь всё уже придумано до тебя


<details>
  <summary>qwerty (en)</summary>
  <ul>
    <li>чередование рук – 52.60%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 7.08%</li>
    <li>равномерность нагрузки рук – 58.69/41.31%</li>
    <li>использование "домашней" группы – 25.70%</li>
  </ul>
</details>
<details>
  <summary>workman (en)</summary>
  <ul>
    <li>чередование рук – 55.96%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 2.91%</li>
    <li>равномерность нагрузки рук – 51.49/48.51%</li>
    <li>использование "домашней" группы – 63.71%</li>
  </ul>
</details>
<details>
  <summary>colemak (en)</summary>
  <ul>
    <li>чередование рук – 58.64%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 1.26%</li>
    <li>равномерность нагрузки рук – 48.38/51.62%</li>
    <li>использование "домашней" группы – 64.95%</li>
  </ul>
</details>
<details>
  <summary>dvorak (en)</summary>
  <ul>
    <li>чередование рук – 70.67%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 2.61%</li>
    <li>равномерность нагрузки рук – 43.30/56.70%</li>
    <li>использование "домашней" группы – 58.92%</li>
  </ul>
</details>
<details>
  <summary>qwpr (en)</summary>
  <ul>
    <li>чередование рук – 58.64%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 4.04%</li>
    <li>равномерность нагрузки рук – 48.38/51.62%</li>
    <li>использование "домашней" группы – 62.53%</li>
  </ul>
</details>
<details>
  <summary>йцукен (ru)</summary>
  <ul>
    <li>чередование рук – 54.78%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 18.17%</li>
    <li>равномерность нагрузки рук – 53.50/46.37% (без "ё")</li>
    <li>использование "домашней" группы – 33.40%</li>
  </ul>
  <sub>Интересный факт: две трети всех нажатий в йцукен приходятся на указательные пальцы. А подобная сгруппированность популярнейших символов в результате приводит к тому, что и каждое пятое нажатие будет выполняться одним и тем же пальцем. О каком "десятипальцевом наборе" в такой ситуации может идти речь?</sub>
</details>
<details>
  <summary>яверты (ru)</summary>
  (** учитывались только буквы основного буквенного блока)
  <ul>
    <li>чередование рук – 48.36%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 8.85%</li>
    <li>равномерность нагрузки рук – 50.69/46.63%</li>
    <li>использование "домашней" группы – 25.41%</li>
  </ul>
</details>
<details>
  <summary>диктор (ru)</summary>
  <ul>
    <li>чередование рук – 73.63%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 3.01%</li>
    <li>равномерность нагрузки рук – 45.71/54.11%</li>
    <li>использование "домашней" группы – 53.21%</li>
  </ul>
</details>
<details>
  <summary>раскладка Зубачёва (ru)</summary>
  <ul>
    <li>чередование рук – 75.02%</li>
    <li>вероятность "чистого" повторного нажатия одним пальцем – 2.25%</li>
    <li>равномерность нагрузки рук – 46.40/53.47%</li>
    <li>использование "домашней" группы – 48.99%</li>
  </ul>
</details>


#### Результат
Как видно, <code>qwerty</code> и <code>йцукен</code> откровенно плохи, если не сказать грубее. Любые существующие альтернативные раскладки (в том числе из не перечисленных) в разы и разы лучше. Если смотреть на обратный результат, то <code>dvorak</code> и <code>раскладка Зубачёва</code>, забирают первенство в своих языках.
Полноценно сравнивать <code>dvorak</code>/<code>раскладку Зубачёва</code> и <code>qPhyx</code> я не стану, так как это сравнение не совсем корректно. Но даже для общего представления вы можете отметить, что в целом цифры топик-стартера если уж не лучше, то как минимум на уровне лидеров.


### Подвешенные вопросы

* снижение нагрузки на мизинцы
* пересмотр важности отдельных критериев
* оформление критерия "аккордности" (набор нескольких клавиш единым последовательным движением пальцев одной руки */как это учитывать?/*)
* обобщение всех критериев в единую результирующую оценку
