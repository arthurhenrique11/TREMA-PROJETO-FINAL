# TRAMA // DPP — Plataforma de Rastreabilidade e Passaporte Digital de Produto

Plataforma web desenvolvida para conectar marcas de moda independente e designers locais a consumidores conscientes, utilizando o conceito de **Passaporte Digital de Produto (DPP)** e etiquetas com **QR Codes dinâmicos** para garantir transparência na cadeia produtiva, mensuração de impacto ambiental e suporte ao ciclo pós-consumo.

---

## Sobre o Projeto

A indústria têxtil tradicional sofre com cadeias produtivas opacas e práticas de *greenwashing*. A **TRAMA // DPP** atua como uma infraestrutura aberta de transparência onde cada peça de roupa recebe um identificador único (UID) vinculado a um histórico auditável.

### Principais Funcionalidades
* **Raio-X de Passaporte Digital (`passaporte-dpp.html`):** Exibe a composição granular da peça, origem geográfica de cada insumo (fibra, linha, aviamentos), linha do tempo de custódia e relato em áudio direto do artesão.
* **Vitrine com Filtragem Sem JavaScript (`catalogo.html`):** Catálogo de peças rastreadas com filtro funcional por tipo de fibra (Algodão Agroecológico, Linho/Cânhamo, Upcycling).
* **Transparência Climática e Hídrica (`impacto.html`):** Gráficos comparativos de consumo de água e emissões de CO₂e frente à indústria convencional.
* **Diretório de Ateliês (`marcas.html`):** Vitrine de estúdios locais verificados com índice de transparência e práticas de comércio justo.
* **Arquitetura Tecnológica (`tecnologia.html`):** Explicação técnica sobre etiquetas tecidas, padrão GS1 Digital Link e vídeo demonstrativo de leitura.
* **Circularidade e Pós-Consumo (`pos-consumo.html`):** Orientações para reparo local, revenda autenticada, logística reversa e guia interativo de conservação têxtil.
* **Onboarding e Autenticação (`cadastro.html` e `login.html`):** Fluxos de solicitação de etiquetas DPP para marcas e acesso ao painel de gestão.

---

## Tecnologias Utilizadas

O projeto foi construído estritamente com tecnologias nativas da web, **sem uso de JavaScript ou frameworks externos**:

* **HTML5 Semântico:** Uso estruturado de `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<figcaption>`, `<table>`, `<details>`, `<summary>`, `<audio>` e `<video>`.
* **CSS3 Externo Modular:** Cada página possui sua própria folha de estilo dedicada na pasta `css/`, utilizando **CSS Custom Properties (Variáveis)**, **CSS Grid**, **Flexbox** e design responsivo via *Media Queries*.
* **Interatividade em CSS Puro:**
  * *Filtros de catálogo:* Implementados com `<input type="radio">` ocultos combinados com a pseudoclasse `:checked` e seletores irmãos (`~`).
  * *Acordeão de FAQ:* Implementado nativamente com as tags `<details>` e `<summary>`.
  * *Confirmação de formulário:* Exibição de modal de sucesso utilizando a pseudoclasse `:target`.