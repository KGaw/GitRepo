```mermaid
flowchart TD
    A[Start] --> B{Czy istnieje zapis bazy?}
    B -- Tak --> C[Wczytaj DB]
    B -- Nie --> D[Utwórz pustą DB]
    B -- Błąd --> E[Pokaż błąd i utwórz pustą DB]

    C --> F[Główne menu]
    D --> F
    E --> F

    F --> G1[Dodaj studenta]
    F --> G2[Dodaj ocenę]
    F --> G3[Edytuj studenta]
    F --> G4[Usuń studenta]
    F --> G5[Wyświetl studenta / listę]
    F --> G6[Oblicz średnie / raporty]
    F --> G7[Zapisz / Eksportuj]
    F --> G8[Wczytaj / Importuj]
    F --> G9[Wyjście]

    G1 --> H1[Wprowadź dane]
    G2 --> H2[Wprowadź dane]
    G3 --> H3[Weryfikuj istnienie studenta]
    G4 --> H4[Weryfikuj istnienie studenta]
    G5 --> H5[Wykonaj akcję]
    G6 --> H6[Oblicz średnie / generuj raporty]
    G7 --> H7[Zapisz dane]
    G8 --> H8[Wczytaj dane]
    G9 --> H9[Pytaj o zapis przed zamknięciem]

    H1 --> I1[Walidacja wejścia]
    H2 --> I2[Walidacja wejścia]
    H3 --> I3[Aktualizuj DB]
    H4 --> I4[Aktualizuj DB]
    H5 --> I5[Potwierdzenie]
    H6 --> I6[Potwierdzenie]
    H7 --> I7[Potwierdzenie]
    H8 --> I8[Potwierdzenie]
    H9 --> I9[Wyjście]

    I1 --> I3
    I2 --> I3
    I3 --> I5
    I4 --> I5
    I5 --> F
    I6 --> F
    I7 --> F
    I8 --> F
    I9 --> J[Koniec]

    %% Legenda
    classDef legenda fill:#f9f,stroke:#333,stroke-width:1px;
    subgraph LEGEND [Legenda]
        L1["DB = baza studentów (id, imię, nazwisko, przedmioty, oceny)"]
        L2["Walidacja: unikalność id, zakres ocen, wymagane pola"]
        L3["Oblicz średnie: per student, per przedmiot, raporty klasowe"]
        L4["Zapis/Wczyt: CSV/JSON, plik lokalny lub DB"]
    end
    class LEGEND legenda

