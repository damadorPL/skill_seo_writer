# 📚 SEO Content Writer - Skill dla Claude Code

Profesjonalny skill do tworzenia treści SEO dla Claude Code - materiał uzuepłniajacy do publickacji IAB SEMbook 2026 https://www.iab.org.pl/baza-wiedzy/sembook-2026/

## Przegląd

Ten skill przekształca Claude w eksperta content marketingu i SEO, zdolnego do tworzenia wysokiej jakości treści dla digital marketingu i e-commerce. Zapewnia kompleksowe wytyczne do pisania artykułów blogowych, postów na LinkedIn, opisów produktów, case studies i więcej - wszystko zoptymalizowane zarówno dla czytelników, jak i wyszukiwarek.

## Funkcjonalności

- ✅ **Tworzenie treści zoptymalizowanych pod SEO** - Posty blogowe, artykuły, landing pages
- ✅ **Treści Social Media** - Posty na LinkedIn, wątki na Twitterze
- ✅ **Treści E-commerce** - Opisy produktów, strony kategorii
- ✅ **Treści Biznesowe** - Case studies, whitepapers, newslettery
- ✅ **Spójność głosu marki** - Zgodnie ze szczegółowymi wytycznymi tone of voice
- ✅ **Kompleksowa checklista SEO** - 10-sekcyjny przewodnik optymalizacji
- ✅ **Gotowe szablony** - 6 szablonów treści w zestawie

## Instalacja

### Dla Claude Code

1. Sklonuj to repozytorium do katalogu skills Claude Code:

```bash
cd ~/.claude/skills/
git clone https://github.com/damadorPL/skill_seo_writer.git seo-content-writer
```

2. Lub skopiuj skill ręcznie:

```bash
# Pobierz i rozpakuj
curl -L https://github.com/damadorPL/skill_seo_writer/archive/main.zip -o seo-writer.zip
unzip seo-writer.zip
mv skill_seo_writer-main ~/.claude/skills/seo-content-writer
```

3. Zrestartuj Claude Code lub przeładuj skills:

```bash
# Claude Code automatycznie wykryje nowy skill
claude-code --reload-skills
```

### Dla innych platform AI

Ten skill jest zgodny z otwartym standardem SKILL.md i działa z:
- Claude Code
- Codex
- ChatGPT (z obsługą skills)
- Każdym narzędziem obsługującym format SKILL.md

## Użycie

### Frazy aktywujące

Skill aktywuje się automatycznie, gdy użyjesz fraz takich jak:
- "napisz treść seo"
- "stwórz post blogowy"
- "artykuł seo"
- "content marketing"
- "napisz post linkedin"
- "opis produktu"

### Ręczne wywołanie

```bash
# Używając Claude Code
claude-code "Użyj skill seo-content-writer aby stworzyć post blogowy o 'AI w Content Marketingu'"

# Lub jawne wywołanie
claude-code "@seo-content-writer Napisz kompleksowy przewodnik o technical SEO"
```

## Przykładowe zastosowania

### 1. Tworzenie artykułu blogowego

```bash
claude-code "Napisz zoptymalizowany pod SEO artykuł blogowy o 'Trendy w Content Marketingu 2026'
- Słowo kluczowe: trendy content marketing
- Długość: 2000-2500 słów
- Uwzględnij dane i statystyki
- Użyj szablonu How-To Guide"
```

### 2. Post na LinkedIn

```bash
claude-code "Stwórz post na LinkedIn o znaczeniu Core Web Vitals
- Użyj tonu B2B
- Dodaj przykład case study
- Dodaj odpowiednie hashtagi"
```

### 3. Opis produktu

```bash
claude-code "Napisz opis produktu dla 'Usługa audytu SEO'
- Grupa docelowa: firmy B2B
- Uwzględnij korzyści i specyfikację
- Zoptymalizuj pod słowo 'audyt seo'"
```

