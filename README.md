# op2ogse
Адаптация движка и некоторых фич OGSE 0.6.9.3 к ОП-2

Форум адаптации и ссылки на скачивание для игроков находятся
здесь:

- http://stalker-worlds.ru/forum/topic/3355-kovyriaemsia-v-ogse/?p=174181

- http://www.amk-team.ru/forum/index.php?showtopic=13176

Изменения, по сравнению с ОП-2:

- В расширенных настройках графики, не включайте опцию "Детальный
  бамп", если не имеете на то веских оснований.

- В настройках игры необходимо назначить заново клавиши для ПНВ,
  напоминаний, ускорителя и быстрого сохранения.

- Погода и выброс заменены на те, что в OGSE.

- Теперь мины выкладываются ровно перед ГГ, на пол. метра впереди.

- Добавил доп. способы массового переноса вещей:

  Первый вариант - это переносить предмет, удерживая клавишу Shift.

  Второй вариант - это выделить предмет мышью и нажать клавишу "Z".

  Способ ОП-2, перенести предмет и нажать "Z" для переноса оставшихся
  предметов - тоже работает.

- Сейвы, которые делает эта адаптация, не будут загружаться в ОП-2,
  Можно сделать специальный квиксейв, который загрузится в ОП-2. Для
  этого нужно выйти в главное меню и нажать F6. Будет сделан сейв с
  именем op2quicksave.

- При загрузке восстанавливается активный оружейный слот.

- Коллиматорные прицелы теперь видны в темноте.

- Светошумовые гранаты теперь не действуют на главного героя, когда он
  находится в укрытии. Принцип такой: эффект от светошумовой гранаты
  будет, если она сработает на расстоянии не более 5-ти метров И
  граната "видит" голову главного героя.

- Прожектора на блокпостах выключаются утром и включаются вечером.

- Менеджер сна из OGSE

- Костюмы, которые должны лечить, теперь действительно лечат.

- Поменял партикл попадания от огнемета на OGSE-ешный. Он не просаживает FPS.

- Поправил несколько вылетов, при отравлении ГГ Гавром.

- Немного оптимизировал замки. При наличии в тайнике нескольких замков,
  тайник все равно будет считаться закрытым, даже если один из замков забрать,
  пока в тайнике имеется хотя бы один замок.

- Исправил вылет, иногда возникающий при автоподборе вещей из трупиков.

- Артефакты, влияющие на голод ГГ, теперь действительно на него влияют.

- Добавил быстрое использование антирадов/сыворотки. Клавиша назначается в
  настройках игры. При отсутствии антирада в инвентаре, используется
  сыворотка.

- Добавил опцию "Погода без дождя" в АМК настройки.

- У оружия с ночным прицелом (СВД Филин, например), ПНВ автоматически не
  включается. Нужно включать вручную.

- Что бы работал ПНВ, его необходимо перенести в свой слот.

- Для детекторов артефактов и биорадаров есть свои слоты. Впрочем, на поясе
  они тоже будут работать.

- Скриптовая логика боя неписей из OGSE

  Совет: никогда не стреляйте на виду у Кузнецова и его группы. Ни в кого.

- Изменен режим паузы после загрузки. При включенной опции
  используется пауза ОП-2, иначе - используется пауза OGSE.

- Грузоподъемность всех костюмов зависит от их состояния. Больший
  износ - меньшая грузоподъемность.

- Изменен третий апгрейд СКАТа-15.

  Дополнительные +20 кг. переносимого веса появляются только при
  наличии на поясе артефакта Черная энергия.  Без этого, переносимый
  вес будет такой же, как у второго апгрейда.  При повышенной
  загрузке, т.е. когда начинают использоваться эти дополнительные 20
  кг., Черная энергия начинает тратиться со скоростью 2 часа
  непрерывного грузопереноса. Если доп. вес не используется, то и
  Черная энергия не тратится.

- Перенес вид, звук и поведение некоторых аномалий из OGSE.

  Поглядывайте по сторонам и пользуйтесь болтами, если что.

- Поддержка шкалы пси здоровья на худе.

- Сталкеры в шлемах и противогазах больше не едят и не пьют сквозь них.

