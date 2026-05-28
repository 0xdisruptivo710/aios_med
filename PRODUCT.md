# Product

## Register

brand

## Users

Donos e donas de clínicas médicas brasileiras — médicos-proprietários, tipicamente entre 40 e 65 anos, que decidem a compra pelo bolso e pela agenda. Falam "fatura", "cadeira vazia", "no-show", "agenda cheia". Tempo escasso, tolerância zero a hype, ceticismo alto com promessas de "IA mágica". Operam clínicas que vão de consultório solo até multi-unidade.

Contexto de uso da landing: chegam por indicação, por anúncio de Instagram, ou por busca direta. Lêem em mobile no intervalo entre pacientes, ou no desktop após uma reunião com o gestor. Tomam decisão de "vale a conversa?" em menos de 90 segundos.

A "job to be done" não é "comprar um software" — é **resolver duas dores específicas: a cadeira vazia (no-show) e o lead que não vira paciente** (WhatsApp ignorado, follow-up que ninguém faz). Tudo o mais é argumento de apoio.

## Product Purpose

O AIOS é a infraestrutura de captação e retenção de pacientes para clínicas brasileiras: CRM com Kanban automático, agente IA que responde, qualifica e agenda no WhatsApp 24/7, e — o ponto que ninguém copia — um gestor de CRM humano dedicado, somado a time dev e especialistas em IA, embutidos no preço. O cliente não compra software, compra um time inteiro com uma máquina que não dorme.

Sucesso na landing: o dono da clínica termina o scroll sentindo **alívio**, não excitação. Marca um diagnóstico gratuito ou pede demo sem precisar pensar muito sobre isso.

## Brand Personality

Três palavras-objeto: **calmo, clínico, criterioso**.

A sensação de referência é clínica privada suíça cruzada com recepção de spa médico de alto padrão — branco ósseo, materiais discretos, tipografia respirada, ausência total de pressa visual. Voz: técnica sem ser tech-bro, confiante sem precisar gritar, generosa em espaço e em prova, parcimoniosa em adjetivo.

Tom de voz proibido: imperativo de vendas ("Multiplique!", "Transforme!", "Eleve!"), "next-gen", "revolucionário", urgência fake, exclamações.

Tom de voz alvo: afirmação seca seguida de evidência. *"+340 clínicas operando."* *"−68% no-show."* *"Seu gestor de CRM dedicado responde em até 15 minutos."*

## Anti-references

O AIOS não pode parecer:

- **SaaS genérico PT-BR.** HubSpot, RD Station, Pipedrive, Bling, Conta Azul. Hero centralizado, ilustração flat de pessoas felizes, três cards `ícone + título + parágrafo` lado a lado, gradiente roxo-azul. Sem exceção.
- **Pharma / clínica genérica.** Azul-pharma (#0066CC e variantes), gradiente branco-azul, foto stock de médico-de-jaleco-sorrindo, cruz vermelha em qualquer lugar, ícones arredondados de coração ou estetoscópio. É o look de site de plano de saúde dos anos 2010.
- **Tech-bro IA genérica.** Gradiente roxo, neon glow, mascote 3D de robô, blob mesh animado, lila/purple slop de IA 2024-2026. "Unleash your clinic's potential" e variações.
- **Linear-clone literal.** Dashboard-mockup-flutuando-no-vácuo com gradiente cinza-cyan idêntico ao Linear. A inspiração está permitida; a cópia, não.
- **Editorial-magazine pastiche.** Itálico Fraunces gigante, drop cap, broadsheet grid, mono uppercase pequeno em tudo. Não é a voz.

## Design Principles

1. **Alívio sobre hype.** Médico-proprietário decide pelo alívio sentido, não pelo argumento lido. Números são evidência fria, nunca slogan. Toda copy passa pelo filtro: "isto soa como promessa ou como fato?"
2. **Mostre, não fale.** Mockup real, dashboard real, conversa de WhatsApp real. Toda promessa precisa ter um print que a prove. Verbos abstratos ("revolucione", "transforme", "potencialize") são banidos.
3. **Densidade respirada.** Um pensamento por seção. O espaço entre seções é parte da mensagem, não decoração. Médico de 55 não quer cockpit; quer ler sem esforço.
4. **Humano + máquina, nessa ordem.** O diferencial competitivo do AIOS não é "ter IA" — é "ter gestor CRM humano + time dev + especialistas IA + agente 24/7". Toda peça lembra essa composição: pessoas sérias na frente, máquina que não dorme atrás.
5. **Calmaria sobre confiança-tech.** A identidade visual (Bricolage Grotesque, cyan, warm-black) fica preservada, mas cada micro-decisão pende para o lado clínico-criterioso, não para o lado tech-bro: accent menos saturado, padding mais generoso, motion mais lento e mais raro, hierarquia conduzida por peso e espaço antes de cor.

## Accessibility & Inclusion

- **WCAG 2.2 AA mínimo, AAA preferencial para texto principal.** Audiência primária tem 40-65 anos e lê em condições variáveis (consultório com fluorescente, mobile na rua). Cinzas decorativos devem ser auditados — `text-muted` deve manter contraste ≥ 4.5:1 contra `background`, idealmente 7:1 em parágrafos.
- **Body type ≥ 16px, lead ≥ 18px.** Sem "elegante 14px" em parágrafos de venda.
- **`prefers-reduced-motion`** respeitado em todas as animações: marquee, fade-in-up, pulse-soft. Fallback é o estado final estático, nunca remoção de conteúdo.
- **Foco visível** em todos os CTAs com `:focus-visible` (2px solid `accent`, offset 2px). Médico-proprietário pode estar navegando por teclado em desktop após um turno cirúrgico.
- **Linguagem em PT-BR sem jargão técnico.** "Webhook", "API", "n8n" só aparecem em seções de integração técnica claramente marcadas. No hero e no funil de vendas, falamos "agenda", "paciente", "agendamento", "follow-up", "cobrança".
- **Mobile-first verificado.** A landing é frequentemente lida em mobile no intervalo entre consultas; testes em viewport ≤ 390px são obrigatórios antes de qualquer release.
