# Освоение профессии «Front-end разработчик»
## Дисклеймер
Нижеизложенный материал представляет из себя список ссылок для самостоятельного изучения, и призван помочь начинающим IT специалистам сделать первые шаги в профессию «Front-end разработчик». Материал не является исчерпывающим и требует самостоятельного поиска ответов на вопросы, которые непонятны читателю, или не освещены в принципе.
  
Автор не является front-end разработчиком и надеется на то, что комьюнити дополнит гайд.

___

## Вопросы и ответы перед тем, как начать
**В:** Должен ли я что-то знать об IT?
**О:** Вы должны быть уверенным пользователем ОС Windows. Если вы работали с macOS или каким-либо дистрибутивом Linux — еще лучше.

**В:** Если автор не является front-end разработчиком, то чему он может научить?  
**О:** Я проходил обучение front-end разработке в большем объеме, чем того требует позиция джуна, но волею судьбы стал DevOps инженером.

**В:** Почему Front-end, а не DevOps?
**О:** Я решил начать освещать именно эту профессию, так как считаю, что соотношение **сложность входа/заработная плата** является оптимальным.

**В:** Какая цель у этого гайда?
**О:** Все чаще знакомые начинают спрашивать, как войти в IT. Я стал замечать, что разговоры затягиваются на час и более, а после них появляются оставшиеся вопросы. Написав это гайд я оптимизирую свое время и смогу давать нуждающимся одну единственную ссылку, не упустив ничего из виду. Помимо этого IT здорово изменило мою жизнь в лучшую сторону, и я хотел бы помочь другим.

**В:** Подойдет ли мне гайд, если я не хочу во front-end?
**О:** В большинстве своем нет, но вводная часть именуемая «Базовые знания» будет полезна для изучения почти всех технический IT профессий. Эта часть будет посвящена наиболее частому вопросу на собеседованиях: «Что происходит, когда вы в браузере вводите google\.com ?».

**В:** Зачем нужен этот гайд, если есть курсы?
**О:** Этот гайд является подготовкой к платным курсам, чтобы вы на них уже знали все и не плавали в материале, были любимчиком менторов и хорошо показали себя на интервью с потенциальным работодателем. Также, если вам достанется ментор, который плохо разбирается в материале, вы сможете его поймать на этом.

**В:** Будет ли гайд меняться?
**О:** Я очень надеюсь, что да. Верю в то, что знакомые профессионалы (а может даже и комьюнити) подхватит эту идею, и по итогу получится гайд без пробелов, без воды и прямой речи, который сможет заменить курсы и сэкономить вам деньги.

___

## 1. Базовые знания

Вы должны обладать пониманием процесса происходящего во время того, как вы ввели адрес сайта в браузерной строке и нажали Enter. Самый популярный вопрос на собеседованиях, касающийся этого, звучит так: «Что происходит, когда вы в браузере вводите google\.com ?».

Ниже есть несколько не очень подробных видео, которые можно посмотреть для ознакомления:
- https://www.youtube.com/watch?v=x2j_fbTsQo8
- https://www.youtube.com/watch?v=ylG8_d9Qk1U

В этих видео не говорят подробно о моделях OSI|TCP/IP и сетях. Более того, там рекомендуют избегать лишних технических подробностей. Лично я считаю, что если у тебя есть шанс блеснуть знаниями, то его нужно использовать. Ответив настолько подробно у вас повышается шанс доказать, что джуны похлеще мидлов базу знают, и что вы не просто гуманитарий, решивший войти в IT из-за хайпа, окончив лишь курсы. Поэтому я разберу более подробный пример интервью в формате вопрос-ответ:

**В:** Что происходит, когда вы в браузере вводите google\.com?
**О:** Мы идем на google\.com по протоколу https и получаем документ, который указан для этого location на веб-сервере Гугл.

**В:** Стойте, стойте. Куда и как именно вы идете?
**О:** Нам нужно разрезолвить DNS-имя google.com при помощи DNS сервера, чтобы получить IP адрес.

**В:** А как вы дойдете до DNS сервера в таком случае?
**О:** У сетевой карты компьютера есть настройки такие настройки как: IP адрес, маска сети, шлюз по умолчанию и DNS.

