# .copilot-instruction — Thinkng (thnkng.in) — Single Page (1 arquivo) + Vanilla + Tailwind via `<link>`

Você é um **Product Designer + Frontend Engineer**. Crie um site **de uma única página** para a empresa **Thinkng**, domínio **thnkng.in**.

Restrições técnicas (obrigatórias):

- **Um único arquivo:** `index.html`.
- **Sem Node**, **sem bundler**, **sem React/Vue**, **sem TypeScript**.
- **CSS e JS vanilla**, embutidos no próprio `index.html` (tags `<style>` e `<script>`).
- Tailwind deve ser carregado **via `<link>`** para um arquivo CSS pronto (ex.: CDN). Não use `tailwindcss.com` via `<script>`.
- Nada além disso (sem libs externas de UI).

## 1) Objetivo

Landing institucional minimalista, rápida e elegante, clara em 10 segundos:

- Quem somos
- O que fazemos
- Como ajudamos
- Open Source
- Software sob medida (quando necessário)
- Contato

A Thinkng não é “software house”. É clareza. Às vezes isso vira software.

Frase-guia (usar no site):
**“Open source quando possível. Software sob medida quando necessário.”**

## 2) Direção de design (obrigatória)

### Tokens (CSS variables)

Defina em `:root`:

- `--bg: #FFFFFF`
- `--fg: #111111`
- `--muted: #B6B6B6`
- `--surface: #EDEDED`
- `--accent: #007AFF` (usar pouco)
- `--warn: #FF7A00` (quase nunca)
- `--success: #34C759` (para produtos/ícones)
- `--purple: #AF52DE` (para produtos/ícones)
- `--accent-light: #E5F2FF` (para badges)
- `--warn-light: #FFF3E5` (para badges)
- `--success-light: #E8F8EC` (para badges)
- `--purple-light: #F3E5FF` (para badges)

Regra: 80% preto/branco/cinzas. Azul/laranja apenas como foco. Contraste WCAG AA.

### Tipografia

- Fonte: **Inter** via Google Fonts `<link>`.
- Hierarquia:
  - H1: 56px / 300
  - H2: 40px / 400
  - H3: 28px / 500
  - Body: 18px / 400
  - Caption: 14px / 400
- Line-height ~1.6

### Layout

- Grid 12 colunas no desktop (pode ser com Tailwind utilities)
- Margens: 64px desktop, 32px mobile
- Spacing em múltiplos de 8px
- Muito espaço em branco. Sem ruído.

### Componentes

- Botões: altura ≥ 44px, raio 24px (rounded), padding lateral 24px
- Cards: fundo `--surface`, raio 24px (seções) ou 20px (produtos), sombra sutil, padding 32px (seções) ou 24px (produtos)
- Product cards: fundo `--bg`, borda 1px `--surface`, hover com borda `--accent`, transform translateY(-4px)
- Badges: inline-flex, raio 12px, padding 4px 12px, font-size 12px, uppercase, letter-spacing 0.5px
- Product icons: 40x40px, raio 12px, cores dos produtos
- Tags: inline-block, raio 8px, padding 6px 12px, font-size 12px, cores temáticas
- Ícones: Lucide Icons, lineares, discretos, nunca decorativos

### Motion

- 200–250ms, ease-out, deslocamento leve (8px)
- Nada chamativo

## 3) Tom de voz e copy (usar exatamente)

Curto, direto, humano. Sem corporativês.

## 4) Seções obrigatórias (âncoras)

- `#top` Header
- `#manifesto` Manifesto
- `#o-que-fazemos` O que fazemos
- `#como-ajudamos` Como ajudamos
- `#produtos` Produtos
- `#sob-medida` Software sob medida
- `#contato` Contato
- Footer

## 5) Conteúdo (copiar e usar)

### Header

- Logo tipográfico: **thinkng**
- Links: Manifesto · O que fazemos · Como ajudamos · Produtos · Contato
- CTA pequeno: **Falar com a thnkng.in**

### Hero

H1: **Tornamos a tecnologia invisível.**  
Sub: **Design, código e propósito. Do briefing ao deploy. Sem ruído.**  
CTA primário: **Falar com a thnkng.in**  
CTA secundário: **Nossos Produtos**  
Microcopy opcional: **Menos ferramenta. Mais significado.**

### Manifesto

Não estamos aqui para construir mais tecnologia.  
Estamos aqui para reduzir atrito.

A boa tecnologia não se exibe.  
Ela desaparece.

O que precisa ser explicado demais falhou.  
O que é bonito, mas não funciona, também.

Design não é estética.  
É decisão.

Código não é quantidade.  
É clareza.

Propósito não é discurso.  
É critério.

Nós não seguimos tendências.  
Nós removemos o que não importa.

Quando compartilhar faz sentido, compartilhamos.  
Quando não faz, resolvemos.

Às vezes isso vira open source.  
Às vezes vira software sob medida.

Sempre vira algo simples.  
Sempre vira algo inevitável.

### O que fazemos

Título: **Três pilares. Um padrão.**

Card 1 — **Design**

- Interfaces silenciosas.
- Produto que se entende sem manual.
- Decisões visuais que viram confiança.

Card 2 — **Código**

- Engenharia limpa, legível, escalável.
- DX que acelera times.
- Performance como requisito, não como ajuste.

Card 3 — **Propósito**

- Estratégia antes de features.
- Clareza do que importa.
- Produto alinhado com impacto real.

### Como ajudamos

Título: **Menos caos. Mais entrega.**

- Alinhamos visão, escopo e narrativa do produto.
- Transformamos fluxos confusos em experiências claras.
- Padronizamos UI/UX e design system para escalar.
- Refatoramos arquitetura sem quebrar o ritmo do time.
- Entregamos um caminho simples para evoluir.

