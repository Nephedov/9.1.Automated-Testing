[![Build status](https://ci.appveyor.com/api/projects/status/h0oln30eed1yylr0?svg=true)](https://ci.appveyor.com/project/Nephedov/cardorderallure)

# Домашнее задание к занятию «4.1. Репортинг»

## Решения
* Задание 1
  * <a href="https://github.com/Nephedov/9.1.Automated-Testing/blob/6a878f38fe5fa186ac46255d83da71ebb03cddcb/src/test/java/netology/CardOrderDeliveryChangeDateTest.java">CardOrderDeliveryChangeDateTest.java</a> - класс с автотестами.

<a href="https://github.com/Nephedov/9.1.Automated-Testing/tree/main">Репозиторий</a> c Allure проектом.
* Задание 2
  * <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/README.md">README.md</a>. - Шаги вопроизведения подключения ReportPortal к проекту.
  * <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/src/test/java/netology/test/CardOrderDeliveryChangeDateTest.java">CardOrderDeliveryChangeDateTest.java</a>. - класс с автотестами.

<a href="https://github.com/Nephedov/9.2.Automated-Testing/tree/main">Репозиторий</a> с ReportPortal проектом.

## Что было сделано
* Задание 1
  * Настроен <a href="https://github.com/Nephedov/9.1.Automated-Testing/blob/6a878f38fe5fa186ac46255d83da71ebb03cddcb/build.gradle">build.gradle</a> с зависимостями:
    * JunitJupier.
    * Lombok.
    * Allure.
    * Selenide.
    * Faker.
  * Подключен к проекту AppVeyor. Настроен <a href="https://github.com/Nephedov/9.1.Automated-Testing/blob/6a878f38fe5fa186ac46255d83da71ebb03cddcb/.appveyor.yml">appveyor.yml</a>. Добавлен бейдж в README.md, о статусе сборки при пуше.
  * Реализован класс с <a href="https://github.com/Nephedov/9.1.Automated-Testing/blob/6a878f38fe5fa186ac46255d83da71ebb03cddcb/src/test/java/netology/CardOrderDeliveryChangeDateTest.java">автотестами</a>, с Allure-Selenide.
  * Реализован класс-генератор тестовых данных - <a href="https://github.com/Nephedov/9.1.Automated-Testing/blob/6a878f38fe5fa186ac46255d83da71ebb03cddcb/src/test/java/netology/DataGenerator.java">DataGenerator.java</a>.
* Задание 2
  * Настроен <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/build.gradle">build.gradle</a> с зависимостями:
    * JunitJupier.
    * Lombok.
    * Selenide.
    * Faker.
    * ReportPortal.
  * Подключен к проекту ReportPortal.
  * Реализован <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/docker-compose.yml">docker-compose.yml</a> - разворачивающий ReportPortal.
  * Реализованы классы логирования шагов - <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/src/test/java/netology/util/LoggingUtils.java">LoggingUtils.java</a> автотестов и скриншотов - <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/src/test/java/netology/util/ScreenShooterReportPortalExtension.java">ScreenShooterReportPortalExtension.java</a>.
  * Реализован класс-генератор тестовых данных - <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/src/test/java/netology/data/DataGenerator.java">DataGenerator.java</a>.
  * Реализован класс с <a href="https://github.com/Nephedov/9.2.Automated-Testing/blob/f10aaff5643206a7746056fbaed1992acfe6c6a4/src/test/java/netology/test/CardOrderDeliveryChangeDateTest.java">автотестами</a>.

## Задача №1: проснулись (Allure)

Вам нужно:   
* взять ваш проект и прикрутить туда Allure, интегрированный с Selenide 
* удостоверится, что при локальном запуске всё работает, отчёты генерируются, скриншоты прикрепляются, и вы можете их посмотреть через Allure 
* приложить в файл README репозитория скриншоты отчета Allure, изображения будет удобным вставить из буфера обмена в вебинтерфейсе Github в режиме редактирования файла README.md

## Задача №2: Report Portal (необязательная)

Что нужно сделать: попробовать интегрировать ваш проект тестирования доставки карт с Report Portal. Нам будет достаточно, если логи вашего теста будут отправляться в запущенный экземпляр Report Portal.

В результате: обновляете ваш проект на GitHub для интеграции с Report Portal и выкладываете краткий manual в виде README.md, в котором описываете необходимые действия для воспроизведения вашей интеграции.