**В:** А откуда эти настройки берутся? Не появились же они там магическим образом.
**О:** Настройки можно ввести вручную, но скорее всего они будут получены, при подключении устройства к сети, от DHCP сервера.
> DHCP сервер выдает сетевые настройки, если что.

**В:** Хорошо. Может вы знаете, за что отвечает каждая настройка?
**О:** Да. IP адрес это сетевой адрес, по которому с устройством можно взаимодействовать на L3 уровне сетевой модели OSI. Маска сети нужна нам для того, чтобы определить во время сетевых запросов, находится ли IP адрес, на который мы хотим «сходить», в нашей локальной сети, либо за ее пределами. Если IP адрес назначения находится за пределами нашей локальной сети, то мы посылаем IP пакеты на IP адрес шлюза по умолчанию. А DNS как раз нужен затем, чтобы переводить читаемые доменные имена в интернетах в IP адреса, иначе мы бы вводили в браузер не google\.com, а 142.251.39.14.

**В:** Вы упомянули про модель OSI. Что это?
**О:** *<Тут вкратце рассказываем про 7 уровней, инкапсуляцию, декапсуляцию>*
> **Материал:**
> — Модель OSI: https://www.youtube.com/watch?v=je0QFU7p5Oo (краткое видео, можно посмотреть еще что-то самостоятельно)

**В:** Как происходит запрос к DNS серверу?
**О:** Мы отсылаем широковещательный запрос в сеть вида «Who has <IP адрес DNS сервера>?». Все компьютеры сети игнорируют этот запрос, кроме того у кого этот адрес. Тот у кого адрес отсылает вам свой MAC адрес. По системе OSI мы инкапсилуруем все данные в Ethernet кадр, и отправляем его на MAC DNS сервера (это будет верным тогда, когда DNS находится внутри вашей сети), попутно записав MAC адрес DNS сервера к себе в ARP таблицу. DNS сервер получает запрос на 53й порт и начинает работать. *<Далее рассказываем про принцип работы DNS>*
> **Материал:**
> — Сети для самых маленьких ч.2: https://linkmeup.ru/blog/1190/ (смотреть до 6:05)
> — Как работает DNS: https://www.youtube.com/watch?v=t2NMbSarXC4

**В:** Хорошо. DNS сервер поработал и вернул вам IP адрес Гугла. Дальше что?
**О:** С помощью маски сети компьютер понимает, что адрес 142.251.39.14 не находится в нашей локальной сети вида 192.168.0.0/24, и отправляет запрос на шлюз по умолчанию. А шлюз по умолчанию отправляет запрос на свой шлюз по умолчанию и так далее, пока не будет достигнут destination IP, либо пока не кончится TTL. 
> **Материал:**
> — Сети для самых маленьких ч.3: https://linkmeup.ru/blog/1190/ (смотреть до 4:20)

**В:** Хорошо. Мы добрались до сервера Гугл до того, как кончился TTL. Дальше что?
**О:** Далее происходит установка TCP сессии *<Далее рассказываем про то как ставится TCP сессия>*
> **Материал:**
> — TCP сессия: https://www.youtube.com/watch?v=vt69HEbZ_pI
> — Еще по TCP: http://ccna.mpei.ac.ru/IntroductionToNetworkTech/course/module7/7.2.1.3/7.2.1.3.html

**В:** А чем отличается TCP сессия от UDP?
**О:** TCP применяется там, где требуется точная и подтверждаемая передача данных – например, отправка фотографий, или переписка между пользователями. UDP, в свою очередь, нужен для общения в голосовом формате, или при передаче потокового видео, например, с веб-камер или IP-камер и скайпов там всяких. TCP — надежный, UDP — быстрый.

**В:** Что происходит после установки TCP сессии?
**О:** Далее происходит установка SSL/TLS сессии, в рамках которой http сессия будет зашифрована. *<Далее рассказываем про то как ставятся HTTP/HTTPS сессии>*
> **Материал:**
> — Как работает HTTP: https://www.youtube.com/watch?v=C_QZtajkDf0 
> — Еще по HTTP: https://developer.mozilla.org/ru/docs/Web/HTTP/Session
> — Как работает HTTPS: https://ru.wikipedia.org/wiki/HTTPS

