## Подробное описание кнопок инструментов

?> Все кнопки можно скрыть или показать в `Настройках отображения` -> `Кнопки инструментов`.<br>
Можно свободно изменять позицию всех кнопок. Кнопки можно группировать по `лево`, `по центру`, `право`, и изменения относительных позиций будут ограничены в пределах группы.<br>
Цвет кнопок можно настроить в `Настройках отображения` -> `Настройки интерфейса` -> `Панель инструментов` -> `Цвет кнопок`.<br>
Некоторые кнопки имеют два значка, чтобы указать две разные состояния. Некоторые кнопки имеют только один значок, но разные цвета для разных состояний.

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css"> 

<style>
    i{
        color: blue;
        width: 20px;
    }
    .fa-icon {
  visibility: hidden;
}
.btnstatus2{
    color: deeppink;
}
</style>

1. #### <i class="fa fa-rotate-right"></i> <i class="fa fa-icon fa-rotate-right"></i> Ручной перевод
    Фактически означает, что с текущего источника текстового ввода прочитается входной текст один раз и будет выполнен перевод.
    Например, если в настоящее время выбран режим OCR, будет выполнена еще одна OCR-операция.

1. #### <i class="fa fa-forward"></i> <i class="btnstatus2 fa fa-forward"></i> Автоматический перевод
    Фактически означает, что приостановить/продолжить автоматическое чтение текста из текущего источника текстового ввода.
    Например, если в настоящее время выбран режим HOOK, чтение текста игры будет приостановлено; в режиме OCR, приостановится автоматическое распознавание изображений; в режиме буфера обмена, приостановится автоматическое чтение буфера обмена.

1. #### <i class="fa fa-gear"></i> <i class="fa fa-icon fa-rotate-right"></i> Открыть настройки
    Краткое описание

1. #### <i class="fa fa-file"></i> <i class="fa fa-icon fa-rotate-right"></i> Прочитать буфер обмена
    Фактически означает, что независимо от текущего источника текстового ввода, с буфера обмена будет прочитан текст один раз и передан в последующий процесс перевода/TTS/...

1. #### <i class="fa fa-heart"></i> <i class="fa fa-icon fa-rotate-right"></i> Коллекция
    Который в основном предназначен для создания отдельных закладок для каждой игры. Автоматически ищет метаданные для страниц с коллекцией игр на vndb/bangumi/dlsite/ и т.д., также можно вручную добавить некоторые веб-страницы, связанные с этой игрой (например, веб-страницы с гайдами по игре, помимо использования блокнота, можно использовать эту функцию для хранения закладок), что облегчает просмотр. Избавляет от необходимости создавать закладки в браузере и управлять ими.<br>
    Нажмите правой кнопкой на всплывающее меню, в котором будут перечислены страницы коллекции, а левой кнопкой - всплывающее окно, которое позволит редактировать содержимое коллекции.

1. #### <i class="fa fa-futbol"></i> <i class="fa fa-icon fa-rotate-right"></i> Настройки игры
    При использовании режима HOOK для подключения к игре или привязке окна игры в режиме OCR, можно использовать эту кнопку для прямого открытия окна настроек текущей игры
1. #### <i class="fa fa-mouse-pointer"></i> <i class="btnstatus2 fa fa-mouse-pointer"></i> Прозрачность окна мыши
    Активация этой кнопки приводит к тому, что при щелчке мышью на окне перевода окно перевода не реагирует на щелчок, а передает событие клика в окно ниже.<br>
    Когда окно перевода размещено над текстовым полем окна игры, активация этой кнопки позволяет щелкнуть текстовое поле игры, а не окно перевода.<br>
    При перемещении мыши в **область кнопки прозрачности окна мыши и одной кнопки слева или справа от нее**, прозрачность автоматически отключается для использования кнопок инструментов; когда мышь выходит из этой области, прозрачность возвращается.