### 4. Audyt treści

```bash
claude-code "Przeprowadź audyt tego artykułu względem checklisty SEO
i podaj konkretne rekomendacje ulepszeń"
```

## Struktura skilla

```
.claude/skills/seo-content-writer/
├── SKILL.md                    # Główny plik skilla z YAML frontmatter
└── references/                 # Pliki referencyjne
    ├── tone_of_voice.md       # Wytyczne głosu marki i stylu
    ├── brand_guidelines.md    # Kompleksowe wytyczne marki
    ├── seo_checklist.md       # 10-sekcyjna checklista optymalizacji SEO
    └── content_templates.md   # 6 gotowych szablonów treści
```

## Pliki referencyjne

### tone_of_voice.md
Definiuje styl komunikacji marki z trzema filarami:
- **Konkretny** - Używaj konkretnych liczb i danych
- **Pomocny** - Skup się na wartości, nie sprzedaży
- **Przemyślany** - Oparty na danych, nie reaktywny

### brand_guidelines.md
Kompleksowe wytyczne marki zawierające:
- Tożsamość i wartości marki
- Głos i ton w różnych kanałach
- Styl pisania i słownictwo
- Filary treści
- Standardy jakości

### seo_checklist.md
Kompleksowa 10-sekcyjna checklista SEO:
1. Badanie słów kluczowych
2. Struktura treści
3. SEO On-Page
4. SEO techniczne
5. Linkowanie wewnętrzne
6. Linkowanie zewnętrzne
7. Czytelność
8. User Experience
9. Meta tagi i Schema
10. Po publikacji

### content_templates.md
6 gotowych szablonów:
1. Post blogowy (Przewodnik How-To)
2. Raport/Badanie oparte na danych
3. Case Study
4. Post na LinkedIn (3 formaty)
5. Newsletter
6. Opis produktu/usługi

## Personalizacja

Możesz dostosować ten skill do swoich potrzeb:

### 1. Modyfikacja głosu marki
Edytuj `.claude/skills/seo-content-writer/references/tone_of_voice.md` aby dopasować do stylu twojej marki.

### 2. Aktualizacja standardów SEO
Edytuj `seo_checklist.md` aby odzwierciedlić wymagania SEO twojej organizacji.

### 3. Dodanie własnych szablonów
Dodaj nowe szablony do `content_templates.md` dla swoich specyficznych typów treści.

### 4. Dostosowanie fraz aktywujących
Edytuj YAML frontmatter w `SKILL.md` aby dodać własne frazy aktywujące:

```yaml
triggers:
  - "napisz treść seo"
  - "twoja własna fraza"
```

## Przykładowy workflow

### Kompletny proces tworzenia treści

```bash
# Krok 1: Research i planowanie
claude-code "Zbadaj temat 'Technical SEO dla E-commerce'
- Przeanalizuj top 10 wyników w Google
- Zidentyfikuj luki w treści
- Zaproponuj outline"

# Krok 2: Stwórz brief
claude-code "Stwórz brief treści na podstawie researchu"

# Krok 3: Napisz treść
claude-code "Napisz artykuł zgodnie z briefem i checklistą SEO"

# Krok 4: Optymalizuj
claude-code "Przejrzyj artykuł względem seo_checklist.md
i zoptymalizuj punkt po punkcie"

# Krok 5: Finalna weryfikacja
claude-code "Przeprowadź finalną kontrolę jakości względem wszystkich wytycznych"
```

## Standardy jakości

Treści tworzone z użyciem tego skilla spełniają rygorystyczne kryteria jakości:
- ✅ Konkretne (liczby, przykłady, bez ogólników)
- ✅ Pomocne (wykonalne następne kroki)
- ✅ Uczciwe (realistyczne oczekiwania)
- ✅ Zwięzłe (bez pustosłowia)
- ✅ Jasne (wyjaśniona terminologia)
- ✅ Wiarygodne (źródła dla twierdzeń)
- ✅ Wykonalne (praktyczne wnioski)

