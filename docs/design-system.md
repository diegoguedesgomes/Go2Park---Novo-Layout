# Go2Park Design System

Versao 0.1.0

## Overview

Go2Park deve se posicionar como uma plataforma de mobilidade operacional: confiavel, tecnica, clara e pronta para gestores que precisam reduzir viagens vazias, controlar frota e provar qualidade de atendimento.

A base conceitual vem do sistema Webflow fornecido: canvas branco generoso, tipografia sem excesso de peso, CTAs disciplinados, cards cromaticos como superficies de categoria e sombras multicamada. A traducao para Go2Park preserva o **near-black como cor de conversao** e usa o azul/verde da marca como linguagem de produto: mapa, dashboard, tracking, status e eficiencia.

**Key Characteristics**

- Canvas branco e superficies cinza-azuladas para leitura limpa em contexto B2B.
- Near-black como cor primaria de CTA, headings e texto de maior hierarquia.
- Azul Go2Park como acento de produto, links de enfase, rotas, tracking e UI ativa.
- Verde-lima reservado para eficiencia, status, economia, sucesso e metricas positivas.
- Acentos saturados aplicados em cards de categoria, nunca como backgrounds de botoes.
- Tipografia Inter com teto de peso em 600, mantendo a voz segura sem gritar.
- Botoes com raio de 4 px, cards com 8 px ou 12 px quando forem superficies de produto.
- Mockups reais do dashboard, app, mapa e WhatsApp como imagens primarias da marca.

## Brand Strategy

### Palavra central

**Controle em tempo real.**

Go2Park nao deve parecer um app generico de transporte. A marca precisa mostrar que conecta tres atores:

- Passageiro: solicita e acompanha a corrida por WhatsApp ou link.
- Motorista: opera a jornada com interface simples.
- Gestor: enxerga demanda, jornada, qualidade e desperdicio no dashboard.

### Promessa de produto

Sistema inteligente para gestao de transporte que digitaliza a jornada da frota, do pedido ao relatorio.

### Tom de voz

- Direto, operacional e consultivo.
- Fala em economia, previsibilidade, qualidade e prestacao de contas.
- Evita exageros de startup e evita linguagem vaga como "revolucionario".
- Prefere frases verificaveis: "setup em 3 a 5 dias", "sem hardware", "link por WhatsApp", "mapa ao vivo".

## Colors

### Brand

| Token | Hex | Use |
|---|---:|---|
| `--g2p-primary` | `#080808` | CTA principal, headings, texto forte e conversao. |
| `--g2p-ink-strong` | `#222222` | Enfase proxima ao preto sem pesar demais. |
| `--g2p-blue` | `#1F64F2` | Cor proprietaria da Go2Park no logo, UI ativa e produto. |
| `--g2p-blue-deep` | `#0F56E5` | Hover de links azuis e superfícies institucionais. |
| `--g2p-lime-brand` | `#A4E244` | Verde da marca no logo, status proprietario e highlights controlados. |

### Accent System

| Token | Hex | Categoria |
|---|---:|---|
| `--g2p-accent-purple` | `#7A3DFF` | Passageiro, experiencia, solicitacao. |
| `--g2p-accent-pink` | `#ED52CB` | Interacoes, notificacoes e momentos de feedback. |
| `--g2p-accent-blue` | `#3B89FF` | Rastreamento, mapa, rotas, tempo real. |
| `--g2p-accent-orange` | `#FF6B00` | Espera, pico, demanda, alerta operacional. |
| `--g2p-accent-green` | `#00D722` | Frota saudavel, sucesso e eficiencia. |
| `--g2p-accent-yellow` | `#FFAE13` | Auditoria, contrato, prestacao de contas. |
| `--g2p-accent-red` | `#EE1D36` | Reclamacoes, risco, atraso critico. |

### Surface & Text

| Token | Hex | Use |
|---|---:|---|
| `--g2p-canvas` | `#FFFFFF` | Fundo principal. |
| `--g2p-canvas-alt` | `#F6F8FC` | Bandas de conteudo e fundos alternados. |
| `--g2p-panel-tint` | `#F1F6FF` | Cards suaves e highlights. |
| `--g2p-hairline` | `#D8D8D8` | Bordas, divisores, inputs. |
| `--g2p-ink` | `#080808` | Texto principal e headings. |
| `--g2p-body` | `#363636` | Paragrafos. |
| `--g2p-muted` | `#898989` | Metadados, placeholders, legendas. |

## Typography