1. #### <i class="fa fa-lightbulb"></i> <i class="btnstatus2 fa fa-lightbulb"></i> Прозрачность фонового окна
    Функция этой кнопки заключается в одном нажатии для переключения непрозрачности окна перевода в 0. Этот переключатель не забывает настройки непрозрачности по умолчанию.

1. #### <i class="fa fa-lock"></i> <i class="btnstatus2 fa fa-unlock"></i> Закрепить панель инструментов
    Если панель инструментов не зафиксирована, при перемещении мыши за пределы панели она автоматически скрывается; после активации панель инструментов будет всегда видна.<br>
    Если панель инструментов не зафиксирована и активирована `прозрачность окна мыши`, панель инструментов будет отображаться только при перемещении мыши в **область кнопки прозрачности окна мыши и одной кнопки слева или справа от нее**; в противном случае панель инструментов отображается при любом входе мыши в окно перевода.<br>
    Если в настоящее время используются эффекты окон (Aero/Arylic) и панель инструментов не зафиксирована, панель инструментов будет находиться в области z-оси над областью текста, а не находиться на y-оси над областью текста. Это связано с тем, что из-за Windows, при использовании эффектов окон, если панель инструментов просто скрывается, а не уменьшается по высоте окна, скрытая панель инструментов все равно будет отображаться с прозрачным фоном Alyric/Aero, что приводит к появлению белого пятна в области панели инструментов.
1. #### <i class="fa fa-link"></i> <i class="fa fa-icon fa-rotate-right"></i> Выбор игры
    **Эта кнопка доступна только в режиме HOOK**<br>
    При нажатии на кнопку открывается окно выбора процесса игры для HOOK.

1. #### <i class="fa fa-tasks"></i> <i class="fa fa-icon fa-rotate-right"></i> Выбор текста
    **Эта кнопка доступна только в режиме HOOK**<br>
    При нажатии на кнопку открывается окно выбора текста игры для перевода.<br>
    Однако окно выбора текста автоматически появляется после выбора процесса, и эта кнопка фактически используется для замены выбранного текста или изменения некоторых настроек.

1. #### <i class="fa fa-crop"></i> <i class="fa fa-icon fa-rotate-right"></i> Выбор области OCR
    **Эта кнопка доступна только в режиме OCR**<br>
    В режиме OCR выбирать область OCR, изменять область OCR или добавлять новую область OCR при активации `OCR настройки` -> `Другие` -> `Многообластный режим`.<br>
    При нажатии правой кнопки мыши все выбранные области сначала будут очищены, а затем добавлены новые.
1. #### <i class="fa fa-square"></i> <i class="fa fa-icon fa-rotate-right"></i> Показать/Скрыть рамку области 
    **Эта кнопка доступна только в режиме OCR**<br>
    Когда никакая область OCR не выбрана, используйте эту кнопку, чтобы отобразить область OCR, автоматически устанавливая область OCR в последний выбранный OCR.<br>
    При нажатии правой кнопки будет очищен весь выбранный диапазон
1. #### <i class="fa fa-crop"></i> <i class="fa fa-icon fa-rotate-right"></i> Выполнить одинOCR
    Эта кнопка аналогична кнопке `Прочитать буфер обмена`, независимо от текущего источника текстового ввода, сначала выбирается область OCR, затем выполняется один OCR, а затем процесс перевода.<br>
    Обычно эта кнопка используется в режиме HOOK, когда при выборе ветвей, временно используется OCR для перевода ветвей. Или в режиме OCR, чтобы временно распознать новый случайный появляющийся раз в другом месте.<br>

1. #### <i class="fa fa-spinner"></i> <i class="fa fa-icon fa-rotate-right"></i> Повторное выполнение OCR
    После использования кнопки `Выполнить одинOCR`, при нажатии этой кнопки можно снова выполнить OCR в исходном положении без повторного выбора области распознавания.

