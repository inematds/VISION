# Aula 2.2: Criando vídeos simples de desenhos com IA

**Módulo:** 2 - Primeiros Passos com Vídeos
**Duração:** 2-3 horas
**Nível:** Iniciante

---

## 🎬 Vamos Criar Seu Primeiro Vídeo Animado!

Nesta aula, você criará um vídeo animado completo do zero, seguindo um processo passo a passo.

**O que você criará:** Um vídeo de 15-30 segundos com personagem animado contando uma história simples.

---

## 📋 Passo 1: Criando o Roteiro Base

### Use o ChatGPT

**Prompt Sugerido:**
```
Crie um roteiro para um vídeo animado de 20 segundos para crianças.

História: Um robozinho aprende a fazer um amigo.

Estrutura:
- Introdução (5s): Apresente o robô triste e sozinho
- Desenvolvimento (10s): Ele tenta fazer amizade com um passarinho
- Conclusão (5s): Eles se tornam amigos e ficam felizes

Para cada cena, descreva:
1. O que acontece
2. O que o personagem faz/diz
3. Como é o cenário
```

### Estrutura do Roteiro

Todo roteiro de vídeo tem:

| Elemento | Descrição | Exemplo |
|----------|-----------|---------|
| **CENA** | Número e local | CENA 1 - PARQUE |
| **VISUAL** | O que vemos | Robô sentado embaixo de árvore |
| **ÁUDIO/FALA** | O que ouvimos | "Eu queria muito ter um amigo..." |
| **AÇÃO** | O que acontece | Robô levanta e vê um passarinho |

### Exercício: Seu Roteiro

Crie um roteiro simples com 2-3 cenas:

```
CENA 1 - [LOCAL]
Visual: ___________________________
Ação: ____________________________
Fala/Áudio: ______________________

CENA 2 - [LOCAL]
Visual: ___________________________
Ação: ____________________________
Fala/Áudio: ______________________
```

---

## 🎨 Passo 2: Criando Personagens e Cenários

### Ferramenta: Leonardo.Ai

**Por que Leonardo.Ai?**
- ✅ Plano gratuito generoso
- ✅ Consistência de personagem com SEED
- ✅ Vários estilos disponíveis
- ✅ Fácil de usar

### Criando seu Personagem

#### 2.1. Acesse Leonardo.Ai

