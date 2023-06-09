# SHA-1 (Secure Hash Algorithm 1)

SHA-1 (Secure Hash Algorithm 1) є криптографічною функцією хешування, яка використовується для створення унікального хеш-коду фіксованої довжини 160 бітів з будь-якого вхідного повідомлення. Ось детальний опис ідеї і підходів алгоритму SHA-1:

1. **Підготовка повідомлення**: Вхідне повідомлення розбивається на блоки фіксованої довжини і доповнюється до встановленої довжини, якщо необхідно. Зазвичай використовується доповнення за схемою "length-1-bit-0-length".


3. **Обробка блоків повідомлення**: Кожен блок повідомлення проходить через ітераційний процес, який включає кілька кроків.

   a. **Поділ блока на слова**: Блок повідомлення розбивається на 32-бітові слова.

   b. **Розширення**: Для кожного слова блока повідомлення формується 80 32-бітових словесних розширень за певною логічною схемою.

   c. **Ініціалізація змінних**: Ініціалізуються певні змінні, які будуть використовуватись для обчислення кінцевого хеш-значення.

   d. **Раундові операції**: Виконуються 80 раундових операцій, в яких змінні перебувають у взаємодії зі словами блока повідомлення та константами.

   e. **Оновлення хеш-значення**: Після кожного раунда змінні оновлюються залежно від результатів раундових операцій.

4. **Формування кінцевого хеш-значення**: Після обробки всіх блоків повідомлення, кінцеве хеш-значення формується шляхом конкатенації значень змінних, що представляють частини хеш-коду.

Алгоритм SHA-1 використовує різні логічні та бітові операції, такі як побітові зсуви, логічні кон'юнкції та диз'юнкції, кругові бітові зсуви та інверсії. Ці операції дозволяють забезпечити добре розподілення бітів та нелінійність у процесі генерації хеш-коду.