1. #### <i class="fa fa-book"></i> <i class="fa fa-icon fa-rotate-right"></i> Перевод собственных названий_прямое замещение
1. #### <i class="fa fa-book"></i> <i class="fa fa-icon fa-rotate-right"></i> Перевод собственных названий_глобально
1. #### <i class="fa fa-book"></i> <i class="fa fa-icon fa-rotate-right"></i> Перевод собственных названий
1. #### <i class="fa fa-won"></i> <i class="fa fa-icon fa-rotate-right"></i> Исправление результатов перевода_глобально
1. #### <i class="fa fa-won"></i> <i class="fa fa-icon fa-rotate-right"></i> Исправление результатов перевода
    Эти пять кнопок похожи по эффекту, они предназначены для быстрого открытия окна настроек оптимизации перевода, добавления новых указанных терминов.<br>
    Для `глобального`, всегда открывается глобальное настройки словаря. Для не `глобального`, при наличии привязанной игры (HOOK-соединение игры/буфер обмена, окно OCR-привязки), открывается настройки специализированного словаря для игры, в противном случае открываются глобальные настройки словаря.

1. #### <i class="fa fa-minus"></i> <i class="fa fa-icon fa-rotate-right"></i> Свернуть в системный трей
    Краткое описание

1. #### <i class="fa fa-times"></i> <i class="fa fa-icon fa-rotate-right"></i> Выход
    Краткое описание

1. #### <i class="fa fa-hand-paper"></i> <i class="fa fa-icon fa-rotate-right"></i> Перемещение
    Перемещение окна перевода.<br>
    На самом деле, когда на панели кнопок есть дополнительное пустое пространство без кнопок, можно свободно перемещать. Эта кнопка используется только для резервирования позиции для перемещения.

1. #### <i class="fa fa-compress"></i> <i class="fa fa-expand"></i> Изменение масштаба окна
    Можно одним нажатием изменить масштаб окна игры (HOOK-соединение игры/буфер обмена, окно OCR-привязки) (по умолчанию используется встроенный Magpie, также можно настроить использование скачанного Magpie и т.д.).<br>

1. #### <i class="fa fa-camera"></i> <i class="fa fa-icon fa-rotate-right"></i> Снимок окна
    Можно сделать снимок привязанного окна (по умолчанию делает два снимка, GDI и Winrt, оба имеют некоторую вероятность сбоя). Лучшее место, если в настоящее время используется Magpie для масштабирования, также будет делать снимок увеличенного окна.<br>
    Снимок экрана будет сохранен в файле при щелчке левой кнопкой мыши, а снимок экрана будет сохранен в буфере обмена при щелчке правой кнопкой мыши.

1. #### <i class="fa fa-volume-off"></i> <i class="btnstatus2 fa fa-volume-up"></i> Выключение звука игры
    После привязки окна игры (не только в режиме HOOK, но и в режиме OCR или буфера обмена, если только окно игры привязано), можно одним нажатием выключить звук игры, избавившись от необходимости отключать звук игры в системном микшере.

1. #### <i class="fa fa-eye"></i> <i class="btnstatus2 fa fa-eye-slash"></i> Показать/скрыть исходный текст
    Переключение отображения исходного текста, вступает в силу немедленно.

1. #### <i class="fa fa-toggle-on"></i> <i class="btnstatus2 fa fa-toggle-off"></i> Показать/скрыть перевод
    Переключение использования перевода, является общим переключателем перевода, после его отключения не будет выполнено никакого перевода.<br>
    Если перевод уже выполнен, после отключения он будет скрыт, и при повторном включении будет снова отображаться результат текущего перевода.<br>
    Если перевод еще не выполнен и переключение скрытия на отображение, будет инициирован перевод текущего предложения.

1. #### <i class="fa fa-music"></i> <i class="fa fa-icon fa-rotate-right"></i> Чтение
    Левый клик по кнопке будет читать текущий текст с синтезом речи.<br>Правый клик на кнопке прерывает чтение.<br>    Это чтение игнорирует `пропуск` (если в `голосовых настройках` соответствует текущему тексту цель `пропуск`, то при использовании кнопки для чтения будет проигнорирован пропуск и будет принудительно прочитано)

