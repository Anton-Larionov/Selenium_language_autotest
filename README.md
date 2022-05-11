# Selenium_language_autotest
Solution for autotest language

<h1>Задание: запуск автотестов для разных языков интерфейса</h1>

Мы хотим, чтобы разрабатываемый нами интернет-магазин работал одинаково хорошо для пользователей из любой страны. Чтобы убедиться в работоспособности решения с поддержкой разных языков, мы планируем запускать набор автотестов для каждого языка. Вам как разработчику автотестов нужно реализовать решение, которое позволит запускать автотесты для разных языков пользователей, передавая нужный язык в командной строке.

<ol>
    <li>Создайте GitHub-репозиторий, в котором будут лежать файлы conftest.py и test_items.py.</li>
    <li>Добавьте в файл conftest.py обработчик, который считывает из командной строки параметр language.</li>
    <li>Реализуйте в файле conftest.py логику запуска браузера с указанным языком пользователя. Браузер должен объявляться в фикстуре browser и передаваться в тест как параметр.</li>
    <li>В файл test_items.py напишите тест, который проверяет, что страница товара на сайте содержит кнопку добавления в корзину. Например, можно проверять товар, доступный по http://selenium1py.pythonanywhere.com/catalogue/coders-at-work_207/.</li>
    <li>Тест должен запускаться с параметром language следующей командой:<br>
<code class="language-bash hljs">pytest --language=es test_items.py</code><br>
и проходить успешно. Достаточно, чтобы код работал только для браузера Сhrome.</li>
<li>Отправить ссылку на данный репозиторий в качестве ответа на данное задание.</li>
<li>Отправить решение на рецензирование другим учащимся. Не забудьте, что решение на рецензирование можно отправить только один раз.
Проверьте решения минимум трех других учащихся, чтобы получить баллы за задание.</li></ol>
Это задание с peer-review, поэтому кроме формальных критериев другие учащиеся могут проверять корректность написания вашего кода. 

Важно! Если при рецензировании чужого решения вы получаете ошибку вроде: 

raise ValueError("option names %s already added" % conflict)

ValueError: option names {'--language'} already added
Перепроверьте, что у вас нет своего conftest.py в директории выше, смотри шаг 4.</ol>