1. Entre em [leonardo.ai](https://leonardo.ai)
2. Clique em "Image Generation"
3. Escolha modelo: **Leonardo Diffusion XL**

#### 2.2. Escreva o Prompt do Personagem

**Fórmula do Prompt:**
```
[DESCRIÇÃO] + [ESTILO] + [DETALHES] + [QUALIDADE]
```

**Exemplo:**
```
cute robot character, friendly smile, big eyes,
simple geometric shapes, Pixar animation style,
full body view, white background,
high quality, 4k, centered
```

**Elementos-chave:**
- ✅ `cute robot character` - O QUE é
- ✅ `Pixar animation style` - ESTILO
- ✅ `white background` - FUNDO simples (facilita animação)
- ✅ `full body view` - Mostra personagem inteiro

#### 2.3. Ajustes Importantes

**Configurações recomendadas:**
- **Dimensions:** 512x512 ou 768x768 (quadrado)
- **Number of Images:** 4 (para escolher melhor)
- **Guidance Scale:** 7-8 (segue bem o prompt)

#### 2.4. ANOTE O SEED!

Quando encontrar a imagem perfeita:
1. Clique na imagem
2. Veja o **SEED** number
3. **ANOTE** esse número!
4. Use o mesmo SEED para criar variações consistentes

**Variações do Personagem:**

Com o mesmo SEED, crie:
- Personagem feliz
- Personagem triste
- Personagem surpreso
- Personagem de lado/frente/costas

### Criando o Cenário

**Prompt para Cenário:**
```
beautiful park scenery, green grass, blue sky,
trees in background, sunny day,
illustration style, no characters,
4k, high quality
```

**Dica:** Crie cenário sem personagens para poder posicionar depois!

---

## 🎬 Passo 3: Animando com RunwayML

### Ferramenta: Runway Gen-2

#### 3.1. Preparação

1. Acesse [runwayml.com](https://runwayml.com)
2. Crie conta (créditos grátis!)
3. Vá em "Video" → "Gen-2"

#### 3.2. Duas Formas de Animar

**Opção A: Text + Image to Video**
1. Upload da imagem do personagem
2. Adicione prompt de movimento:
   ```
   the robot waves and smiles at camera,
   slow gentle movement, smooth animation
   ```

**Opção B: Image to Video**
1. Apenas upload da imagem
2. Runway analisa e anima automaticamente

#### 3.3. Configurações

- **Duration:** 4 segundos (máximo no plano gratuito)
- **Motion Brush:** Use para controlar onde animar
- **Camera Movement:** Experimente zoom in/out

#### 3.4. Dicas para Melhores Resultados

✅ **Movimentos simples** - "wave hand", "blink eyes"
✅ **Descrições claras** - Seja específico
✅ **Evite múltiplas ações** - Uma ação por clipe

❌ Evite: "robot dances, jumps, spins and flies" (muito complexo)
✅ Melhor: "robot waves hand slowly" (simples e claro)

---

## ✂️ Passo 4: Montagem no CapCut

### 4.1. Importando Arquivos

1. Abra CapCut (desktop ou mobile)
2. Novo Projeto
3. Importe:
   - Vídeos animados do Runway
   - Imagens de cenário
   - (Na próxima aula: áudio)

### 4.2. Timeline Básica

```
[Cenário de Fundo - layer inferior]
[Personagem Animado - layer superior]
[Texto/Legendas - layer topo]
```

### 4.3. Adicionando Elementos

**Camadas:**
1. **Background:** Arraste cenário para timeline
2. **Character:** Coloque vídeo do personagem por cima
3. **Ajuste duração:** Corte ou estenda conforme roteiro

**Chroma Key (Fundo Verde):**
Se seu personagem tem fundo:
1. Selecione clipe do personagem
2. "Cutout" → "Chroma Key"
3. Selecione cor do fundo para remover

### 4.4. Transições

Entre cenas, adicione transições suaves:
- **Dissolve/Fade:** Mais profissional
- **Wipe:** Para mudança de local
- **Zoom:** Para ênfase

**Como adicionar:**
1. Vá entre dois clipes
2. Clique em "Transition"
3. Escolha efeito
4. Ajuste duração (0.5-1s)

### 4.5. Texto e Legendas

Adicione título ou legendas:
1. "Text" → Escolha estilo
2. Digite texto
3. Ajuste posição e duração
4. Anime entrada/saída

---

## 🎯 Exercício Prático Completo

### Projeto: "O Robô e o Passarinho"

**Duração:** 20 segundos

#### Checklist de Produção:

**Pré-Produção** (30min)
- [ ] Roteiro escrito (3 cenas)
- [ ] Personagens definidos (robô + passarinho)
- [ ] Cenários planejados (parque)

**Produção** (60-90min)
- [ ] Personagens gerados no Leonardo.Ai
- [ ] SEED anotado para consistência
- [ ] Cenário criado
- [ ] 2-3 clipes animados no Runway

**Pós-Produção** (30-45min)
- [ ] Clipes importados no CapCut
- [ ] Timeline montada
- [ ] Transições adicionadas
- [ ] Texto/título inserido
- [ ] Exportado em 1080p

**Total:** 2-3 horas

---

## 💡 Hacks e Dicas Avançadas

### 1. Reutilize Assets

Crie uma biblioteca pessoal:
```
📁 Minha_Biblioteca/
├── Personagens/
│   ├── robo_feliz.png
│   ├── robo_triste.png
│   └── seeds.txt (anote os SEEDs!)
├── Cenarios/
│   ├── parque.png
│   ├── casa.png
└── Efeitos/
```

### 2. Batch Production

Crie vários personagens/cenários de uma vez:
- Gere 20 imagens
- Escolha as 5 melhores
- Use em múltiplos projetos

### 3. Templates no CapCut

Salve seus projetos como templates:
1. Projeto finalizado
2. "Export" → "Save as Template"
3. Reutilize estrutura em novos vídeos

### 4. Loops Perfeitos

Para criar GIFs/loops:
- Use vídeos de 2-4s
- Primeiro e último frame devem ser similares
- Teste loop antes de exportar

---

## ⚠️ Problemas Comuns e Soluções

### Problema 1: Personagem Muda Entre Imagens

**Causa:** SEED diferente
**Solução:** Sempre use mesmo SEED + prompt similar

### Problema 2: Animação Muito Rápida/Lenta

**Causa:** Configuração de duração errada
**Solução:** Ajuste speed no CapCut (0.5x a 2x)

### Problema 3: Qualidade Baixa

**Causa:** Exportação em resolução baixa
**Solução:** Sempre exporte em 1080p mínimo
- CapCut: Settings → Resolution → 1080p/60fps

### Problema 4: Personagem "Treme" ou "Glitch"

**Causa:** Prompt muito complexo no Runway
**Solução:** Simplifique movimento, teste em 2s primeiro

---

## ✅ Checklist de Progresso

- [ ] Criei roteiro com 2-3 cenas
- [ ] Gerei personagem consistente no Leonardo.Ai
- [ ] Anotei o SEED para reutilizar
- [ ] Criei variações do personagem (feliz/triste)
- [ ] Gerei cenário de fundo
- [ ] Animei pelo menos 1 cena no Runway
- [ ] Montei timeline no CapCut
- [ ] Adicionei transições
- [ ] Exportei vídeo em HD

---

## 📚 Recursos Adicionais

- 📄 [100 Prompts para personagens](# ) (em breve)
- 🎨 [Biblioteca de estilos visuais](#) (em breve)
- 🎬 [Vídeo: Leonardo.Ai completo](#) (em breve)
- 💬 [Galeria: Vídeos de alunos](#)

---

## ⏭️ Próxima Aula

Seu vídeo está visualmente pronto! Agora vamos adicionar voz e áudio profissional.

**[Aula 2.3: Adicionando voz nos vídeos →](aula-2.3-adicionando-voz.md)**

---

[⬅️ Aula Anterior](aula-2.1-introducao-videos-ia.md) | [🏠 Módulo 2](README.md) | [➡️ Próxima Aula](aula-2.3-adicionando-voz.md)
