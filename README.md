![IAB Tech Lab](https://drive.google.com/uc?id=10yoBoG5uRETSXRrnJPUDuONujvADrSG1)

# **AdCOM 1.0**

#### Executive Summary
Одним из наиболее успешных стандартов IAB является OpenRTB.  Этот протокол для проведения аукционов в режиме реального времени между биржами, работающими на стороне продавца, и участниками торгов на стороне спроса впервые был запущен как OpenRTB v1.0 Mobile в феврале 2011 года.  Позже в том же году была выпущена версия OpenRTB v2.0, в которой был представлен единый протокол для мобильных устройств, дисплеев и видео.  Благодаря широкому распространению OpenRTB в январе 2012 года, с выходом версии v2.1, он был признан стандартом IAB, хотя управление техническим контентом оставалось за сообществом OpenRTB.  С тех пор и в соответствии со своей первоначальной целью OpenRTB стал лингва франка программной рекламы в реальном времени и в 2018 году вступил в силу в версии 2.5.

За эти годы программная реклама стала доминирующей силой в отрасли.  Однако это также привело к усложнению цепочки поставок, что может повысить уровень мошенничества и других рисков.  Это один из ключевых мотивов, побудивших OpenRTB v3.0, поскольку уровень изменений, необходимый для решения проблем programmatic в настоящее время и в будущем, не может быть реализован в виде обратной совместимости (т. е. в виде дополнительного релиза v2.x).

В сочетании с целью OpenMedia по рационализации портфеля стандартов IAB, это привело к многоуровневому подходу, где OpenRTB будет фокусироваться на фактических сделках медиа-коммерции (например, параметры аукциона, сделки, предложения и т.д.), в то время как концепции, общие с другими спецификациями (например, реклама, размещение, пользователи, устройства, сайты, издатели и т.д.) будут включены в собственную многократно используемую спецификацию.  Так возникла общая объектная модель рекламы (Advertising Common Object Model или AdCOM).

Помимо обеспечения модульности, позволяющей использовать спецификации в дополнение к OpenRTB, AdCOM стремится решить и другие бизнес-задачи программной рекламы.  Например, издатели в настоящее время имеют ограниченную возможность контролировать типы креативов, которые они запускают на своих сайтах, из-за непрозрачной природы, в которой передается традиционная дисплейная реклама.  Многие типы нежелательных креативов попадают в контент издателя, например, слишком тяжелые полезные нагрузки, те, которые не обеспечивают безопасность бренда, чрезмерное количество пикселей и JavaScript, запускающий вредоносное ПО.

Эти и другие проблемы приводят к плохому и потенциально вредному опыту пользователей, снижению доверия пользователей, установке блокировщиков рекламы, снижению монетизации издателей, а также к тому, что добросовестным рекламодателям становится все труднее достичь своей целевой аудитории.  AdCOM пытается решить эти проблемы, поддерживая новые и более безопасные структурированные рекламные форматы.

Возможность многократного использования различных спецификаций IAB позволяет AdCOM использовать подобные решения в различных отраслях.

#### Об этом репозитории
Ветка **master** этого репозитория всегда содержит самый последний выпуск AdCOM. Смотрите ["AdCOM v1.0 Final.md"](https://github.com/InteractiveAdvertisingBureau/AdCOM/blob/master/AdCOM%20v1.0%20FINAL.md) в основной ветке для получения последней версии спецификации.

Существуют ветви для предыдущих выпусков. Используйте их, чтобы просмотреть подробные изменения от одного выпуска к другому. Краткий журнал изменений находится в самой спецификации.

Ветка **develop** содержит незавершенные работы для грядущего релиза. Она может измениться в любой момент.

#### OpenMedia
https://iabtechlab.com/openmedia 

#### OpenRTB 
https://github.com/InteractiveAdvertisingBureau/openrtb

#### Contact
Чтобы получить дополнительную информацию или принять участие, пожалуйста, напишите openmedia@iabtechlab.com.

#### О IAB Tech Lab  

Технологическая лаборатория IAB (Tech Lab) - это некоммерческий консорциум по исследованиям и разработкам, который разрабатывает и предоставляет стандарты, программное обеспечение и услуги для стимулирования роста эффективной и устойчивой глобальной экосистемы цифровых медиа. IAB Tech Lab, в состав которой входят цифровые издатели и компании, занимающиеся рекламными технологиями, а также маркетологи, агентства и другие компании, заинтересованные в интерактивном маркетинге, стремится обеспечить рост брендов и СМИ за счет прозрачной, безопасной и эффективной цепочки поставок, более простых и последовательных измерений и лучшего рекламного опыта для потребителей, уделяя особое внимание развитию мобильных и ТВ/цифровых видеоканалов. В портфолио IAB Tech Lab входит служба стандартизированной идентификации DigiTrust, работающая в режиме реального времени и предназначенная для улучшения цифрового опыта потребителей, издателей, рекламодателей и сторонних платформ. В состав совета директоров входят AppNexus, ExtremeReach, Google, GroupM, Hearst Digital Media, Integral Ad Science, Index Exchange, LinkedIn, MediaMath, Microsoft, Moat, Pandora, PubMatic, Quantcast, Telaria, The Trade Desk и Yahoo! Japan. Основанная в 2014 году, IAB Tech Lab имеет штаб-квартиру в Нью-Йорке, офис в Сан-Франциско и представительства в Сиэтле и Лондоне.

Узнать больше о лаборатории IAB Tech Lab можно здесь: [https://www.iabtechlab.com/](https://www.iabtechlab.com/)


#### Contributors and Technical Governance

Члены рабочей группы OpenRTB вносят свой вклад в этот репозиторий. Участники рабочей группы OpenRTB должны быть членами IAB Tech Lab. Техническое руководство и коммиты кода для проекта обеспечиваются группой IAB Tech Lab OpenRTB Commit Group.

### Лицензия
Лицензия OpenRTB Specification the IAB Tech Lab распространяется на условиях Creative Commons Attribution 3.0 License.   Чтобы ознакомиться с копией этой лицензии, посетите сайт https://creativecommons.org/licenses/by/3.0/ или напишите по адресу Creative Commons, 171 Second Street, Suite 300, San Francisco, CA 94105, USA.

Предоставляя идею, спецификацию, программный код, документ, файл или другой материал (каждый - "Представление") в репозиторий AdCOM, любому члену рабочей группы Programmatic Supply Chain Working Group или в IAB Tech Lab в связи с AdCOM, вы соглашаетесь и настоящим лицензируете такое Представление IAB Tech Lab на условиях лицензии Creative Commons Attribution 3.0 License и соглашаетесь, что такое Представление может быть использовано и доступно для общественности на условиях такой лицензии. Если вы являетесь членом IAB Tech Lab, то к вашему Представлению также могут быть применимы положения и условия [Политики ПИС](https://iabtechlab.com/ipr-iab-techlab/acknowledge-ipr/), и если Политика ПИС применима к вашему Представлению, то Политика ПИС будет иметь преимущественную силу в случае конфликта между Лицензией Creative Commons Attribution 3.0 и Политикой ПИС.

#### Отказ от ответственности

СТАНДАРТЫ, СПЕЦИФИКАЦИИ, РУКОВОДСТВА ПО ИЗМЕРЕНИЯМ И ЛЮБЫЕ ДРУГИЕ МАТЕРИАЛЫ ИЛИ УСЛУГИ, ПРЕДОСТАВЛЯЕМЫЕ ИЛИ ИСПОЛЬЗУЕМЫЕ ВАМИ ПО НАСТОЯЩЕМУ ДОКУМЕНТУ ("ПРОДУКТЫ И УСЛУГИ"), ПРЕДОСТАВЛЯЮТСЯ "КАК ЕСТЬ" И "КАК ДОСТУПНО", И IAB TECHNOLOGY LABORATORY, INC. ("TECH LAB") НЕ ДАЕТ НИКАКИХ ГАРАНТИЙ В ОТНОШЕНИИ НИХ И НАСТОЯЩИМ ОТКАЗЫВАЕТСЯ ОТ ВСЕХ ЯВНЫХ, ПОДРАЗУМЕВАЕМЫХ ИЛИ УСТАНОВЛЕННЫХ ЗАКОНОМ ГАРАНТИЙ, ВКЛЮЧАЯ, БЕЗ ОГРАНИЧЕНИЙ, ЛЮБЫЕ ГАРАНТИИ ТОВАРНОГО СОСТОЯНИЯ, ПРИГОДНОСТИ ДЛЯ КОНКРЕТНОЙ ЦЕЛИ, ДОСТУПНОСТИ, БЕЗОШИБОЧНОЙ ИЛИ БЕСПЕРЕБОЙНОЙ РАБОТЫ, А ТАКЖЕ ЛЮБЫЕ ГАРАНТИИ, ВЫТЕКАЮЩИЕ ИЗ ХОДА СДЕЛКИ, ХОДА ИСПОЛНЕНИЯ ИЛИ ИСПОЛЬЗОВАНИЯ В ТОРГОВЛЕ. В ТОЙ МЕРЕ, В КАКОЙ TECH LAB НЕ МОЖЕТ В СООТВЕТСТВИИ С ПРИМЕНИМЫМ ЗАКОНОДАТЕЛЬСТВОМ ОТКАЗАТЬСЯ ОТ КАКОЙ-ЛИБО ПОДРАЗУМЕВАЕМОЙ ГАРАНТИИ, ОБЪЕМ И ПРОДОЛЖИТЕЛЬНОСТЬ ТАКОЙ ГАРАНТИИ БУДУТ МИНИМАЛЬНЫМИ, РАЗРЕШЕННЫМИ В СООТВЕТСТВИИ С ТАКИМ ЗАКОНОДАТЕЛЬСТВОМ. ПРОДУКТЫ И УСЛУГИ НЕ ЯВЛЯЮТСЯ ДЕЛОВЫМИ ИЛИ ЮРИДИЧЕСКИМИ КОНСУЛЬТАЦИЯМИ. TECH LAB НЕ ГАРАНТИРУЕТ, ЧТО ПРОДУКТЫ И УСЛУГИ, ПРЕДОСТАВЛЯЕМЫЕ ИЛИ ИСПОЛЬЗУЕМЫЕ ВАМИ ПО НАСТОЯЩЕМУ ДОКУМЕНТУ, ПРИВЕДУТ ВАС И/ИЛИ ВАШИ ПРОДУКТЫ ИЛИ УСЛУГИ В СООТВЕТСТВИЕ С ЛЮБЫМИ ПРИМЕНИМЫМИ ЗАКОНАМИ, НОРМАТИВНЫМИ АКТАМИ ИЛИ СИСТЕМАМИ САМОРЕГУЛИРОВАНИЯ, И ВЫ НЕСЕТЕ ПОЛНУЮ ОТВЕТСТВЕННОСТЬ ЗА ИХ СОБЛЮДЕНИЕ, ВКЛЮЧАЯ, В ЧАСТНОСТИ, ЗАКОНЫ О ЗАЩИТЕ ДАННЫХ, ТАКИЕ КАК ЗАКОН О ЗАЩИТЕ ПЕРСОНАЛЬНОЙ ИНФОРМАЦИИ И ЭЛЕКТРОННЫХ ДОКУМЕНТОВ (КАНАДА), ДИРЕКТИВА О ЗАЩИТЕ ДАННЫХ (ЕС), ДИРЕКТИВА ОБ ЭЛЕКТРОННОЙ КОНФИДЕНЦИАЛЬНОСТИ (ЕС), ОБЩЕЕ ПОЛОЖЕНИЕ О ЗАЩИТЕ ДАННЫХ (ЕС) И ПОЛОЖЕНИЕ ОБ ЭЛЕКТРОННОЙ КОНФИДЕНЦИАЛЬНОСТИ (ЕС), КОГДА ОНИ ВСТУПЯТ В СИЛУ.