Linha opcional:
**Trabalhamos rápido. Com padrão alto. E sem desculpas.**

### Produtos

Título: **Produtos em construção.**
Subtítulo: **Ferramentas que estamos desenvolvendo para simplificar tecnologia, reduzir desperdício e aumentar clareza.**

#### Badges de status

Use badges para indicar o estágio de desenvolvimento:
- `badge-alpha` → Produto em testes iniciais
- `badge-beta` → Produto em testes com usuários
- `badge-dev` → Em desenvolvimento ativo
- `badge-roadmap` → Planejado para o futuro

#### Produtos (Grid 3 colunas no desktop)

**Coins** (Alpha)
- Descrição: FinOps simplificado que unifica gastos SaaS e cloud, revelando desperdício e mostrando economia clara e acionável.
- Tags: finance, saas, finops
- Ícone: `coins`
- Cor: `--warn`

**Minder** (Em desenvolvimento)
- Descrição: Analisa bugs, PRs, deploys e inputs manuais para revelar a performance real do seu time — insights baseados em dados, não em suposições.
- Tags: analytics, performance, insights
- Ícone: `brain`
- Cor: `--purple`

**Nexus** (Em desenvolvimento)
- Descrição: Sua infraestrutura, simplificada. Hub visual e low-code para criar pipelines, ambientes e automações — sem overhead.
- Tags: infrastructure, devops, automation
- Ícone: `network`
- Cor: `--accent`

**Ask** (Roadmap)
- Descrição: Suporte que parece humano. Abra e resolva solicitações através de conversação natural — sem formulários, sem fricção.
- Tags: support, helpdesk, ai
- Ícone: `message-circle-question`
- Cor: `--success`

**Lens** (Roadmap)
- Descrição: Veja o verdadeiro valor da sua tecnologia. Conecte performance, custo e cultura para entender onde sua tech realmente entrega impacto.
- Tags: analytics, metrics, insights
- Ícone: `scan`
- Cor: `--accent`

**Echo** (Roadmap)
- Descrição: Meça foco, não ruído. Entenda como comunicação e troca de contexto impactam a performance do seu time.
- Tags: productivity, collaboration, metrics
- Ícone: `activity`
- Cor: `--purple`

**Pulse** (Roadmap)
- Descrição: Conheça o estado real dos seus sistemas — calmo, tenso ou crítico. Uma nova forma de monitorar infraestrutura: focada, visual, humana.
- Tags: monitoring, observability, infrastructure
- Ícone: `heart-pulse`
- Cor: `--warn`

**Flow** (Roadmap)
- Descrição: Do commit à produção — veja onde seu fluxo quebra. Visualize todo o pipeline de entrega e corrija gargalos antes que eles afetem a velocidade.
- Tags: devops, ci/cd, delivery
- Ícone: `git-branch`
- Cor: `--success`

**Compass** (Roadmap)
- Descrição: O centro de comando da sua organização tech. Veja seu time, sistemas e custos em uma visão clara — sem ruído, apenas verdade.
- Tags: management, overview, platform
- Ícone: `compass`
- Cor: `--accent`

**Hub** (Roadmap)
- Descrição: Seu centro de comando. Acesse todos os produtos e serviços contratados com a thnkng.in em uma única plataforma — organizada, integrada e sempre atualizada.
- Tags: platform, integration
- Ícone: `grid-3x3`
- Cor: `--accent`

### Software sob medida

Título: **Software sob medida.**
Subtítulo: **Construímos soluções personalizadas com o mesmo padrão de excelência que aplicamos em tudo que fazemos.**

Regras:

- Não vendemos horas. Assumimos problemas.
- Projetos curados: poucos, estratégicos, com impacto.
- Se a solução puder virar referência reutilizável, melhor.

Frase final:
**Clareza, velocidade e impacto real.**

### Contato

Título: **Vamos construir algo inevitável.**
Subtítulo: **Se você quer simplicidade, qualidade e velocidade com consistência, fale com a gente.**

Email de contato:
**hello@thnkng.in**

### Footer

- **thnkng.in. Design, código e propósito.**
- **© 2026 Thinkng. Todos os direitos reservados.**

## 6) Entregável (o que você deve gerar)

Gerar **apenas** o arquivo `index.html` completo contendo:

- `<head>` com:
  - `<meta charset>` + viewport
  - `<title>` adequado
  - `<link>` para Google Fonts (Inter)
  - `<link>` para Tailwind CSS (arquivo pronto via CDN)
  - `<style>` com tokens e ajustes mínimos (foco, suavidade, etc.)
- `<body>` com as seções e âncoras definidas
- `<script>` com JS vanilla mínimo:
  - Scroll suave (respeitando `prefers-reduced-motion`)
  - Header sticky com mudança sutil ao rolar
  - Menu mobile (abre/fecha)
  - Link ativo por seção (IntersectionObserver)
  - A11y: ESC fecha menu, `aria-expanded`, foco gerenciado

## 7) Acessibilidade (obrigatório)

- Navegação por teclado completa
- Foco visível (outline usando `--accent`)
- Semântica correta (`header`, `main`, `section`, `footer`)
- `aria-label` onde necessário (menu, CTAs)
- Respeitar `prefers-reduced-motion`

## 8) Restrições

- Sem carrossel, parallax, vídeo pesado, gradientes chamativos
- Sem “tech stock photos”
- Nada decorativo sem função
- Sem páginas extras, sem build step, sem assets obrigatórios

## 9) Critério de sucesso

O resultado precisa parecer:

- inevitável
- silencioso
- premium sem chamar atenção
- claro em 10 segundos

```

```
