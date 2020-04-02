### Использование:
0. [Optional] Устанавливаем/Обновляем шаблоны если они изменились `generamba template install`
1. Создаем сцену с помощью команды `generamba gen [MODULE_NAME] swifty_reactor`

Для установки Generamba `gem install generamba`

### Настройка проекта:
Пользуемся стандратным настройщиком [`generamba setup`](https://github.com/rambler-digital-solutions/Generamba/wiki/Available-Commands#basic-generamba-configuration)
Либо используем готовую настройку:
1. Создаем файл с именем `Rambafile`
2. Копируем туда заменив `ModuleName` на название своего проекта
```
### Headers settings
company: BCS
### Xcode project settings
project_name: ModuleName
xcodeproj_path: ModuleName.xcodeproj
### Code generation settings section
# The main project target name
project_target: ModuleName
### Dependencies settings section
podfile_path: Podfile
# The file path for new modules
# Path где будет лежать сгенерированый модуль
project_file_path: ModuleName/Scenes
# The Xcode group path to new modules
project_group_path: ModuleName/Scenes
### Templates
catalogs:
- 'https://github.com/BCS-Broker/GenerambaTemplates'
templates:
- { name: swifty_reactor}
```
3. Устанавливаем шаблоны `generamba template install`
4. Создаем сцену с помощью команды `generamba gen [MODULE_NAME] swifty_reactor`

