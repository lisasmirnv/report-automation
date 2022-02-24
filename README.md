# Боты для автоматизации отчетности

Бот **bot_logic.py** расчитывает метрики ленты новостей за вчера:
* DAU.
* Лайки.
* Просмотры.
* CTR.

Бот **bot_2_logic.py** расчитывает метрики ленты новостей и мессенджера за прошлую неделю: 
* DAU отдельно для ленты новостей и мессенджера, а также совместных пользователей.
* Действия пользователей и их усредненное количество на пользователя:
  * Лайки.
  * Просмотры.
  * Сообщения.

Бот **bot_anomalies_checker.py** с периодичностью 15 минут отслеживает аномальное поведение метрик:
* Активные пользователи.
* Лайки.
* Просмотры.
* Сообщения.
* CTR.

При каждом расчете бот запрашивает актуальные данные из БД (**CH.py**). 
