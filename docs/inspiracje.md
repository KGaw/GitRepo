# Inspiracje i źródła do stworzenia programu zarządzającego listą studentów i ocen

## 1. Dokumentacja frameworków / bibliotek
- **Django (Python):** [https://docs.djangoproject.com/](https://docs.djangoproject.com/)
- **Flask (Python):** [https://flask.palletsprojects.com/](https://flask.palletsprojects.com/)
- **Spring Boot (Java):** [https://spring.io/projects/spring-boot](https://spring.io/projects/spring-boot)
- **ASP.NET Core (C#):** [https://docs.microsoft.com/aspnet/core/](https://docs.microsoft.com/aspnet/core/)

## 2. Bazy danych i ORM
- **PostgreSQL:** [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)
- **SQLite:** [https://www.sqlite.org/docs.html](https://www.sqlite.org/docs.html)
- **SQLAlchemy (Python ORM):** [https://docs.sqlalchemy.org/](https://docs.sqlalchemy.org/)
- **Hibernate (Java):** [https://hibernate.org/orm/documentation/](https://hibernate.org/orm/documentation/)

## 3. Przykładowe projekty i repozytoria na GitHub
- Szukaj fraz: `"student management"`, `"gradebook"`
- Wzorce CRUD, autoryzacja, import/eksport CSV/Excel, API REST

## 4. UI/UX i front-end
- **Bootstrap:** [https://getbootstrap.com/](https://getbootstrap.com/)
- **React:** [https://reactjs.org/docs/getting-started.html](https://reactjs.org/docs/getting-started.html)
- **Vue.js:** [https://vuejs.org/guide/introduction.html](https://vuejs.org/guide/introduction.html)
- Przykłady tabel, formularzy i walidacji: DataTables, AG Grid

## 5. Autentykacja i uprawnienia
- **OAuth2 / OpenID Connect**
- Biblioteki: Django Allauth, Spring Security, ASP.NET Identity
- Role: `admin`, `wykładowca`, `student`

## 6. Import/eksport danych
- Format CSV, XLSX: `pandas` (Python), `Apache POI` (Java), `EPPlus` (C#)
- API do integracji z systemami uczelnianymi (jeśli dotyczy)

## 7. Testowanie
- Testy jednostkowe i integracyjne: `pytest`, `JUnit`, `xUnit`
- Testy API: Postman, REST-assured

## 8. Wzorce projektowe
- MVC, Repository, Service Layer, DTO
- Walidacja po stronie serwera i klienta

## 9. Prywatność i bezpieczeństwo
- RODO/GDPR: minimalizacja danych, szyfrowanie, dostęp na podstawie ról
- Bezpieczne przechowywanie haseł (`bcrypt`)
- Ochrona przed CSRF, SQLi, XSS

## 10. Kursy i artykuły
- Kursy CRUD + autoryzacja (platformy: Udemy, Coursera, freeCodeCamp)
- Blogi techniczne pokazujące budowę prostego systemu ocen

## 11. Dane testowe
- Generatory fikcyjnych danych: Faker
- Przykładowe CSV z listą studentów i ocen do importu

## 12. Funkcjonalności do rozważenia
- CRUD studentów i kursów
- Przypisywanie ocen
- Historia ocen
- Raporty PDF/CSV
- Filtrowanie i sortowanie
- Powiadomienia email
