# Перечень автоматизируемых сценариев
## UI Тестирование

## Полные пути оплаты

### Позитивные сценарии

1. Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидными* значениями поля: Номер карты, месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД появляется.
2. Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидными* значениями поля: Номер карты, месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение о неудачной попытке оплаты. Запись в БД создается.

### Негативные сценарии

3. Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным* значением поле номер карты. Заполнить валидными* значениями поля: месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неудачной попытке оплаты. Запись в БД не создаётся.

## Поле «Номер карты»

### Позитивные сценарии

4. (Граничное значение - 16 символов) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить валидными значениями поля: месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создается.

### Негативные сценарии

5. (Граничное значение - 15 символов) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты (Заполняются только 15 символов из 16). Заполнить валидными значениями поля: месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создается.
6. (Граничное значение - 1 числовой символ) Открыть страницу покупки тура. Нажать на кнопку «Купить». В поле «Номер карты» вводится любое числовое значение от 0 до 9 . Заполнить валидными значениями поля: месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создается.
7. (Граничное значение - пустое поле) Открыть страницу покупки тура. Нажать на кнопку «Купить». Поле «Номер карты» не заполняется. Заполнить валидными значениями поля: месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
8. (Граничное значение - все символы - нули) Открыть страницу покупки тура. Нажать на кнопку «Купить». Все поле «Номер карты» заполняется нулями. Заполнить валидными значениями поля: месяц, год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.

**(Валидное значение для поля «Номер карты» - 16 числовых символов)**

## Поле «Месяц»

### Позитивные сценарии

9. (Граничное значение - 01) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «месяц» значением 01. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
10. (Граничное значение - 02) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «месяц» значением 02. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
11. (Граничное значение - 11) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «месяц» значением 11. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
12. (Граничное значение - 12) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «месяц» значением 12. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.

### Негативные сценарии

13. (Граничное значение - пустое поле) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Месяц» не заполняется. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
14. (Граничное значение - 00) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Месяц» заполняется значением - 00. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
15. (Граничное значение - 13) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Месяц» заполняется значением - 13. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
16. (Граничное значение - 1 числовой символ) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Месяц» заполняется любым числовым значением от 0 до 9. Заполнить валидными значениями поля: год, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.

**(Валидное значение для поля «Месяц» - двухзначное число (от 01 до 12))**

## Поле «Год»

### Позитивные сценарии

17. (Граничное значение - последние две цифры текущего года) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Год» двумя последними цифрами текущего года. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
18. (Граничное значение - последние две цифры следующего года, относительного текущего) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Год» последними двумя цифрами следующего года, относительного текущего. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
19. (Граничное значение - последние две цифры текущего года + 2) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Год» последними двумя цифрами текущего года + 2. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
20. (Граничное значение - последние две цифры текущего года + 7) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Год» последними двумя цифрами текущего года + 7. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
21. (Граничное значение - последние две цифры текущего года + 8) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Год» последними двумя цифрами текущего года + 8. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.

### Негативные сценарии

22. (Граничное значение - пустое поле) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Год» не заполняется. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
23. (Граничное значение - 1 символ) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Год» заполняется любым числовым значением от 0 до 9. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
24. (Граничное значение - последние две цифры текущего года - 1) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Год» заполняется последними двумя числами текущего года - 1. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
25. Граничное значение - последние две цифры текущего года + 9) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Год» заполняется последними двумя числами текущего года + 9. Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
26. (Граничное значение - 0000) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Ввести 0000 в поле «Год». Заполнить валидными значениями поля: месяц, владелец, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.

