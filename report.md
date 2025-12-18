# Web Application Pentest Report – Roles and Permissions Issues

## Overview
Ten raport opisuje problemy bezpieczeństwa związane z nieprawidłową obsługą ról użytkowników i uprawnień w aplikacji webowej.

## Scope
Zakres testów obejmował:
- dostęp użytkowników do funkcji administracyjnych
- weryfikację ról użytkowników przy wykonywaniu akcji
- możliwość zmiany ról oraz uprawnień użytkowników

## Identified Issues
Aplikacja nie weryfikuje ról użytkowników przy każdej akcji, co może umożliwiać zwykłym użytkownikom dostęp do funkcji administracyjnych, w tym modyfikowanie danych, zarządzanie innymi użytkownikami oraz zmianę własnych uprawnień.

## Impact
Nieprawidłowa kontrola ról może prowadzić do eskalacji uprawnień, utraty kontroli nad aplikacją oraz nieautoryzowanego dostępu do danych i funkcji administracyjnych, co stanowi istotne ryzyko dla bezpieczeństwa systemu i użytkowników.

## Recommendations
Aplikacja powinna każdorazowo weryfikować role i uprawnienia użytkownika po stronie serwera przed wykonaniem każdej wrażliwej operacji. Funkcje administracyjne oraz zmiana ról powinny być dostępne wyłącznie dla uprawnionych użytkowników.