1. #### <i class="fa fa-copy"></i> <i class="fa fa-icon fa-rotate-right"></i> Копировать в буфер обмена
    Копирование текущего извлеченного текста в буфер обмена один раз. Если вы хотите автоматически извлечь в буфер обмена, следует активировать `Текстовый ввод` -> `Вывод текста` -> `Буфер обмена` -> `Автоматическое вывод`.

1. #### <i class="fa fa-rotate-left"></i> <i class="fa fa-icon fa-rotate-right"></i> Показать/скрыть историю переводов
    Открыть или закрыть окно истории переводов.

1. #### <i class="fa fa-gamepad"></i> <i class="fa fa-icon fa-rotate-right"></i> Управление игрой
    Открыть интерфейс менеджера игр.

1. #### <i class="fa fa-edit"></i> <i class="fa fa-icon fa-rotate-right"></i> Редактирование
    Открыть окно редактирования, запустить редактирование текущего извлеченного текста.<br>
    В этом окне можно изменить текст, а затем перевести; или перевести любой введенный текст.

1. #### <i class="fa fa-edit"></i> <i class="fa fa-icon fa-rotate-right"></i> Редактирование_журнал переводов
    Открыть окно редактирования журнала переводов текущей игры.

1. #### <i class="fa fa-download"></i> <i class="fa fa-icon fa-rotate-right"></i> Имитация нажатия клавиши Ctrl
11. #### <i class="fa fa-download"></i> <i class="fa fa-icon fa-rotate-right"></i> Имитация нажатия клавиши Enter
    Так же, для отправки имитации нажатия клавиши в окно игры. Может быть полезно при использовании потоковой передачи/планшета.

1. #### <i class="fa fa-list-ul"></i> <i class="fa fa-icon fa-rotate-right"></i> Заметки
    Открыть окно заметок для текущей игры, которая находится в процессе игры. Для каждой игры есть отдельный файл заметок.<br>
    Можно использовать для временной записи заметок или копирования стратегий для игры и удаления их по мере прохождения, очень удобно, избавляя от необходимости открытия веб-страниц/отдельного файла txt, очень практично.

1. #### <i class="fab fa-windows"></i> <i class="btnstatus2 fab fa-windows"></i> Привязка окна (не поддерживается некоторыми программами) (нажмите, чтобы отменить)
    **Эта кнопка очень важна, многие функции зависят от предварительной настройки этой кнопки**<br>
    После привязки окна игры, такие функции, как `изменение масштаба окна`, `снимок окна`, `выключение звука игры`, `следование за окном игры` -> `снять привилегированный режим, когда игра теряет фокус` и `синхронное перемещение с окном игры`, а также учет времени игры и т. д., становятся доступными.
    Независимо от режима HOOK/OCR/буфера обмена эта кнопка доступна.<br>
    В режиме HOOK автоматически привязывается к окну игры, соединенной с игрой, но также можно использовать эту кнопку для повторного выбора другого окна.<br>
    В режиме OCR после привязки окна дополнительно разрешается синхронное автоматическое перемещение области и рамки OCR при перемещении окна игры.
    
    В режиме OCR/буфера обмена после привязки окна также можно, как и в режиме HOOK, связать текущую игру с настройками игры, чтобы использовать специализированный словарь оптимизации перевода для текущей игры и т. д.

1. #### <i class="fa fa-neuter"></i> <i class="btnstatus2 fa fa-neuter"></i> Окно на переднем плане
    Отменить/установить окно перевода на передний план

1. #### <i class="fa fa-i-cursor"></i> <i class="btnstatus2 fa fa-i-cursor"></i> Выделение
    Сделать текст в области текста окна перевода доступным для выбора. После активации возможности выбора текста, перетаскивание в тексте будет невозможно, можно только перетаскивать панель инструментов (поскольку при перетаскивании происходит выбор текста)

1. #### <i class="fa fa-search"></i> <i class="fa fa-icon fa-rotate-right"></i> Поиск слова
    Открыть окно поиска слов.