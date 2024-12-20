### Таблиця 1. Опис функціональних вимог

| №     | Опис                                                                                                                              | Пріоритет | Джерело (зацікавлена особа)                                               |
|-------|------------------------------------------------------------------------------------------------------------------------------------|-----------|-------------------------------------------------------|
| FR1   | Система надсилає сповіщення працівникам, керівнику ділянки та оператору крана у разі наближення до небезпечної зони або об’єкта. | Високий   | Працівник на майданчику, Керівник ділянки, Оператор крану |
| FR1.1 | Сповіщення на мобільний пристрій працівника із напрямком для виходу із зони ризику, якщо він наближається до небезпечної ділянки. | Високий   | Працівник на майданчику                               |
| FR1.2 | Сповіщення звуковим сигналом через шолом, якщо працівник знаходиться у радіусі небезпечної ділянки, аж до виходу з неї.          | Високий   | Працівник на майданчику                               |
| FR1.3 | Сповіщення керівнику ділянки у разі, якщо працівник не відповідає на попередження, або якщо виявлено критичний ризик.             | Високий   | Керівник ділянки                                      |
| FR1.4 | Сповіщення оператору крана про присутність людей у радіусі роботи крана; повторне інформування керівника при відсутності реакції. | Високий   | Оператор крану                                        |
| FR2   | Система автоматично блокує рух крана або підйомного обладнання при виявленні критичної загрози в зоні дії цього обладнання.            | Високий   | Оператор крана, Керівник ділянки |
| FR2.1 | Система зупиняє рух обладнання при виявленні працівників або об'єктів у радіусі небезпечної дії підйомного обладнання.                 | Високий   | Оператор крана                  |
| FR2.2 | Оператор отримує повідомлення з поясненням причини автоматичної зупинки обладнання та інструкцією для подальших дій.                   | Високий   | Оператор крана                  |
| FR2.3 | Керівник ділянки отримує сповіщення про автоматичне блокування обладнання та можливу причину загрози для контролю ситуації.            | Середній  | Керівник ділянки                |
| FR2.4 | Система розблоковує рух обладнання лише після підтвердження оператора або керівника, що загроза більше не актуальна.                  | Високий   | Оператор крана, Керівник ділянки |
| FR3   | Система створює щотижневий звіт про інциденти та загрози на майданчику для аналізу і ухвалення рішень.                        | Середній  | Керівник ділянки                |
| FR3.1 | Система автоматично збирає дані про всі зафіксовані інциденти та загрози на майданчику протягом тижня.                        | Високий   | Керівник ділянки                |
| FR3.2 | Система агрегує дані інцидентів і форматує їх у зрозумілий звіт із зазначенням часу, місця, типу загрози та можливих причин.  | Середній  | Керівник ділянки                |
| FR3.3 | Звіт генерується у зручному форматі і надсилається керівнику ділянки для подальшого аналізу.                  | Високий   | Керівник ділянки                |
| FR3.4 | Система зберігає звіти за попередні періоди (період вибирається користувачем), щоб забезпечити можливість доступу до даних при аналізі.             | Середній  | Керівник ділянки                |

