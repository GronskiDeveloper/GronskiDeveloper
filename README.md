# Cześć, jestem Dominik 👋

Full-stack developer z Poznania. Właściciel **[GroDev](https://grodev.pl)** — buduję strony, sklepy i aplikacje na zamówienie. Bez szablonów.

## Stack

Laravel · PHP 8.3 · MySQL · Three.js (WebGL) · Tailwind · WooCommerce · Python/Qt · Claude API

## AI-first workflow

Pracuję z **Claude Code (Anthropic)** jako codzienne narzędzie — nie jako gadżet. Każde publiczne repo poniżej zawiera:

- **`CLAUDE.md`** — dosłowna tabela „co zrobił człowiek, co zrobiła AI" dla każdej warstwy projektu, wraz z listą rzeczy, które **odrzuciłem** z draftu AI i dlaczego. Autorstwo widoczne, nie deklarowane.
- **Notatki weryfikacyjne** — konkretne kroki, którymi sprawdziłem output AI (lint, ręczne testy w przeglądarce, wywołania po instalacji), zapisane obok kodu.
- **Znane pułapki** (`Known gotchas`) — miejsca, gdzie następna iteracja AI zrobiłaby coś głupiego, i wprost napisane co „nie". Chroni to zarówno mnie, jak i model na kolejnym przebiegu.

Rozszerzone materiały:

- 📝 **[Full write-up on Dev.to → *How I document my AI-first workflow in every public repo*](https://dev.to/gronskideveloper/how-i-document-my-ai-first-workflow-in-every-public-repo-4l0h)** — dłuższy artykuł EN pokazujący cały wzorzec (CLAUDE.md + case study + agent commands) na przykładzie 5 działających repo.
- **[Case study — jak powstał `claude-chat-widget`](https://github.com/GronskiDeveloper/claude-chat-widget/blob/main/CASE_STUDY.md)** — pełna retrospektywa jednego repo, krok po kroku: threat model → wyciągnięcie dokładnego kształtu SDK (nie zgadywanie) → draft AI → audyt linia po linii → hardening → weryfikacja w prawdziwej przeglądarce → dokumentacja. Pokazuje realny podział pracy, nie ogólniki.
- **[Konfiguracja agenta — `.claude/commands/security-review.md`](https://github.com/GronskiDeveloper/claude-chat-widget/blob/main/.claude/commands/security-review.md)** — slash-command wymuszający listę 6 niezmienników bezpieczeństwa przed każdą zmianą w proxy. Przykład, jak automatyzuję powtarzalny code review przez konfigurację, nie przez dyscyplinę.

**Filozofia:** AI to szybki pisarz i rozsądny recenzent. Autorytet decyzyjny (architektura, threat model, walidacja, dobór zależności, co **odrzucić**) zostaje po stronie człowieka. Repo, w którym to się myli, sypie w produkcji — nawet jeśli `lint` przechodzi.

## Konfiguratory produktowe 3D

Prawdziwe wdrożenia dla polskich producentów, każdy 100% na zamówienie:

- 🏊 [basen3d.grodev.pl](https://basen3d.grodev.pl) — konfigurator basenów
- 🚪 [brama3d.grodev.pl](https://brama3d.grodev.pl) — bramy segmentowe
- 💡 [lampy3d.grodev.pl](https://lampy3d.grodev.pl) — lampy dekoracyjne
- 📦 [opakowania3d.grodev.pl](https://opakowania3d.grodev.pl) — opakowania kartonowe
- 🌿 [oranzeria3d.grodev.pl](https://oranzeria3d.grodev.pl) — oranżerie ogrodowe
- ☀️ [pergola3d.grodev.pl](https://pergola3d.grodev.pl) — pergole bioklimatyczne
- 🧖 [sauna3d.grodev.pl](https://sauna3d.grodev.pl) — sauny ogrodowe
- 🎪 [zadaszenie3d.grodev.pl](https://zadaszenie3d.grodev.pl) — zadaszenia tarasu
- 🎯 [kasetony3d.grodev.pl](https://kasetony3d.grodev.pl) — kasetony reklamowe

Wszystkie: **Three.js + PWA + eksport do PDF/email + integracja WooCommerce/CRM**.

## Featured open source

Fragmenty stacku, którego używam w komercyjnych wdrożeniach — bierz i używaj:

| Repo | Co to jest | Stack | AI-first |
|---|---|---|---|
| **[threejs-product-configurator-starter](https://github.com/GronskiDeveloper/threejs-product-configurator-starter)** · [live demo →](https://gronskideveloper.github.io/threejs-product-configurator-starter/) | Minimalny konfigurator produktu 3D — parametryczna geometria, wybór wykończenia, wycena na żywo | Three.js · WebGL | [CLAUDE.md](https://github.com/GronskiDeveloper/threejs-product-configurator-starter/blob/main/CLAUDE.md) |
| **[claude-chat-widget](https://github.com/GronskiDeveloper/claude-chat-widget)** · [UI preview →](https://gronskideveloper.github.io/claude-chat-widget/showcase.html) | Chatbot AI na stronę firmową: bezpieczne proxy PHP (klucz API zostaje na serwerze) + widget vanilla JS ~6 KB | PHP 8.1 · Claude API | [CLAUDE.md](https://github.com/GronskiDeveloper/claude-chat-widget/blob/main/CLAUDE.md) · [CASE_STUDY](https://github.com/GronskiDeveloper/claude-chat-widget/blob/main/CASE_STUDY.md) |
| **[claude-chat-react](https://github.com/GronskiDeveloper/claude-chat-react)** · [`npm i @grodev/claude-chat-react` ↗](https://www.npmjs.com/package/@grodev/claude-chat-react) | Reactowy chatbot AI: komponent + hook `useClaudeStream`, TypeScript, ~8 KB gzipped, zero runtime deps poza React. **Opublikowany na npm.** | React 18+ · TypeScript · Claude API | [CLAUDE.md](https://github.com/GronskiDeveloper/claude-chat-react/blob/main/CLAUDE.md) |
| **[booking-slots-php](https://github.com/GronskiDeveloper/booking-slots-php)** | Silnik wolnych terminów dla systemów rezerwacji — godziny otwarcia + istniejące rezerwacje ⇒ wolne sloty | PHP 8.1 · Laravel-ready | [CLAUDE.md](https://github.com/GronskiDeveloper/booking-slots-php/blob/main/CLAUDE.md) |
| **[woocommerce-custom-product-data](https://github.com/GronskiDeveloper/woocommerce-custom-product-data)** | Plugin WordPress: konfiguracja produktu do koszyka i zamówienia — most między konfiguratorem 3D a WooCommerce | PHP · WordPress | [CLAUDE.md](https://github.com/GronskiDeveloper/woocommerce-custom-product-data/blob/main/CLAUDE.md) |
| **[booking-ai-demo](https://github.com/GronskiDeveloper/booking-ai-demo)** ⭐ **fusion** | Kompletna aplikacja demo składająca trzy repo powyżej w realny produkt: landing salonu kosmetycznego z kalendarzem rezerwacji online i asystentem AI. Dowód że umiem łączyć komponenty w działający biznes, nie tylko izolowane biblioteki. | React · TS · PHP · Claude API | [CLAUDE.md](https://github.com/GronskiDeveloper/booking-ai-demo/blob/main/CLAUDE.md) |

## Usługi

- [Konfigurator 3D produktu](https://grodev.pl/konfigurator-produktowy-3d) — 12–55 tys. zł
- [Asystenty AI na Claude API](https://grodev.pl/ai) — 4–15 tys. zł
- [System rezerwacji online](https://grodev.pl/system-rezerwacji-online) — od 15 tys. zł
- [Sklep WooCommerce](https://grodev.pl) — 15–40 tys. zł
- [System CRM na zamówienie](https://grodev.pl) — 25–80 tys. zł
- [Aplikacja desktopowa (Python/Qt)](https://grodev.pl) — 15–60 tys. zł

## Kontakt

🌍 **[grodev.pl](https://grodev.pl)**
📧 dominik@grodev.pl
📞 +48 888 517 845
📍 Poznań, PL — pracuję zdalnie w całej Polsce i EU

## Znajdź mnie

[![grodev.pl](https://img.shields.io/badge/Website-grodev.pl-1D9E75?style=flat-square&logo=googlechrome&logoColor=white)](https://grodev.pl)
[![npm](https://img.shields.io/badge/npm-@grodev-CB0000?style=flat-square&logo=npm&logoColor=white)](https://www.npmjs.com/~grodev)
[![Dev.to](https://img.shields.io/badge/Dev.to-@gronskideveloper-000000?style=flat-square&logo=devdotto&logoColor=white)](https://dev.to/gronskideveloper)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Dominik_Groński-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/grodev)
[![LinkedIn Company](https://img.shields.io/badge/LinkedIn-GroDev_(firma)-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/grodev-pl)
[![X](https://img.shields.io/badge/X-@GronskiDev-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/GronskiDev)
[![Facebook](https://img.shields.io/badge/Facebook-GroDev-1877F2?style=flat-square&logo=facebook&logoColor=white)](https://www.facebook.com/profile.php?id=61591220535823)
[![Instagram](https://img.shields.io/badge/Instagram-@gronski__dev-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/gronski_dev/)
[![Google Business](https://img.shields.io/badge/Google-Wizyt%C3%B3wka-4285F4?style=flat-square&logo=google&logoColor=white)](https://share.google/Ya69VkMYlbbod2naZ)

*JDG · NIP 7773109895 · ul. Wawrzyńca Engeströma 10, 60-571 Poznań*
