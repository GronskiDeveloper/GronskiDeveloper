# Cześć, jestem Dominik 👋

Buduję **custom 3D product configurators** dla producentów, plus strony, sklepy i aplikacje na zamówienie pod marką **[GroDev](https://grodev.pl)**. Klient konfiguruje produkt robiony na wymiar, widzi go w 3D w przeglądarce i dostaje cenę liczoną na serwerze, nie zgadywaną w JavaScripcie.

**Dowód, nie deklaracje:** wdrożony portal B2B dla [Ustawnik.pl](https://ustawnik.pl) (Aravix s.c., Poznań), ocena **5,0 na [Clutch](https://clutch.co/profile/grodev)** w E-Commerce Development, a strony konfiguratorów grodev.pl są dziś najczęściej cytowaną polską domeną w odpowiedziach AI na „konfigurator produktu 3D”. Od niedawna także po angielsku, niemiecku i niderlandzku, pod rynki DACH i Benelux.

## Open source: fragmenty stacku, którego używam w komercyjnych wdrożeniach

Bierz i używaj. Każde repo to jeden plik albo czysty starter, bez build stepu tam, gdzie się da, z `CLAUDE.md` pokazującym podział pracy człowiek/AI.

| Repo | Co to | Live |
|---|---|---|
| **[threejs-configurator-server-side-pricing](https://github.com/GronskiDeveloper/threejs-configurator-server-side-pricing)** | Konfigurator 3D, w którym cena liczy się na serwerze, nie w przeglądarce. Ten jeden błąd architektury widuję najczęściej. | [demo](https://gronskideveloper.github.io/threejs-configurator-server-side-pricing/) |
| **[threejs-parametric-geometry](https://github.com/GronskiDeveloper/threejs-parametric-geometry)** | Cały produkt budowany z wymiarów. Jeden model, każdy rozmiar, bez modelowania wariantów ręcznie. | [demo](https://gronskideveloper.github.io/threejs-parametric-geometry/) |
| **[threejs-configurator-ar-preview](https://github.com/GronskiDeveloper/threejs-configurator-ar-preview)** | WebXR: skonfiguruj produkt i postaw go na własnej podłodze przez kamerę telefonu, bez instalowania aplikacji. | [demo](https://gronskideveloper.github.io/threejs-configurator-ar-preview/) |
| **[blender-to-glb-pipeline](https://github.com/GronskiDeveloper/blender-to-glb-pipeline)** | Jak wyciągnąć czysty `.glb` z Blendera/CAD na web, plus bezzależnościowy checker, który łapie typowe błędy. | checker CLI |
| **[claude-chat-react](https://github.com/GronskiDeveloper/claude-chat-react)** | Reactowy chatbot na Claude API, komponent + hook, ~8 KB. **Na npm:** `@grodev/claude-chat-react`. | [npm](https://www.npmjs.com/package/@grodev/claude-chat-react) |
| **[threejs-product-configurator-starter](https://github.com/GronskiDeveloper/threejs-product-configurator-starter)** | Minimalny konfigurator produktu 3D: geometria parametryczna, wykończenia, wycena na żywo. | [demo](https://gronskideveloper.github.io/threejs-product-configurator-starter/) |

Więcej: `claude-chat-widget` (proxy PHP), `booking-slots-php`, `woocommerce-custom-product-data`, `booking-ai-demo` (fuzja trzech repo w działający produkt).

## Jak pracuję: AI-first, ale autorstwo widoczne

Buduję z **Claude Code (Anthropic)** jako codziennym narzędziem, nie jako gadżetem. Każde publiczne repo ma `CLAUDE.md` z dosłowną tabelą „co zrobił człowiek, co zrobiła AI”, listą rzeczy, które **odrzuciłem** z draftu AI, i notatkami z weryfikacji (lint, testy w przeglądarce, uruchomienie skryptu na prawdziwych danych). Autorytet decyzyjny, czyli architektura, threat model, walidacja i co **odrzucić**, zostaje po stronie człowieka. Pełny opus: [How I document my AI-first workflow in every public repo](https://dev.to/gronskideveloper/how-i-document-my-ai-first-workflow-in-every-public-repo-4l0h).

## Konfiguratory 3D: dziesięć działających demonstratorów

Każdy to konfigurator otwierany w przeglądarce bez rejestracji, gotowy pod katalog i branding konkretnej firmy. Pełna lista z podglądami: **[grodev.pl/demo](https://grodev.pl/demo/)**. Dwa, które pokazują skalę:

- 🎪 **[modularstudio.grodev.pl](https://modularstudio.grodev.pl)** stoiska targowe: mapa hali z 65 parcelami, rezerwacja na zegar, portal wystawcy, konsola organizatora.
- 🏭 **[factory3d.grodev.pl](https://factory3d.grodev.pl)** cela produkcyjna: walidacja kolizji i stref bezpieczeństwa, symulacja wydajności, zestawienie materiałowe (BOM) z wyceną.

## Stack

Laravel · PHP · Three.js (WebGL, WebXR) · React · Next.js · TypeScript · WooCommerce · Python · Claude API

## Kontakt

Konfigurator, sklep albo aplikacja na zamówienie: **dominik.gronski@grodev.pl** · [grodev.pl](https://grodev.pl)
