# Detecção de Comentários Capacitistas no YouTube

Este projeto utiliza **Processamento de Linguagem Natural (PLN)** com o spaCy para identificar **comentários capacitistas** em textos extraídos do YouTube. O código implementa padrões linguísticos específicos com `DependencyMatcher` para detectar frases que contenham termos ofensivos a pessoas com deficiência.

## Objetivo

Automatizar a detecção de **capacitismo textual** em comentários da internet, com foco em identificar estruturas como xingamentos, comparações pejorativas, adjetivos discriminatórios e outras formas sutis ou explícitas de discurso capacitista.

- **spaCy** com `DependencyMatcher`
- Modelo de linguagem: `pt_core_news_lg`
- Análise de padrões gramaticais (sintáticos e semânticos)
- Exportação dos resultados para `.csv`

---

##  Padrões Detectados

O script detecta frases com base em diferentes **padrões de discurso capacitista**, como:

- **Predicação direta:** “ele é burro”, “ela está retardada”
- **Verbo + termo ofensivo:** “ficou idiota”
- **Verbo + intensificador + termo:** “ficou muito burro”
- **Ofensas diretas:** “seu idiota!”, “mongol!”
- **Comparações pejorativas:** “parece um retardado”, “age como um mongolóide”
- **Tratamento depreciativo:** “foi chamado de aleijado”, “tratada como doente mental”

