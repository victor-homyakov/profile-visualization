##### вступление

Задача вступительной части презентации – познакомить слушателей с темой доклада, заинтересовать их,
показать важность темы и установить контакт с аудиторией.

- почему именно я рассказываю именно об этой теме и какой у меня опыт в данной области
    профессионально занимаюсь анализом и улучшением производительности страницы поиска в Яндексе
    (добавить картинку/видео загрузки серпа или видео сравнения загрузки Яндекс vs Google)
    (график сравнения скорости загрузки Yandex vs Google)
    (график сравнения скорости загрузки с прошлогодней для иллюстрации прогресса?)

- почему аудитории важно послушать мой доклад
    анализировать числа - тяжело и медленно,
    анализировать изображение - быстрое распознавание тренда и "особых мест"
    пример - https://stat.yandex-team.ru/-/CBR1ARVpgA
    таблица чисел против графика

- какую пользу получит слушатель от моего выступления
    узнает про удобные способы и инструменты анализа,
    станет чаще профилировать и ускорять свой код

##### React на вкладке Performance

надо скриншот

https://yandex.ru/search/?text=%D0%B3%D0%B8%D1%84%D0%BA%D0%B8%20%D1%81%D0%B0%D0%BB%D1%8E%D1%82%D1%8B%20%D1%84%D0%B5%D0%B9%D0%B5%D1%80%D0%B2%D0%B5%D1%80%D0%BA%D0%B8&noredirect=1&lr=213

Development-сборка React 

react-dom/cjs/react-dom.development.js

https://github.com/facebook/react/blob/4a635785f5cc40bde901ada6090904fdc8cc120d/packages/react-reconciler/src/ReactDebugFiberPerf.js#L80-L101

https://reactjs.org/docs/optimizing-performance.html#profiling-components-with-the-chrome-performance-tab

User Timing API
https://developer.mozilla.org/en-US/docs/Web/API/User_Timing_API

##### Свои таймлайны на вкладке Performance

- console.time(label), console.timeEnd(label)
- console.timeStamp(label)

performance.mark(markName);
performance.measure(label, markName);
// Clear marks immediately to avoid growing buffer.
performance.clearMarks(markName);
performance.clearMeasures(label);

https://developer.mozilla.org/en-US/docs/Web/API/User_Timing_API

##### вкладка profiler (deprecated для html, OK для node)

много текста и чисел - неинтересно (надо скриншот)

JS flame chart - уже лучше (надо скриншот)

console.profile(), console.profileEnd() — для JavaScript Profiler

экспорт нескольких профайлов + merge + импорт + визуализация (надо скриншоты по шагам)

https://github.com/victor-homyakov/merge-cpuprofiles

##### custom visualization

google charts

##### chrome://tracing (ex about:tracing)

http://www.chromium.org/developers/how-tos/trace-event-profiling-tool/trace-event-reading

https://www.html5rocks.com/en/tutorials/games/abouttracing/

? console.time(), console.timeEnd()

##### ссылки 

https://developers.google.com/web/tools/chrome-devtools/ — документация по Chrome DevTools

https://umaar.com/dev-tips — полезные советы по DevTools

? ссылка на console API

Chrome DevTools Protocol documentation: https://chromedevtools.github.io/devtools-protocol/1-2/Profiler#type-Profile

Protocol sources: https://chromium.googlesource.com/v8/v8/+/master/src/inspector/js_protocol.json#1421

##### заключение

Чтобы красиво закончить выступление, подведите итоги, кратко повторите ключевые мысли выступления
и расскажите слушателям, чего вы теперь от них ожидаете, что они должны сделать.


01. Цель выступления
Участники мероприятия должны научиться профилировать свой код.

02. Анализ аудитории
- сколько людей будет меня слушать, какого они возраста, профессии?
    200, 20-40 лет
- какие ожидания, потребности и проблемы у моей аудитории?
- обладают ли слушатели опытом и достаточным уровнем знаний в предметной области?
    некоторые да, некоторые нет
- будут ли на мероприятии другие спикеры, выступающие на ту же тему, что и я?
    ?

03. План выступления
- о чём я хочу рассказать аудитории, описанной выше, для достижения своей цели?
- каковы ключевые идеи моего рассказа?
    1. Анализировать большое количество чисел - сложно.
    2. Анализировать картинку - просто.
    3. Результаты профилирования можно представить визуально.
Помните также, что любая презентация состоит из трех частей — вступление, основная часть, заключение.
По времени они должны распределяться примерно как 20/60/20.




До 7 февраля ты пришлёшь черновой вариант доклада
(наброски слайдов, план выступления, любые материалы по теме доклада).
До 14 февраля мы тебя послушаем (созвон с программным комитетом в скайпе).
Чем раньше — тем лучше.

Пример можно посмотреть тут: https://minskjs.timepad.ru/event/606211/

- Тема: Профилирование JS: увидеть самое важное и не утонуть в море чисел
- Описание: Профилирование JavaScript многим кажется сложным. Море малопонятных чисел, бесконечные стеки вызова,
    странные имена функций из недр используемого фреймворка... Не зря говорят: хорошая картинка стоит тысячи слов.
    Зная, как визуализировать результаты профилирования, можно облегчить и ускорить анализ узких мест кода,
    и сделать профилирование проще и приятнее.
- Спикер: Виктор Хомяков, старший разработчик интерфейсов в Яндекс. Работает в команде скорости Поиска.
    Следит за тем, чтобы страница поиска Яндекса быстро открывалась и на новых ноутах, и на старых смартфонах.
