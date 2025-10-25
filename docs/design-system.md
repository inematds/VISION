# VISION - Design System

**Baseado em:** [FEP Course Website](https://inematds.github.io/FEP/)
**Data de criação:** 25 de Outubro de 2025
**Arquivo CSS:** `css/vision-styles.css`

---

## 📋 Índice

1. [Visão Geral](#visão-geral)
2. [Paleta de Cores](#paleta-de-cores)
3. [Espaçamento](#espaçamento)
4. [Tipografia](#tipografia)
5. [Componentes](#componentes)
6. [Animações](#animações)
7. [Acessibilidade](#acessibilidade)
8. [Como Usar](#como-usar)

---

## 🎨 Visão Geral

O Design System VISION é baseado no estilo visual do site FEP, adaptado para ser reutilizável em projetos de conteúdo educacional e audiovisual. O sistema utiliza **CSS Variables** (Custom Properties) para facilitar a personalização e manutenção.

### Características Principais:

- ✅ Totalmente responsivo
- ✅ Acessível (WCAG 2.1)
- ✅ Animações suaves e performáticas
- ✅ Sistema de cores baseado em níveis/categorias
- ✅ Componentes reutilizáveis
- ✅ Suporte a tema claro/escuro (preparado para expansão)

---

## 🎨 Paleta de Cores

### Cores de Categoria/Nível

```css
--color-iniciante: #10B981;      /* Verde - Nível Iniciante */
--color-tecnico: #3B82F6;        /* Azul - Nível Técnico */
--color-masterclass: #8B5CF6;    /* Roxo - Nível Masterclass */
```

**Uso:** Utilize essas cores para diferenciar níveis de dificuldade, categorias de conteúdo, ou status.

**Exemplo visual:**
- 🟢 **Iniciante (#10B981):** Verde esmeralda, representa facilidade e início
- 🔵 **Técnico (#3B82F6):** Azul médio, representa conhecimento intermediário
- 🟣 **Masterclass (#8B5CF6):** Roxo vibrante, representa expertise avançado

### Cores Primárias

```css
--color-primary: #3B82F6;         /* Azul principal */
--color-primary-hover: #2563EB;   /* Azul hover (mais escuro) */
--color-primary-light: #EFF6FF;   /* Azul claro para backgrounds */
```

### Escala de Cinza

| Variável | Hex | Uso Recomendado |
|----------|-----|-----------------|
| `--color-gray-50` | #F9FAFB | Backgrounds muito claros |
| `--color-gray-100` | #F3F4F6 | Backgrounds claros |
| `--color-gray-200` | #E5E7EB | Bordas sutis |
| `--color-gray-300` | #D1D5DB | Bordas médias |
| `--color-gray-400` | #9CA3AF | Texto secundário, ícones inativos |
| `--color-gray-500` | #6B7280 | Texto terciário |
| `--color-gray-600` | #4B5563 | Texto secundário escuro |
| `--color-gray-700` | #374151 | Texto principal |
| `--color-gray-800` | #1F2937 | Texto destaque |
| `--color-gray-900` | #111827 | Texto muito escuro |

---

## 📏 Espaçamento

Sistema baseado em múltiplos de **1rem (16px)**:

```css
--spacing-xs: 0.25rem;    /* 4px */
--spacing-sm: 0.5rem;     /* 8px */
--spacing-md: 1rem;       /* 16px */
--spacing-lg: 1.5rem;     /* 24px */
--spacing-xl: 2rem;       /* 32px */
--spacing-2xl: 3rem;      /* 48px */
```

### Classes Utilitárias de Espaçamento

```css
/* Margin Top */
.mt-xs, .mt-sm, .mt-md, .mt-lg, .mt-xl

/* Margin Bottom */
.mb-xs, .mb-sm, .mb-md, .mb-lg, .mb-xl

/* Padding Top */
.pt-xs, .pt-sm, .pt-md, .pt-lg, .pt-xl

/* Padding Bottom */
.pb-xs, .pb-sm, .pb-md, .pb-lg, .pb-xl
```

---

## 🔤 Tipografia

### Responsividade Tipográfica

Em telas móveis (max-width: 640px):

```css
h1 { font-size: 2rem; }      /* 32px */
h2 { font-size: 1.75rem; }   /* 28px */
h3 { font-size: 1.5rem; }    /* 24px */
```

### Classes Utilitárias

```css
.font-bold       /* 700 */
.font-semibold   /* 600 */
.font-normal     /* 400 */

.text-center
.text-left
.text-right
```

---

## 🧩 Componentes

### 1. Cards

#### Level Card (Card de Nível/Categoria)

```html
<div class="level-card">
  <!-- Conteúdo do card -->
</div>
```

**Comportamento:**
- Hover: Sombra XL + movimento sutil para cima
- Transição suave com cubic-bezier

#### Module Card (Card de Módulo)

```html
<div class="module-card">
  <!-- Conteúdo do módulo -->
</div>
```

**Comportamento:**
- Hover: Move 4px para cima + sombra LG

---

### 2. Botões

#### Botão Primário

```html
<button class="content-button content-button-primary">
  Começar Agora
</button>
```

**Estilo:**
- Fundo azul (#3B82F6)
- Texto branco
- Hover: Azul mais escuro (#2563EB)

#### Botão Secundário

```html
<button class="content-button content-button-secondary">
  Saber Mais
</button>
```

**Estilo:**
- Fundo transparente
- Borda azul
- Hover: Fundo azul claro (#EFF6FF)

---

### 3. Badges

```html
<span class="badge badge-iniciante">Iniciante</span>
<span class="badge badge-tecnico">Técnico</span>
<span class="badge badge-masterclass">Masterclass</span>
```

**Uso:** Indicadores de nível, categoria ou status

---

### 4. Progress Bar

```html
<div class="progress-bar">
  <div class="progress-fill" style="width: 60%;"></div>
</div>
```

**Características:**
- Altura de 0.5rem
- Gradiente azul → roxo
- Transição suave na mudança de largura

---

### 5. Breadcrumb

```html
<nav class="breadcrumb">
  <a href="/">Início</a>
  <span class="breadcrumb-separator">/</span>
  <a href="/cursos">Cursos</a>
  <span class="breadcrumb-separator">/</span>
  <span>Audiovisual</span>
</nav>
```

---

### 6. Category Filters

```html
<button class="category-filter">Todos</button>
<button class="category-filter active">Audiovisual</button>
<button class="category-filter">Design</button>
```

**Estados:**
- Normal: Borda cinza, texto cinza
- Hover: Borda roxa, fundo roxo claro
- Active: Fundo roxo, texto branco

---

### 7. Toast Notification

```html
<div class="toast">
  Operação realizada com sucesso!
</div>
```

**Características:**
- Posição fixa no canto inferior direito
- Animação de entrada pela direita
- Sombra LG

---

### 8. Loading State

```html
<div class="loading">
  Conteúdo carregando...
</div>
```

**Comportamento:**
- Reduz opacidade para 0.6
- Mostra spinner rotativo centralizado
- Desabilita interações (pointer-events: none)

---

## 🎬 Animações

### Fade In

```html
<div class="animate-fade-in">
  <!-- Conteúdo com fade in -->
</div>
```

**Comportamento:**
- Duração: 0.8s
- Move de 20px baixo para cima
- Opacidade 0 → 1

### Scroll Animation

```html
<div class="animate-on-scroll">
  <!-- Conteúdo revelado ao scroll -->
</div>
```

**Ativação:** Adicione a classe `fade-in` via JavaScript quando o elemento entrar no viewport.

```javascript
// Exemplo de ativação
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('fade-in');
    }
  });
});

document.querySelectorAll('.animate-on-scroll').forEach(el => {
  observer.observe(el);
});
```

---

## ♿ Acessibilidade

### 1. Focus Visible

Todos os elementos interativos têm indicador visual ao receber foco:

```css
*:focus-visible {
  outline: 2px solid #3B82F6;
  outline-offset: 2px;
}
```

### 2. Skip to Main Content

```html
<a href="#main-content" class="skip-to-main">
  Pular para conteúdo principal
</a>
```

**Comportamento:**
- Invisível por padrão
- Aparece ao receber foco (Tab)

### 3. Reduced Motion

Respeita preferência de usuários que desabilitam animações:

```css
@media (prefers-reduced-motion: reduce) {
  /* Animações reduzidas a 0.01ms */
}
```

### 4. Print Styles

Layout otimizado para impressão:
- Remove navegação e rodapé
- Converte tudo para preto e branco

---

## 🚀 Como Usar

### 1. Incluir o CSS

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>VISION</title>

  <!-- Design System VISION -->
  <link rel="stylesheet" href="css/vision-styles.css">
</head>
<body>
  <!-- Seu conteúdo aqui -->
</body>
</html>
```

### 2. Exemplo Completo de Card

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>VISION - Exemplo</title>
  <link rel="stylesheet" href="css/vision-styles.css">

  <!-- Tailwind CSS (opcional, para classes utilitárias extras) -->
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-50">

  <div class="container mx-auto px-4 py-8">

    <!-- Card de Nível -->
    <div class="level-card bg-white p-6 rounded-lg shadow-md">

      <!-- Badge -->
      <span class="badge badge-iniciante mb-4">🌟 Iniciante</span>

      <!-- Título -->
      <h2 class="text-2xl font-bold mb-4">Fundamentos de Audiovisual</h2>

      <!-- Descrição -->
      <p class="text-gray-600 mb-6">
        Aprenda os conceitos básicos de produção audiovisual
        com inteligência artificial.
      </p>

      <!-- Progress Bar -->
      <div class="progress-bar mb-4">
        <div class="progress-fill" style="width: 45%;"></div>
      </div>

      <!-- Botões -->
      <div class="flex gap-md">
        <button class="content-button content-button-primary">
          Continuar Curso →
        </button>
        <button class="content-button content-button-secondary">
          Ver Detalhes
        </button>
      </div>

    </div>

  </div>

</body>
</html>
```

### 3. Personalizando Cores

Para personalizar as cores do sistema, basta sobrescrever as variáveis CSS:

```css
/* Seu arquivo custom.css */
:root {
  --color-primary: #FF6B6B;  /* Vermelho personalizado */
  --color-iniciante: #51CF66; /* Verde mais vibrante */
}
```

### 4. Adicionando Tailwind CSS (Opcional)

O design system funciona muito bem com Tailwind CSS:

```html
<!-- CDN do Tailwind -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Ou via npm -->
<!-- npm install -D tailwindcss -->
```

Combine classes do VISION com Tailwind:

```html
<div class="level-card bg-white p-6 rounded-lg max-w-md mx-auto">
  <!-- Conteúdo -->
</div>
```

---

## 📦 Estrutura de Arquivos Recomendada

```
projeto-vision/
├── css/
│   └── vision-styles.css      # Design System
├── js/
│   └── main.js                # JavaScript principal
├── doc/
│   └── design-system.md       # Esta documentação
└── index.html                 # Página principal
```

---

## 🎯 Próximos Passos

1. **Tema Escuro:** Adicione suporte a dark mode
2. **Mais Componentes:** Cards de vídeo, modal, accordion
3. **Formulários:** Estilos para inputs, selects, checkboxes
4. **Grid System:** Sistema de grid customizado
5. **Ícones:** Integração com biblioteca de ícones

---

## 📝 Changelog

### v1.0.0 - 2025-10-25
- ✅ Primeira versão do Design System
- ✅ Baseado no estilo FEP
- ✅ Componentes principais implementados
- ✅ Sistema de cores e espaçamento
- ✅ Animações e transições
- ✅ Acessibilidade (WCAG 2.1)

---

## 📄 Licença

Este design system foi criado para uso no projeto VISION, baseado em análise do site FEP disponível publicamente.

---

## 🤝 Contribuindo

Sugestões de melhorias e novos componentes são bem-vindas!

---

**Desenvolvido com ❤️ para o projeto VISION**
