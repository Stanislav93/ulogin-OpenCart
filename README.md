# uLogin

Donate link: http://ulogin.ru  
Tags: ulogin, login, social, authorization  
Tested up to: 2.1.0.1  
Stable tag: 2.0.1  
License: GNU General Public License, version 2  

**uLogin** — это инструмент, который позволяет пользователям получить единый доступ к различным Интернет-сервисам без необходимости повторной регистрации,
а владельцам сайтов — получить дополнительный приток клиентов из социальных сетей и популярных порталов (Google, Яндекс, Mail.ru, ВКонтакте, Facebook и др.)


## Установка

Скачайте архив *ulogin-2.\*.ocmod.zip*.  

- На странице "Установка расширений"/"Extension Installer" раздела "Модули"/"Extensions" загрузите данный архив.  
- При успешной установке должны загрузиться модификатор ("uLogin - authorisation") и два модуля ("uLogin - панель", "uLogin - общие настройки").  
- Убедитесь, что данные модули и модификатор добавлены в списки модулей и модификаторов на соответствующих страницах. Активируйте их.  
- На странице "Модификаторы" обновите данные (кнопка "Обновить"/"Refresh" в верхнем правом углу экрана).  

Для данного способа установки должна быть выполнена предварительная настройка ftp.  

#### Альтернативная установка:

- Распакуйте содержимое папки **upload** архива установки в корень сайта.  
- Убедитесь, что данные модули ("uLogin - панель", "uLogin - общие настройки") добавлены в списки модулей. Активируйте их.  
- Распакуйте файл **install.xml** архива установки, установите его на странице "Установка расширений"/"Extension Installer" способом описанным выше.  
- Убедитесь, что на странице "Модификаторы" добавился модификатор "uLogin - authorisation" и что он включен.  
- На этой же странице обновите данные.  


При активации(установке) модуля *"uLogin - панель"* автоматически создаются дочерние модули и добавляются в макет *Account*.  
При активации(установке) модуля *"uLogin - общие настройки"* создаётся группа клиентов *uLogin* для новых, регистрирующихся через uLogin клиентов.  


## Модуль "uLogin - общие настройки"

В данном модуле задаётся **Значение поля uLogin ID** - общее поле для всех виджетов uLogin, необязательный параметр (см. *"Настройки виджета uLogin"*).  
Также здесь задается группа, присваиваемая клиентам, зарегистрированных с помощью uLogin. По умолчанию - группа *uLogin* - создаётся при активации(установке) модуля.


## Модуль "uLogin - панель"

Здесь Вы можете указывать параметры для каждой панели uLogin отдельно.

Параметр модуля **Значение поля uLogin ID** - задаёт значение для виджета данной панели. Пустое поле - значение берётся из модуля "uLogin - общие настройки". 
Параметр **Тип формы** - влияет на отображение панели uLogin: 

- *Форма offline - авторизация* - форма для авторизации, отображается, когда пользователь онлайн. Место расположения определяется в макетах.
- *Форма online - синхронизация* - форма для связывания аккаунтов различных соцсетей, отображается, когда пользователь офлайн. Место расположения определяется в макетах.
- *Форма online - синхронизация в личном кабинете пользователя* - то же, что и *Форма online - синхронизация*, 
за исключением того, что форма будет отображаться только в личном кабинете пользователя на странице редактирования данных только при добавлении модуля в макет *Account*.

При активации(установке) модуля *"uLogin - панель"* автоматически создаются два дочерних модуля и добавляются в макет *Account*.


## Настройки виджета uLogin

При установке расширения uLogin авторизация пользователей будет осуществляться с настройками по умолчанию.  
Для более детальной настройки виджетов uLogin Вы можете воспользоваться сервисом uLogin.  

Вы можете создать свой виджет uLogin и редактировать его самостоятельно:

для создания виджета необходимо зайти в Личный Кабинет (ЛК) на сайте http://ulogin.ru/lk.php,
добавить свой сайт к списку Мои сайты и на вкладке Виджеты добавить новый виджет. После этого вы можете отредактировать свой виджет.

**Важно!** Для успешной работы плагина необходимо включить в обязательных полях профиля поле **Еmail** в Личном кабинете uLogin.  
Заполнять поля в графе «Тип авторизации» не нужно, т.к. расширение uLogin настроено на автоматическое заполнение данных параметров.

Созданный в Личном Кабинете виджет имеет параметр **uLogin ID**.  
Скопируйте значение **uLogin ID** вашего виджета в соответствующее поле в настройках плагина на вашем сайте и сохраните настройки.   

Если всё было сделано правильно, виджет изменится согласно вашим настройкам.

