# LenteApp [RU]

Данный репозиторий содержит код и данные мастерской №7 "Большие данные", ЛШЮП 2018.

## Участники
* Бояршин Андрей - подмастерье - LenteApp.LibraryBase, отдельные части остальных проектов
* Вандакуров Артём - LenteApp.CUI.Artyom, LenteApp.Impl.Artyom, LenteApp.UI.Desktop
* Лаптев Сергей - LenteApp.CUI.Sergey, LenteApp.Impl.Sergey, LenteApp.UI.Web
* Юриков Никита - LenteApp.CUI.Nikita, LenteApp.Impl.Nikita
* Алексеев Фёдор и Полушин Денис - решали иные задачи

## Сборка
Несмотря на изначальную работу с NuGet пакетами и feed'ами в качестве основного инструмента CI/CD, в данном репозитории все проекты сведены в один Solution. Связи между проектами основаны на ProjectReference.

Для сборки достаточно .NET Core SDK версии 2.1.x, процесс разработки не имеет особенностей. Для справки ознакомьтесь с документацией по стандартным командам dotnet CLI.

## Trivia
* Репозиторий содержит 3 схожих словаря (каждый около 100 МБ), сгенерированных на основе словаря Зализняка. Программы генерации не сохранились.
* Ожидается запуск в данной директории (корень репозитория) как текущей рабочей директории всех проектов, кроме проекта LenteApp.UI.Web. В силу особенностей работы ASP.NET Core его требуется запускать в директории проекта, то есть на один уровень ниже всех остальных.
* Не все комбинации *движок*-*интерфейс* были оттестированы. Наиболее универсальным и проверенным является интерфейс LenteApp.UI.Desktop.

# LenteApp [EN]

This repository contains the code and data of the 7th workshop ("BigData"), SSYP 2018.

## Building
Despite the initial use of NuGet packages and feeds as the main instrument of CI/CD, this repo contains a single Solution for all projects, inter-linked by ProjectReference.

Build requirements are very modest: only .NET Core SDK 2.1.x branch is required, the development process does not require any special workarounds, so use dotnet CLI Help for reference.

## Trivia
* Repository contains 3 simpilar dictionaries (each is around 100 MiB in size), autogenerated from Zaliznyak's Russian dictionary. The autogen source code is missing.
* Current working directory is repository root for all projects but one. LenteApp.UI.Web must be launched from the project's root due to some ASP.NET Core quirks.
* Not all *engine*-*UI* combinations were tested. The most profound UI is LenteApp.UI.Desktop, tested to work against all backend implementations.

