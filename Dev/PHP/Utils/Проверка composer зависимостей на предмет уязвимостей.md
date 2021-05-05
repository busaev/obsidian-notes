Возможно, вы уже знаете об этом, но я все равно напишу:

Проверять свои composer зависимости на предмет известных уязвимостей можно просто добавив в dev зависимости пакет:

composer require --dev roave/security-advisories:dev-latest


Это простой metapackage, в котором в директиве conflict описаны известные версии библиотек с уязвимостями. Т.е. при попытке установить пакет с уязвимостью вы получите ошибку на уровне composer require.

Ссылка на github: https://github.com/Roave/SecurityAdvisories

#composer #security