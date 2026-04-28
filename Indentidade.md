# ☠️ PROMPT DE CONTINUIDADE: PROJETO CISCO CYBER DOCS

---

## 🎯 INSTRUÇÃO DE ATUAÇÃO

> "Atue como um Engenheiro Front-end e Especialista em Cybersecurity. O objetivo é dar continuidade à documentação pessoal do curso Cisco Cybersecurity, transformando capturas de tela em seções web de alto nível."

---

## 1. 🎨 IDENTIDADE VISUAL & UI (RIGOROSO)

### 🎯 Paleta de Cores

```css
--bg-main: #121212;      /* Fundo principal */
--card-bg: #1e1e1e;      /* Cards */
--text-main: #ffffff;    /* Texto principal */
--cisco-green: #66bf53;  /* Destaques */
```

### 🔤 Tipografia

* Fonte: **Inter (Google Fonts)**
* Estilo: moderno, legível e técnico

### ☠️ Identidade de Marca

* Uso do símbolo Unicode:

```html
&#9760; <!-- Caveira -->
```

* Aplicação: títulos e elementos de destaque

### ✨ Efeitos Visuais

* **Glassmorphism na Navbar**:

```css
backdrop-filter: blur(10px);
background: rgba(18, 18, 18, 0.7);
```

* **Animações com Anime.js**:

```html
<script src="https://cdn.jsdelivr.net/npm/animejs/lib/anime.min.js"></script>
```

* Classe padrão de animação:

```css
.reveal {
  opacity: 0;
  transform: translateY(20px);
}
```

---

## 2. 🧱 ESTRUTURA DE CÓDIGO & RESPONSIVIDADE

### ⚙️ Framework

* **Bootstrap 5** (layout e responsividade)

### 📌 Navbar

```html
<nav class="navbar navbar-expand-lg sticky-top">
```

* Fixa no topo
* Links com âncora (`#id`)

### 🏷️ Badges Responsivos

```css
.badge-cisco {
  background-color: var(--cisco-green);
}

@media (max-width: 768px) {
  .badge-cisco {
    width: 100%;
    margin-bottom: 12px;
    text-align: center;
  }
}
```

### 🧭 Navegação com Offset

```css
section {
  scroll-margin-top: 100px;
}
```

---

## 3. 🧠 METODOLOGIA DE CONTEÚDO (MASTER LEVEL)

### 📚 Abordagem Didática

* Não apenas listar conceitos
* Aplicar **casos reais de uso**

#### Exemplos:

* **RAT (Remote Access Trojan)** → invasor controla máquina remotamente
* **APT (Advanced Persistent Threat)** → ataque silencioso e contínuo
* **Ransomware** → sequestro de dados com impacto financeiro

### ⚠️ Análise de Risco

Cada ameaça deve conter:

* Impacto financeiro
* Impacto operacional
* Cenário real

**Exemplo:**

> Falha em sistema de sprinklers pode causar interrupção total de operação industrial.

### 🗂️ Organização Visual

* Uso de **cards** para separação de contexto
* Uso de **tabelas responsivas**

```html
<div class="table-responsive">
  <table class="table topic-table"></table>
</div>
```

---

## 4. 📦 BIBLIOTECAS NECESSÁRIAS (CDNs)

### Bootstrap 5

```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

### Font Awesome 6

```html
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
```

### Anime.js

```html
<script src="https://cdn.jsdelivr.net/npm/animejs/lib/anime.min.js"></script>
```

---

## 5. 🧩 PROGRESSO DO PROJETO

### ✅ Módulo 1 - Estrutura Concluída

#### 📌 Seções já documentadas:

* **1.0.1** → Introdução
* **1.0.2** → Aprendizado
* **1.1.1** → Domínios
* **1.1.2** → Tipos de Ameaças
* **1.1.8 / 1.1.9** → Fator Humano
* **1.2.1** → Termos Master

---

## 🚀 PADRÃO DE CONTINUIDADE

Use este prompt para expandir o projeto:

> "Continuando o projeto Cisco Cyber Docs.
> Contexto: Módulo [X].
> Seção: [ID + Nome].
> Aplicar identidade visual padrão (dark + verde Cisco + caveira).
> Incluir: explicação técnica, caso real, impacto e UI com Bootstrap.
> Utilizar animações `.reveal` e organização em cards/tabelas."

---

## ✅ OBSERVAÇÕES FINAIS

* Estrutura pronta para documentação profissional
* Compatível com projetos **HTML estático**, **Next.js** ou **Docusaurus**
* Foco em **alto nível técnico + apelo visual moderno**
* Ideal para portfólio ou documentação pessoal avançada

---

**Versão:** 1.0
**Formato:** Markdown (.md)
**Projeto:** Cisco Cyber Docs