## Wsparcie językowe

### Polski (Podstawowy)
- Używa formy "Ty" (nieformalnej ale profesjonalnej)
- Strona czynna
- Krótkie, jasne zdania
- Akceptuje terminy angielskie gdy są powszechniejsze

### Angielski (Drugorzędny)
- Ortografia amerykańska
- Bezpośredni i zwięzły
- Zorientowany na działanie

## Metryki wydajności

Oczekiwane ulepszenia przy użyciu tego skilla:
- **Wydajność**: 40% szybsze tworzenie treści
- **Spójność**: 60% poprawa spójności głosu marki
- **Jakość**: Średni wynik SEO 85+/100
- **Czytelność**: Flesch Reading Ease 60-70

## Współpraca

Zachęcamy do współpracy! Aby wnieść wkład:

1. Zforkuj repozytorium
2. Stwórz branch funkcji
3. Wprowadź zmiany
4. Zaktualizuj dokumentację
5. Wyślij pull request

## Kompatybilność

- **Claude Code**: Pełne wsparcie (standard 2026)
- **Claude.ai Skills**: Kompatybilny
- **Codex**: Kompatybilny z formatem SKILL.md
- **ChatGPT**: Kompatybilny (z obsługą skills)
- **Inne platformy**: Każde narzędzie obsługujące standard SKILL.md

## Historia wersji

- **2026.1.0** - Pierwsze wydanie w formacie standardu 2026
  - SKILL.md z YAML frontmatter
  - Struktura oparta na katalogach
  - Kompatybilność cross-platform
  - Zaktualizowane o najnowsze praktyki SEO

## Licencja

Licencja MIT - Zobacz plik LICENSE dla szczegółów

## Autor

**Krzysztof Radzikowski** - Specjalista SEO/SEM R&D

[Strona internetowa](https://radzikow.ski)

## Wsparcie

- **Problemy**: [GitHub Issues](https://github.com/damadorPL/skill_seo_writer/issues)
- **Dyskusje**: [GitHub Discussions](https://github.com/damadorPL/skill_seo_writer/discussions)

## Powiązane zasoby

### Oficjalna dokumentacja
- [Dokumentacja Claude Code Skills](https://code.claude.com/docs/en/skills)
- [Specyfikacja formatu SKILL.md](https://aiskill.market/blog/claude-code-skill-md-format)

### Materiały edukacyjne
- [Kompleksowy przewodnik po Claude Skills 2026](https://anandbg.com/blog/claude-skills-comprehensive-guide-2026)
- [Kompletny przewodnik budowania Skills dla Claude](https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf)

### Społeczność
- [Agent Skills Marketplace](https://skillsmp.com/)
- [Claude Code Skills Guide](https://fp8.co/articles/Claude-Code-Skills-Complete-Developer-Guide)

## FAQ

**P: Czy muszę używać wszystkich plików referencyjnych za każdym razem?**
O: Nie. Dla prostych zadań skill automatycznie wie co użyć. Dla złożonych projektów będzie się odwoływał do wszystkich wytycznych.

**P: Czy mogę udostępnić ten skill mojemu zespołowi?**
O: Tak! Każdy może go zainstalować w swoim katalogu `.claude/skills/`, lub możesz go skonfigurować we wspólnym workspace.

**P: Czy to działa z innymi narzędziami AI poza Claude?**
O: Tak! Format SKILL.md to otwarty standard kompatybilny z wieloma platformami AI.

**P: Czy mogę dostosować to do mojej konkretnej branży?**
O: Absolutnie! Edytuj pliki referencyjne aby dopasować je do twojej branży, marki i wymagań.

**P: Jak zaktualizować skill?**
O: Pobierz najnowsze zmiany z repozytorium, lub użyj `git pull` jeśli sklonowałeś je.

