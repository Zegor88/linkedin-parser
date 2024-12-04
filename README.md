# LinkedIn Profile Scraper

## Описание
Скрипт автоматически извлекает данные из профилей LinkedIn с помощью Selenium и BeautifulSoup. Он авторизуется через учетные данные из переменных окружения, переходит на указанный профиль и собирает информацию.

## Сбор данных профиля:
   - Имя и заголовок.
   - Раздел "Обо мне" (About).
   - Опыт работы (Experience): название компании, должность, периоды работы, описание обязанностей и навыки.
   - Образование (Education): университеты, полученные степени, даты обучения и сертификаты.
   - Сертификаты (Licenses & Certifications): название, издатель, дата выдачи, Credential ID.
   - Активность пользователя (Posts): посты, их содержание, количество реакций и комментариев.

## Установка и запуск
1. Установите зависимости:
   ```bash
   pip install selenium beautifulsoup4 python-dotenv
   ```

2. Убедитесь, что у вас установлен веб-драйвер (например, ChromeDriver), совместимый с вашей версией браузера.

3. Создайте файл `.env` в корневой папке проекта и добавьте свои учетные данные LinkedIn:
   ```env
   LINKEDIN_EMAIL=your_email@example.com
   LINKEDIN_PASSWORD=your_password
   ```

4. Запустите скрипт:
   ```bash
   python linkedin_scraper.py
   ```

## Важные замечания
- **Этические аспекты:** Убедитесь, что использование скрипта соответствует политике LinkedIn.
- **Скорость запросов:** Чтобы избежать блокировок со стороны LinkedIn, добавлены задержки (time.sleep) между действиями.
- **Обновление структуры:** LinkedIn может изменять структуру своих страниц, поэтому XPath и классы элементов могут потребовать обновления.

## Авторы
Скрипт основан на примерах из репозиториев [LinkedIn-Profile-Scrapper-in-Python](https://github.com/laxmimerit/LinkedIn-Profile-Scrapper-in-Python) и [WebScraping_Linkedin](https://github.com/MariyaSha/WebScraping_Linkedin), с доработками и дополнениями.