- Добавлен режим разрядки артефактов на поясе.

  Идея этого режима пришла мне в голову, когда я понял, что уже сотню игровых
  дней у меня на поясе висят одни и те же артефакты. Как я их повесил
  когда-то, так они все и используются. И полагаю, до самого конца игры, так
  меня и защищали-бы эти же самые артефакты. Т.е. они принимают на себя
  попадания пуль, осколков гранат и взрывы и им хоть бы что. Не-е-е-е,
  так не бывает. И вот пришла мне мысль, что пусть артефакты обладают
  способностью поглотить определенное кол-во энергии воздействий, от которых
  они защищают. Готово. При включенном режиме, артефакты на поясе будут
  постепенно разряжаться, нейтрализуя вредные воздействия. После полного
  разряда, артефакт превратится в Булыжник. Величина максимальной поглощенной
  энергии зависит от уровня сложности. Чем сложнее, тем меньше. Так же, в
  этом режиме отключается защита, не позволяющая превышать артефактами на поясе
  определенный уровнь защиты. Можно хоть, как елка, обвешаться артефактами и
  пойти гулять по блок-посту военных. Если, конечно, артефактов не жалко,
  которые такой прогулки могут и не пережить.

  Опция, включающая этот режим, находится в АМК Опциях и называется:
  "Постепенный разряд артефактов на поясе".

  Имейте ввиду, разряжаются любые артефакты, даже уникальные и квестовые.
  Т.ч. думайте сами, использовать такие и следить за их состоянием, что бы
  они не успели в Булыжники превратиться или в тайнике держать.

  В этом режиме учитывается пулестойкость брони. Т.к. параметр
  пулестойкости брони не используется игрой, я добавил его эмуляцию,
  но только в ослабленном виде. Например, у СКАТа-15 пулестойкость
  55%. С такой защитой ГГ практически неуязвим. Поэтому используется
  коэффициент, который зависит от величины хита. Т.е. чем больше полученный
  хит, тем большая часть пулезащиты костюма используется, но в любом случае,
  не меньше 10% от пулезащиты брони. Таким образом, в том же СКАТе-15,
  пулезащита будет минимум 5.5%. Максимум пулезащиты, 55%, будет
  использоваться только при достаточно большом уроне.

- Для использования ремкомплектов, необходимо иметь в инвентаре что-нибудь
  на разборку.

  Это что-нибудь должно иметь состояние не менее 15%. Величина, на
  которую будет отремонтирован предмет, зависит от состояния
  разбираемого, но всегда не менее 10%.

- Добавил в АМК опции возможность выключить оффлайновую симуляцию боев

  А то вот вооружаешь сталкеров, вооружаешь, а потом приходишь, а там
  труп.

- NPC, имеющие оружие с оптическим прицелом или снайперское оружие,
  стреляют точнее.

- "Умное" выпадение частей некоторых мутантов

  Включается в АМК Опциях. Если гарантированно хотите снять с
  кровососа шупальца, то не стрелйте ему в голову. И т.п. для других
  мутантов.

- Что бы отрезать часть мутанта, ножа надо иметь не в рюкзаке, а в руках.

  А что бы обыскать тело непися, наоборот, руки должны быть свободны.

- Звуки отрезания запчастей мутантов включаются в АМК опциях

- Для работы ПНВ, необходимо иметь на поясе аккумулятор.

  Аккумуляторы продает Сахаров. Их можно подзаряжать, используя артефакты
  "Темная энергия" или "Батарейка". Разные ПНВ с разной скоростью тратят
  заряд аккумулятора. Чем ПНВ лучше, тем быстрее он разряжает аккумулятор.


Установка:

- Переименовываем папку bin, например в binОП2

- Удаляем или переименовываем gamedata, если есть

- Копируем всё из архива в папку с игрой и соглашаемся на замену.

- Всё.

Откат:

- Удаляем папку bin и файл gamedata.dbw, обратно переименовываем папку bin от
  ОП-2.

- Всё.


Хочу выразить благодарность:

- Команде ОП-2 за отличный мод

- Команде OGSE за отличный код

- людям, чьи работы я использовал или кто мне помогал другим способом:
  art0run, BlooderDen.