**(Валидное значение для поля «Год» - двухзначное число (последние 2 цифры текущего года + от 1 до 8(включительно))**

## Поле «Владелец»

### Позитивные сценарии

27. (Граничное значение - 3 буквенных символа) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» 3-мя валидными буквенными символами. Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
28. (Граничное значение - 4 буквенных символа) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» 4-мя валидными буквенными символами. Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
29. (Граничное значение - поле имя с пробелом) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» валидным именем с наличием пробела. Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
30. (Граничное значение - поле имя с дефисом) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» валидным именем с наличием дефиса. Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
31. (Граничное значение - 19 буквенных символов) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец»  валидными буквенными символами (19 символов). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.
32. (Граничное значение - 20 буквенных символа) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец»  валидными буквенными символами (20 символов). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.

### Негативные сценарии

33. (Граничное значение - 2 буквенных символа) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец»  валидными буквенными символами (2 символа). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
34. (Граничное значение - пустое поле) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Поле «Владелец» не заполняется. Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
35. (Эквивалентное значение - цифры) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» цифровыми значениями в допустимом диапазоне). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
36. (Эквивалентное значение - спецсимволы) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» спецсимволами в допустимом диапазоне). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
37. (Эквивалентное значение - пробелы) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» пробелами в допустимом диапазоне). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
38. (Эквивалентное значение - кириллица) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец» кириллицей в допустимом диапазоне). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
39. (Граничное значение - 21 буквенный символ) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить поле «Владелец»  валидными буквенными символами (21 символ). Заполнить валидными значениями поля: месяц, год, CVC/CVV. Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.

**(Валидное значение для поля «Владелец» - латинские буквы с использованием пробелов, дефисов, заглавных букв в количестве от 3 до 20 символов (включительно))**

## Поле «CVC/CVV»

### Позитивные сценарии

40. (Граничное значение - 3 символа) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить валидными значениями поля: владелец, месяц, год. Поле «CVC/CVV» заполнить 3-мя валидными символами.  Нажать на кнопку «Продолжить». Форма отправлена. Появляется сообщение об успешной оплате. Запись в БД создаётся.

### Негативные сценарии

41. (Граничное значение - 1 символ) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить валидными значениями поля: владелец, месяц, год. Поле «CVC/CVV» заполнить 1 символом.  Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
42. (Граничное значение - 2 символа) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить валидными значениями поля: владелец, месяц, год. Поле «CVC/CVV» заполнить 2-мя символами.  Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
43. (Граничное значение - пустое поле) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить валидными значениями поля: владелец, месяц, год. Поле «CVC/CVV» не заполняется.  Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.
44. (Граничное значение - 000) Открыть страницу покупки тура. Нажать на кнопку «Купить». Заполнить валидным значением поле номер карты. Заполнить валидными значениями поля: владелец, месяц, год. Ввести 000 в поле «CVC/CVV».  Нажать на кнопку «Продолжить». Форма не отправлена. Появляется сообщение о неправильном заполнении поля. Запись в БД не создаётся.

**(Валидное значение для поля «CVC/CVV» - трехзначное число)**


* Для тестирования пункта «Купить в кредит» следует повторить все тест-кейсы, приведенные выше.

# Перечень необходимых инструментов

1. IntelliJ IDEA - Среда для автотестов
2. Gradle - Система сборки кода
3. JUnit 5 - Тестовая среда
4. Selenide - Фреймворк для UI тестирования
5. REST Assured - Фреймворк для API тестирования
6. Docker - создание контейнера тестируемый БД
7. Allure Система репортинга
8. SQL Система для написания запросов к БД
9. Faker - Генерация данных
10. Github - инструмент контроля версий, а также хранения кода

# Перечень и описание возможных рисков при автоматизации

1. Большое количество тестов, необходимость их постоянной поддержки
2. Изменения некоторых элементов на странице, структуры и организации.
3. Изменения верстки страницы.

# Интервальная оценка с учётом рисков в часах

Работа включает: настройка тестового окружения(10 часов), написание автотестов (20 + часов), устранение ошибок(10 + часов), создание баг-рапортов(10 часов) , создание отчета о результатах (5 часов).

Общее время, необходимое для выполнения 70-80 часов

# План сдачи работ
Написание автотестов 05.10.2022
Результаты прогона 10.10.2022



