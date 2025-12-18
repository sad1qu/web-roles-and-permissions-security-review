# Web Application Pentest Report – Roles and Permissions Security Review

## Overview
Ten raport opisuje problemy bezpieczeństwa związane z obsługą ról użytkowników, uprawnień oraz dostępem do funkcji administracyjnych w aplikacji webowej.

## Scope
Zakres testów obejmował dostęp do funkcji administracyjnych oraz weryfikację roli użytkownika przy wykonywaniu wrażliwych akcji.

## Identified Issues
Aplikacja nie weryfikuje roli użytkownika przy każdej wykonywanej akcji, co umożliwia dostęp do funkcji administracyjnych użytkownikom bez odpowiednich uprawnień.

## Impact
Brak prawidłowej weryfikacji ról może prowadzić do eskalacji uprawnień, nieautoryzowanych zmian w aplikacji oraz utraty kontroli nad danymi i funkcjami systemu, co stanowi istotne ryzyko dla bezpieczeństwa użytkowników i organizacji.

## Recommendations
Aplikacja powinna każdorazowo weryfikować rolę użytkownika po stronie serwera przed wykonaniem każdej wrażliwej akcji, zamiast polegać wyłącznie na ograniczeniach w interfejsie użytkownika, które mogą zostać łatwo pominięte.
