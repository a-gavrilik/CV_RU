# **Определение "узких" мест воронки продаж**

### Инструменты:
Python 
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scipy

### Описание задачи:
**some_site.com** - интерфейс (фронтенд) для выполнения ставок на спорт на протоколе Azuro. Основная задача фронтенда - дать лучший игровой опыт, чтобы игрокам было приятно, интересно и безопасно играть.

**Опыт складывается из:**
- набора событий на которые можно поставить;
- удобство интерфейса, возможность с минимальной когнитивной нагрузкой выбрать событие, исход, и сделать ставку;
- простота онбординга - понять что такое крипта, приобрести ее, подключиться к сервису, сделать ставку.

**Задача:**

Необходимо выдвинуть и подтвердить анализом гипотезу по улучшению игрового опыта в https://some_site.com/.

Для подтверждения гипотезы предлагается использовать датасет из трех событий:
- page load: загрузка страницы сайта
- balance update: подключение крипто-кошелька (логин) на сайте
- bet place: успешное совершение ставки

Три события представляет собой воронку:
1. пользователь приходит на сайт
2. подключает кошелек (если он у него есть)
3. совершает ставку (если он находит интересное событие)

Описание особых полей набора данных:
- WALLET_INJECTED_INSTALLED: признак наличия web3.js библиотеки, свидетельствует о том, что страница открыта в хроме с установленным виджетом ИЛИ страница открыта в браузере мобильного приложения кошелька
- WALLET_TYPE - способ подключения к кошельку. Injected - web3.js API, WalletConnect - использование WalletConnect API.


