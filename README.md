# Использование clang-format в QtCreator

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/linux-code-2-e1620113254838.png)


### Использование clang-format в QtCreator для согласованного стиля кода в проекте C ++

Самый лучший на данный момент - это, вероятно, формат clang. Одна замечательная особенность заключается в том, что его конфигурация (стиль кода) может быть легко опубликована в репозитории кода. Все, что требуется, - это файл в формате .clang (или _clang-format), содержащий конфигурацию. Один пример конфигурации формата .clang, который очень хорошо соответствует стилю Qt (поскольку Qt может использовать его в обязательном порядке в будущем), можно найти здесь:  http://code.qt.io/cgit/qt/qt5.git/tree/_clang-format . Многие IDE и редакторы поддерживают этот инструмент. QtCreator тоже. Так что новым / всем участникам проекта легко соответствовать стилю кодирования. А вот краткое руководство о том, как настроить QtCreator для использования clang-формата:

Сначала вам нужно установить clang-format. Для Windows он включен в пакет clang  http://releases.llvm.org/download.html . В дистрибутивы Linux обычно уже включены пакеты. Пользователи MacOS могут, например, использовать brew для его установки.

Далее необходимо создать файл формата .clang в корневом каталоге вашего проекта. Параметры конфигурации можно найти здесь:  https://clang.llvm.org/docs/ClangFormatStyleOptions.html . Существует даже (очень медленный) инструмент для создания конфигурации из вашего существующего кода  https://github.com/johnmcfarlane/unformat .

В QtCreator подключаемый модуль beautifier должен быть включен в «Справка -> О модулях…» 

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_plugins.png)

В настройках QtCreator плагин beautifier должен использовать clang-format. И при желании включите автоматическое форматирование при сохранении (настоятельно рекомендуется).

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_beautifier.png)

Затем настройте clang-format для использования файла конфигурации. И при необходимости укажите путь к исполняемому файлу формата clang. 

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_clang-format.png)

При желании вы можете отформатировать код вручную с помощью сочетания клавиш. Поэтому необходимо установить ярлык.

![](https://www.vikingsoftware.com/wp-content/uploads/2021/03/QtC_shortcut.png)

В качестве файла настройки можно использовать готовый [файл](https://raw.githubusercontent.com/PickNikRobotics/roscpp_code_format/master/.clang-format "файл")