***Опциональные вопросы***

**В:** Как веб-сервер понимает к какому виртуальному серверу происходит обращение?
**О:** По полю host в заголовках HTTP.

**В:** Вы вводили в браузер google\.com, то есть обратились на стандартный HTTP. Почему в результате мы попали на https://google.com?
**О:** На веб-сервере включен редирект.

**В:** Вот вы сказали, что веб-сервер определяет, какой виртуальный хост использовать по полю host в HTTP заголовках. Но HTTPS он же шифрованный! Как мы можем определить какой виртуальный хост использовать, если поле host в HTTPS зашифровано?
**О:** Идентификатор хоста передается в этом случае еще во время первичного SSL хэндшейка вместе с сертификатом подлинности.

**В:** Какие методы в HTTP вы знаете?
**О:** *<Рассказать про GET, POST, PUT и DELETE>*
> **Материал:**
> — Типы HTTP-запросов и философия REST: https://habr.com/ru/post/50147/

**В:** Какие порты использует HTTP и HTTPS?
**О:** TCP 80 и TCP 443 соответственно. 

> **Отдельной рекомендацией выделю то, что в идеале вы должны отлично поинмать то, что происходит во вкладке Networking консоли разработчика вашего браузере. Оставлю это на самостоятельное изучение.**


___

## 2. HTML, CSS, Sass, базовый Javascript 

**HTML** (от англ. HyperText Markup Language — «язык гипертекстовой разметки») — стандартизированный язык гипертекстовой разметки документов для просмотра веб-страниц в браузере. Веб-браузеры получают HTML документ от сервера по протоколам HTTP/HTTPS или открывают с локального диска, далее интерпретируют код в интерфейс, который будет отображаться на экране монитора.

**CSS** (от англ. Cascading Style Sheets «каскадные таблицы стилей») — формальный язык описания внешнего вида документа (веб-страницы), написанного с использованием языка разметки (чаще всего HTML или XHTML). Также может применяться к любым XML-документам, например, к SVG или XUL. Вкратце HTML делает скелет вашего сайта, а CSS делает сайт красивым.

**Javascript** — язык программирования, с помощью которого, сайт становится «живым». Все действия при нажатиях на кнопки, валидации форм с данными телефонов и кредитных карт и прочее — это все он. Этот язык программирования работает прямо в вашем браузере. Он, кстати, и рекламу назойливую вам показывает тоже.

**БЭМ** — методология web-разработки, которая поможет вам правильно именовать HTML элементы, что существенно упростит написание CSS.

**Sass** — это метаязык на основе CSS, предназначенный для увеличения уровня абстракции CSS-кода и упрощения файлов каскадных таблиц стилей. Sass поможет вам писать CSS быстрее. Например, вы можете назначить цвет переменной, и использовать везде переменную, вместо написания hex кода. И это самое примитивное, что умеет Sass.

