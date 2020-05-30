# RU-PopularMusic-Corpus
В этот репозиторий я складываю свои попытки собрать Диахронический корпус русскоязычной популярной музыки (1990-2019) и что-то понять о том, что происходило в этих текстах: что казалось авторам актуальным, какие бытовые детали они описывали. В общем, про что пели в эти 30 лет. <br>
Научный руководитель: <a href='https://github.com/danilsko'>DanilSko</a><br><br>
Весь код находится в трех тетрадях: <br>
<ol>
<li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/1.%20Scraping%20from%20genius.ipynb'>Scraping from genius.ipynb</a> - код для того, чтобы через библиотеку <a href='https://github.com/johnwmillr/LyricsGenius'> lyricsgenius </a> скачать файлы с genius.com, которые пойдут для построения корпуса.</li>
<li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/2.%20Mystem%20%2B%20Writing%20to%20base.ipynb'>Mystem + Writing to base.ipynb</a> - код, который создает корпус (реляционную базу данных), и разбирает тексты при помощи морфологического анализатора <a href='https://yandex.ru/dev/mystem/'> mystem</a>.</li>
<li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/3.%20An%20example%20research.ipynb<a>An example research.ipynb</a> - пример исследования, которое можно провести при помощи корпуса. В исследовании используется <a href='http://ucrel.lancs.ac.uk/usas/'>система семантического анализа UCREL (USAS)</a>. В работе использована версия 2006 года. Оказалось, что систему усовершенствовали, поэтому лучше использовать <a href='https://github.com/UCREL/Multilingual-USAS/tree/master/Russian'>обновленные</a> данные из репозитория UCREL. Способ остается тем же.</li>
</ol>
Другие файлы, которые находятся в репозитории:
<ol>
  <li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/ALLP.db'>ALLP.db - сам корпус. 1129 песен от 60 исполнителей, 169257 токенов.</a></li>
  <li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/altcorp.db'>altcorp.db - корпус исполнителей в жанре рок, хип-хоп, электроника. 37 исполнителей, 1454 песни, 253861 токен.</a></li>
  <li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/freqrnc2011.csv'>freqrnc2011.csv</a> - список частотностей слов из <a href='http://dict.ruslang.ru/freq.php'>Нового частотного словаря Национального корпуса русского языка</a> (2011).</li>
  <li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/frequency.tsv'>frequency.tsv</a> - список частотностей слов из песенного корпуса (ALLP.db)</li>
  <li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/keywords.txt'>keywords.txt</a> - ключевые слова для каждого из исполнителей корпуса, получены при помощи TfidfVectorizer из sklearn</li>
  <li><a href='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/noun.tsv'>noun.tsv</a> - список существительных с самой высокой частотностью в корпусе</li>
  <li><a href ='https://github.com/mjolnika/RU-PopCultural-Corpus/blob/master/semantic_lexicon_rus.usas'>semantic_lexicon_rus.usas - <a href='http://ucrel.lancs.ac.uk/projects/assist/RSTDecember2006.zip'>лексикон</a> отсюда (острожно! ссылка на zip-arcive)</li>
  </ol>
  *<br>
  <a href = 't.me/rupopcorpus'>тг-канал</a> про то, как все было сложно
    
