# Dashboard
- '/'
    -statystyki dzisiejszych zamówień(zdalne i lokalne)
    -listę rezerwacji i eventów zaplanowanych na dzisiaj
# Logowanie

- '/login'
    -pola na login i hasło
    -guzik do zalogowania(link do dashboardu)

# Widok dostępności stolików

- '/tables'
    -wybór daty i godziny
    - tabelaz listą rezerwacji oraz wydarzeń
        - każda kolumna = 1 stolik
        - każdy wiersz = 30 minut
        - ma przypominać widok tygodnia w kalendarzu Google, gdzie w kolumnach zamiast dni są różne stoliki
        - po kliknięciu rezerwacji lub eventu przechodzimy na stronę szczegółów
- '/tables/booking/:id'
    - zawiera wszystkie informacje dotyczące rezerwacji
    - umożliwia edycję i zapisanie zmian
- '/tables/booking/new'
    - analogicznie do powyższej, bez początkowych informacji
- '/tables/events/:id'
    - analogicznie do powyższej, dla eventów
- '/tables/events/new'
    - analogicznie do powyższej, dla eventów bez początkowych informacji

# Widok Kelnera

-'/waiter'
    - Tabela
        - w wierszach stoliki
        - w kolumnach różne rodzaje inforamcji (status, czas od ostatniej aktywności)
        - w ostatniej kolumnie dostępne akcje dla danego stolika
-'/waiter/order/new'
    - numer stolika (edytowalny)
    - menu produktów
    - opcje wybranego produktu
    - zamówienie (zamówione produkty z opcjami i ceną)
    - kwota zamówienia
-'/waiter/order/:id'
    -jak powyższa

# Widok Kuchni

-'/kitchen'
    - wyświetla listę zamówień w kolejności ich złożenia
    - lista musi zawierać
        - numer stolika (lub zamówienia zdalnego)
        - pełne informacje dotyczące zamówionych dań
    - na liście musi być możliwość oznaczenia zamówienia jako zreazlizowane