**Материл:**
- HTML, CSS, базовый JavaScript: можно пройти легко и весело на тренажерах [HTML Academy](https://htmlacademy.ru/study). Подписка на месяц стоит около 1 500₽.
- БЭМ: https://ru.bem.info/methodology/quick-start/
- SASS: https://sass-scss.ru/documentation/

> Этот раздел нуждается в доработке, так как на момент прохождения HTML Academy мною, существовали лишь пара курсов и удобные в обучении тренажеры, львиная доля которых была бесплатной, а часть была доступна по платной подписке. Сейчас в новых аккаунтах этих тренажеров не найти, а в моем старом есть. Мы с моим другом поменяли мой емейл в моем старом аккаунте на его. И сейчас он пользуется тренажерами. Как временное решение: мой друг, может также сменить свой емейл на ваш. В качестве постоянного решения я покажу данный гайд знакомым фронтендерам на ревью, и, возможно, они вставят более акутальные материалы.

**Что вы должны уметь после:**
- Вы должны уметь верстать адаптивные и responsive сайты на основе БЭМ методологии (очень желательно с использованием Sass)
- Вы должны уметь базово использовать Javascript. Например, «навешивать» события на кнопки, вызывать алерты и т.д.
- Вы должны понимать что такое DOM и shadow DOM

___

## 3. Продвинутый Javascript 

**Материл:**
- Javascript deep dive: https://learn.javascript.ru (нужно прочитать от корки до корки)
- Опционально: книга «[Выразительный Javascript](https://www.litres.ru/mareyn-haverbeke/vyrazitelnyy-javascript-sovremennoe-veb-programm-50447564/otzivi/)» (опционально)

**Что вы должны уметь после:**
- Вы должны отлично знать JS
- Вы должны отлично знать ES6 и последующие стандарты
- Вы должны понимать что такое Event Loop, промисы, ассинхронность, прототипы, новый синтаксический сахар новых  ECMAScript и т.д.
- Вы должны уметь импортировать сторонние библиотеки и писать свои

___

## 4. React, Git, NPM, WebPack

**React** — это очень популярная JavaScript библиотека для создания пользовательских интерфейсов. Она была выпущена в мае 2013 года и в настоящее время используется не только для создания веб-интерфейсов, но также для разработки мобильных (React Native) и настольных приложений (React с Electron).

**Git** — это система управления версиями с распределенной архитектурой. В git репозиториях выполняется вся работа с кодом на проектах.

**NPM** — менеджер пакетов. Нужен для того, чтобы удобно скачивать зависимости для проекта одной командой, вместо того, чтобы скачивать библиотеки вручную.

**Webpack** — соберет ваше React приложение.

**Материл:**
- React: книга «[React и Redux. Функциональная веб-разработка](https://www.litres.ru/a-benks-piter/react-i-redux-funkcionalnaya-veb-razrabotka-pdf-epu-29415793/otzivi/) (книга слегка устарела, например, в ней ничего нет o webhooks, но зато она дает отличное понимание того, как React работает под капотом)
- Документация по React: https://ru.reactjs.org (закроет вопросы не освещенные в книге. И, вообще, привыкайте читать документацию.)
- Git: https://learngitbranching.js.org/?locale=ru_RU
- Gitflow: https://www.atlassian.com/ru/git/tutorials/comparing-workflows/gitflow-workflow
- Видео по Gitflow: https://www.youtube.com/watch?v=rC6varfUhCo
- Краткий обзор NPM: https://www.youtube.com/watch?v=sL6VvWOAuLE (поиск более подробной информации остается за читателем)
- Webpack: https://www.youtube.com/watch?v=eSaF8NXeNsA

**Что вы должны уметь после:**
- Вы должны отлично React со всеми фичами
- Вы должны уметь хранить состояние в Redux
- Вы должны уметь работать с базовыми git командами: clone, commit, checkout, merge rebase, log, diff, reset, remote, stash.
- Вы должны уметь работать с Gitflow
- Вы должны знать зачем нужен NPM, как установить зависимость, как установить зависимость конкретной версии, и в чем отличие package.json от package-lock.json.
- Вы должны понимать конфигурационный файл Webpack, как подключить транспиляторы и уметь настраивать плагины по их официальной документации.
- Уметь тестировать свой код с помощью Jest и react-testing library.

___

## 5. Курсы
Если вы прошли весь материал и все поняли, то на курсах вы будете самым умным, легко их закончите, увеличите шанс прохождения интервью, и будете требовать от менторов большего, чем они дают. Знания получатся более консистентные.

При должном уровне практики, вы можете вообще не ходить ни на какие курсы. Просто делаете свое портфолио на гите и вперед с ним на собеседования.

Советы по выбору курсов: 
- Смотрите и сравнивайте программы
- Не гонитесь за ценой
- Читайте отзывы о курсах каждой онлайн школы
- Думаю не стоит объяснять, что курсы от Яндекс практикум или Geekbrains будут лучше, чем noname курсы
- Смотрите, чтобы по окончанию курсов предлагалась возможность трудоустройства

Удачи вам!

___

## Полезные ссылки:

- Front-end roadmap 2022: https://roadmap.sh/frontend
