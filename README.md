# 📚 Agent Content Creation - Pliki Konfiguracyjne

## Przegląd

Ten folder zawiera kompletny zestaw plików konfiguracyjnych do pracy z agentami AI (Claude Code, Gemini CLI itp.) w kontekście content marketingu. Pliki te definiują zachowanie agenta, styl komunikacji, standardy SEO i gotowe szablony.

## 📁 Struktura plików

### 1. **agent.md** - Definicja agenta
**Główny plik definiujący rolę i zadania agenta.**

**Zawiera:**
- Definicję roli (Content Marketing Specialist)
- Kluczowe kompetencje
- Proces pracy (before → during → after)
- Zasady i ograniczenia
- Formaty outputu
- Linki do innych zasobów

**Kiedy używać:**
- Na początku każdego projektu (agent czyta ten plik aby zrozumieć swoją rolę)
- Przy onboardingu nowych członków zespołu
- Jako źródło prawdy o tym, co agent powinien robić

### 2. **tone_of_voice.md** - Styl komunikacji
**Definicja tonu, głosu i stylu pisania marki.**

**Zawiera:**
- 3 filary tonu (Konkretny, Pomocny, Przemyślany)
- Głos w różnych kontekstach (blog, LinkedIn, opisy)
- Słownictwo (co używać, czego unikać)
- Przykłady dobre vs złe
- Checklist przed publikacją

**Kiedy używać:**
- Przy każdej treści (agent sprawdza czy ton jest spójny)
- Przy briefowaniu freelancerów
- Podczas brand audits

### 3. **seo_checklist.md** - Standardy SEO
**Kompleksowa checklist optymalizacji SEO.**

**Zawiera:**
- 10 sekcji: od keyword research po post-publishing
- Szczegółowe checklisty dla każdego elementu
- Narzędzia do użycia
- Targetowe wartości metryk

**Kiedy używać:**
- Przed publikacją każdej treści SEO
- Do audytów istniejącego contentu
- Jako template do review procesu

### 4. **brand_guidelines.md** - Wytyczne brandowe
**Pełne brand guidelines dla content marketingu.**

**Zawiera:**
- Brand identity (kim jesteśmy, dla kogo)
- Voice & tone (szczegółowo)
- Writing style i vocabulary
- Content pillars
- Visual style
- Channel-specific guidelines
- Quality standards

**Kiedy używać:**
- Podczas onboardingu zespołu
- Przy większych projektach (rebranding, new products)
- Jako reference dla agencji zewnętrznych

### 5. **content_templates.md** - Gotowe szablony
**6 gotowych szablonów dla różnych typów treści.**

**Zawiera szablony dla:**
1. Blog Post (How-To Guide)
2. Data-Driven Report/Study
3. Case Study
4. LinkedIn Post (3 formaty)
5. Newsletter
6. Product/Service Description

**Kiedy używać:**
- Na starcie każdego nowego content piece
- Jako inspiration podczas writer's block
- Do standardyzacji outputu w zespole

---

## 🚀 Jak używać z narzędziami CLI

### Claude Code

**Setup:**
```bash
# Umieść pliki w folderze projektu
mkdir -p ~/marketing-content/config
cd ~/marketing-content/config

# Skopiuj wszystkie pliki .md
```

**Przykłady użycia:**

```bash
# Napisanie artykułu blogu
claude-code "Napisz artykuł SEO o 'AI w content marketingu' 
używając wytycznych z agent.md, tone_of_voice.md i seo_checklist.md.
Użyj szablonu 'How-To Guide' z content_templates.md"

# Case study
claude-code "Stwórz case study dla klienta XYZ 
według szablonu z content_templates.md 
w tonie z brand_guidelines.md"

# Audyt istniejącej treści
claude-code "Przeanalizuj ten artykuł pod kątem seo_checklist.md
i zaproponuj konkretne poprawki"
```

### Gemini CLI / Inne narzędzia

Podobnie jak z Claude Code - narzędzia czytają pliki markdown i stosują się do wytycznych.

---

## 🎯 Workflow content creation

### Krok 1: Planning
```bash
# Agent analizuje temat i sprawdza wytyczne
claude-code "Research topic 'Technical SEO trends 2026'
- Sprawdź content_templates.md który format jest najlepszy
- Zidentyfikuj słowa kluczowe
- Przeanalizuj top 10 w Google
- Zaproponuj outline"
```

### Krok 2: Brief
```bash
# Agent tworzy szczegółowy brief
claude-code "Stwórz content brief dla artykułu na podstawie research,
uwzględniając agent.md proces pracy"
```

### Krok 3: Writing
```bash
# Agent pisze według wytycznych
claude-code "Napisz artykuł według brief i szablonu,
stosując się do tone_of_voice.md i brand_guidelines.md"
```