Use **Inter** como familia principal. Se a equipe tiver uma fonte proprietaria no futuro, ela pode substituir Inter mantendo os mesmos pesos e proporcoes.

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---:|---:|---:|---:|---|
| `display-xxl` | 80px | 600 | 83px | -0.8px | Hero desktop. |
| `display-xl` | 56px | 600 | 60px | -0.56px | Hero compacto e secoes-chave. |
| `display-lg` | 44.8px | 600 | 46.6px | 0 | Headlines de secao. |
| `display-md` | 32px | 500 | 40px | 0 | Titulo de bloco ou card grande. |
| `display-sm` | 24px | 500 | 32px | 0 | Card e subsecoes. |
| `body-lg` | 28.8px | 400 | 46.08px | -0.288px | Lead paragraph. |
| `body-md` | 16px | 400 | 26px | -0.16px | Texto padrao. |
| `body-sm` | 14px | 400 | 22.4px | 0 | Captions e textos secundarios. |
| `eyebrow` | 15px | 500 | 19.5px | 1.5px | Labels uppercase de secao. |
| `caption` | 12.8px | 550 | 16px | 0 | Badges e chips. |
| `button-md` | 16px | 500 | 24px | -0.12px | Botoes. |

## Layout

### Spacing

Base de 4 px:

`2, 4, 8, 12, 16, 20, 24, 32, 48, 64, 96`

### Container

- Marketing desktop: max-width 1180 px, gutter 32 px.
- Dashboard/product preview: pode usar 1280 px quando houver mockup largo.
- Mobile: gutter 20 px.

### Breakpoints

| Name | Width | Behavior |
|---|---:|---|
| Mobile | < 480px | Tudo 1 coluna, hero com copy antes do mockup. |
| Tablet | 768px | Cards 2 colunas, hero pode empilhar. |
| Desktop | 992px | Grids 3 colunas, nav completa. |
| Wide | 1280px | Preview de dashboard maior e metricas laterais. |

## Components

### Button Primary

Use near-black como CTA principal. O azul Go2Park aparece em links de enfase, superfícies de produto e estados ativos, mas nao como background padrao de botao.

- Background `#080808`
- Text `#FFFFFF`
- Hover `#222222`
- Radius 4 px
- Padding 12 px 20 px
- Label 16 px, weight 500

### Button Secondary

- Background branco
- Text `#111827`
- Border `#DDE5F2`
- Radius 4 px
- Padding 12 px 20 px

### Button Lime

Use apenas para confirmacao/resultado, nao como CTA universal.

- Background `#A4E244`
- Text `#111827`
- Hover `#91D82E`

### Cards

**Feature Card**

- Background branco
- Border `#DDE5F2`
- Radius 8 px
- Padding 32 px
- Shadow level 1 por padrao, level 2 quando destacado

**Metric Card**

- Fundo azul, navy, verde ou lime dependendo da metrica.
- Numeral grande, label curta, caption operacional.
- Nao usar iconografia decorativa demais.

**Category Cards**

Use cards cheios para representar pilares:

- Rastreamento em tempo real: route blue.
- Controle da frota: fleet green.
- Experiencia do passageiro: passenger purple.
- Demanda e espera: wait orange.
- Auditoria e contratos: contract yellow.

### Navigation

Nav branca em marketing, navy em app/dashboard. Links pequenos, 14 px/500. CTA principal no canto direito.

### Forms

Inputs brancos com borda `#DDE5F2`, radius 4 px e padding 12 px 16 px. Placeholders sempre em `#8A98AE`.

## Application Guidance

### Hero

Estrutura recomendada:

1. Eyebrow: "GESTAO DE TRANSPORTE EM TEMPO REAL"
2. Headline: "Controle sua frota, reduza viagens vazias e prove a qualidade do atendimento."
3. Lead: "Go2Park conecta passageiro, motorista e gestor em uma operacao digital, sem hardware e sem app obrigatorio."
4. CTAs: "Agendar demonstracao" e "Ver funcionalidades"
5. Mockup real do produto, preferencialmente dashboard + celular.

### Secoes Prioritarias

- Problema: desperdicio, reclamacoes, falta de previsibilidade.
- Solucao: mapa ao vivo, WhatsApp, jornada do motorista, dashboard do gestor.
- Resultados: reducao de custos, valorizacao do servico, fidelizacao, seguranca juridica.
- FAQ: hardware, acesso do passageiro, tempo de implementacao.

### Do

- Use screenshots reais do produto como principal recurso visual.
- Use verde-lima para comunicar eficiencia e sucesso.
- Use navy para dar peso B2B e aproximar do dashboard.
- Mantenha botoes retangulares com 4 px de raio.
- Escreva beneficios como operacao, nao como promessa abstrata.

### Don't

- Nao transformar a pagina em um festival de gradientes.
- Nao usar pill CTAs.
- Nao usar verde-lima como cor dominante da pagina.
- Nao esconder o produto atras de ilustracoes genericas.
- Nao usar pesos 700, 800 ou 900 em titulos.