### Krok 4: Optimization
```bash
# Agent optymalizuje SEO
claude-code "Przejdź przez seo_checklist.md punkt po punkcie
i zoptymalizuj artykuł"
```

### Krok 5: Review
```bash
# Self-review przed publikacją
claude-code "Wykonaj final check zgodnie z wszystkimi guidelines
i zaproponuj poprawki jeśli potrzebne"
```

---

## 🔧 Customizacja dla Twojej firmy

### Co dostosować:

**W agent.md:**
- [ ] Zmień specjalizację (e-commerce → SaaS, B2B → B2C)
- [ ] Dodaj własne przykłady high-quality content
- [ ] Zaktualizuj listę narzędzi (dodaj własne)

**W tone_of_voice.md:**
- [ ] Dostosuj 3 filary do swojej marki
- [ ] Zmień przykłady na własne
- [ ] Dodaj specyficzne "zakazane wyrażenia" dla branży

**W brand_guidelines.md:**
- [ ] Wypełnij sekcję "Kim jesteśmy"
- [ ] Dodaj swoje logo guidelines
- [ ] Określ własne content pillars
- [ ] Dodaj linki do brand assets

**W content_templates.md:**
- [ ] Dostosuj długości do swojej strategii
- [ ] Dodaj własne szablony (np. webinar landing page)
- [ ] Zmień CTAs na własne

### Przykład customizacji:

```markdown
# W agent.md - zmiana dla SaaS B2B

## Kluczowe kompetencje

### 1. Tworzenie treści
- Product comparisons (vs. konkurencja)
- Feature announcements
- Integration guides
- API documentation (user-friendly)
- Customer success stories

### 2. Optymalizacja SEO
- Bottom-of-funnel keywords (buying intent)
- Comparison pages (vs, alternative, competitor)
- Integration pages (X + Y)
```

---

## 📊 Metryki sukcesu

### Dla zespołu content:

**Efektywność:**
- Czas tworzenia treści: -40%
- Consistency score: +60%
- Revision cycles: -50%

**Jakość:**
- SEO score average: 85+/100
- Readability: 60-70 (Flesch)
- Errors per 1000 words: <2

**Rezultaty:**
- Organic traffic growth: [target]
- Conversion rate: [target]
- Engagement rate: [target]

---

## 🤝 Współpraca z zespołem

### Dla content writers:
1. Przeczytaj agent.md i tone_of_voice.md
2. Zapoznaj się z content_templates.md
3. Używaj seo_checklist.md przed każdą publikacją

### Dla SEO specialists:
1. Aktualizuj seo_checklist.md gdy Google zmienia algo
2. Dodawaj nowe best practices
3. Review content pod kątem checklist

### Dla brand managers:
1. Zarządzaj brand_guidelines.md
2. Aktualizuj co kwartał
3. Zapewnij spójność z overall brand strategy

---

## 🔄 Maintenance

### Weekly:
- [ ] Review published content vs. guidelines
- [ ] Update examples w templates (jeśli masz nowe, lepsze)

### Monthly:
- [ ] Sprawdź czy tone_of_voice jest konsistentny
- [ ] Update seo_checklist z nowymi insights

### Quarterly:
- [ ] Full review wszystkich plików
- [ ] Update brand_guidelines jeśli były zmiany
- [ ] Dodaj nowe templates jeśli potrzebne

### Yearly:
- [ ] Major audit i refresh
- [ ] Rebrand considerations
- [ ] Industry trends integration

---

## 📚 Dodatkowe zasoby

### Narzędzia do integracji:

**MCP Servers (dla Claude Code):**
- Google Drive - dostęp do poprzednich treści
- Notion - content calendar
- Airtable - content database
- Slack - notyfikacje o publikacjach

**Skills (opcjonalne):**
- SEO Specialist skill (custom)
- Web Analyzer skill (dla research)
- Content Optimizer skill (custom)

### Przydatne linki:
- [Anthropic MCP Documentation](https://github.com/anthropics/mcp)
- [Claude Code Guide](https://docs.anthropic.com)

---

## ❓ FAQ

**Q: Czy muszę używać wszystkich plików za każdym razem?**
A: Nie. Dla prostych tasków wystarczy agent.md + tone_of_voice.md. Dla kompleksowych projektów użyj wszystkich.

**Q: Jak często aktualizować pliki?**
A: Minimum raz na kwartał. Częściej jeśli są większe zmiany (rebranding, pivot).

**Q: Czy mogę dzielić się tymi plikami z freelancerami?**
A: Tak! To świetny sposób na onboarding. Możesz stworzyć "light version" bez wrażliwych danych.

**Q: Co jeśli moja branża jest bardzo specyficzna?**
A: Dostosuj agent.md i dodaj własne szablony. Framework pozostaje ten sam.

**Q: Czy to działa z innymi AI niż Claude?**
A: Tak! Markdown guidelines działają z każdym LLM (GPT-5, Gemini, itp.)
