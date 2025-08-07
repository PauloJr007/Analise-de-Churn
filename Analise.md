# 🔁 Análise de Dados – Churn e Retenção

#### Case Completo proposto pela empresa: [Case_2.pdf](https://af60cd74-0f43-4a22-879f-66da15034211.filesusr.com/ugd/733747_ad50f8ae2c594f4b896928db908c7c2d.pdf)

# Resumo Executivo

### 📌 Resumo do Caso

A empresa enfrentava uma elevada taxa de cancelamento de planos de aluguel de veículos, o que comprometia o crescimento e a sustentabilidade do negócio. Embora o modelo fosse acessível e focado em atender trabalhadores informais, 
cerca de 46% dos cancelamentos estavam ligados a fatores controláveis — como falhas no atendimento, problemas técnicos e experiência do cliente —, enquanto 54% decorriam de fatores externos, 
como dificuldades financeiras e questões pessoais. O desafio era compreender os principais fatores de risco, segmentar os clientes com maior propensão ao churn e desenvolver estratégias com impacto direto na retenção, 
buscando reduzir a taxa em 10% em até 6 meses, mesmo diante de novos concorrentes e aumento da inadimplência.

### 🎯 Objetivos

- Identificar os principais fatores que levam ao cancelamento dos planos de aluguel (churn);
- Classificar os clientes de acordo com o risco de cancelamento, considerando variáveis como região, idade e tempo de contrato;
- Desenvolver estratégias de retenção com foco em reduzir o churn em 10% nos próximos 6 meses;
- Definir a melhor alocação do orçamento disponível (R$ 500.000) para maximizar a retenção;
- Apresentar um plano de ação para enfrentar cenários críticos, como aumento da concorrência e da inadimplência.
--------------------------------------------------------------------------------------------------------------------------
Este relatório apresenta uma análise aprofundada do cancelamento de planos de aluguel de motos na empresa, com o objetivo de **reduzir o churn em 10% nos próximos seis meses**. 
A partir da base de dados fornecida, foram identificadas duas categorias principais de churn: **controlável** (motivado por fatores internos) e **não controlável** (relacionado a fatores externos ou pessoais do cliente).

​A análise focou inicialmente no churn controlável, cujos principais fatores foram:

- Atendimento ao cliente ineficiente
- Qualidade da moto (manutenção e conforto)
- Custo do plano

Com base nesses fatores, foi proposta uma estratégia de retenção centrada em **valor percebido, melhoria da experiência do cliente e fidelização inteligente**, respeitando o orçamento disponível de **R$ 500 mil**. 
As principais ações incluem:

- Reestruturação do atendimento com metas de SLA e respostas personalizadas
- Programa de fidelidade com benefícios práticos (como manutenção garantida, motos preferidas e bônus por tempo de contrato)
- Ofertas segmentadas por região e profissão, priorizando os públicos mais sensíveis ao preço

Diante do **cenário de crise** — com a entrada de uma concorrente com preços 20% mais baixos e aumento de 15% na inadimplência — o plano foi adaptado com foco em:


- Promoções sazonais e comunicações agressivas dos diferenciais da empresa
- Maior ênfase em benefícios não financeiros e curtos prazos de retorno para o cliente
- Ações específicas para inadimplentes, como parcelamentos automatizados, uso de pontos de fidelidade para negociação de dívidas e suspensão temporária de planos sem multa

​A estratégia equilibrada visa preservar a **base de clientes de alto valor**, recuperar inadimplentes com eficiência e manter a competitividade frente ao novo cenário de mercado — com foco em **retenção inteligente e sustentável**.

# 📊 Análises

Foram identificados dois grupos principais de cancelamento:

1. Churn Controlável (46%)
2. Churn Não Controlável (54%)

A distinção entre esses dois grupos é fundamental para a definição de estratégias eficazes que promovam a retenção de clientes e sustentem o crescimento da operação.

**Distribuição dos Motivos de Churn**

<img width="743" height="318" alt="image" src="https://github.com/user-attachments/assets/40fe5153-6197-4771-9b55-cef1f4201f91" />  

#### *Observação sobre faixa etária (Idade)*

A variável **idade** foi considerada na análise tanto dos churns controláveis quanto dos não controláveis. No entanto, **não apresentou influência significativa** sobre os principais motivos de cancelamento.  

Mesmo nos casos de **problemas financeiros** — principal motivo de churn — a distribuição por idade é proporcional ao volume geral de cancelamentos, **sem indicar um grupo etário com maior propensão a um tipo específico de churn**.  

Observa-se que clientes entre **35 e 49 anos** aparecem com maior frequência na base de churn. No entanto, **não é possível afirmar que essa faixa etária tem maior propensão ao cancelamento sem a base comparativa de clientes ativos**. 
Por isso, a variável idade **não foi utilizada como fator explicativo** nas análises desta entrega.  

## Churn Controlável

A análise foca nos três principais fatores diretamente influenciáveis pela empresa, que representam quase 80% do churn controlável:

**1. Atendimento ao Cliente - 29,03%  
2. Qualidade da Moto - 27,19%  
3. Custo do Plano - 23,04%**

As regiões com maior concentração de churn controlável são:

**1. Nordeste (27,33%)  
2. Centro-Oeste (22,67%)  
3. Sudeste (22,67%)**  

Essas três regiões concentram **72,67% dos cancelamentos controláveis**.

<img width="751" height="198" alt="image" src="https://github.com/user-attachments/assets/065e794c-336b-480d-89ca-d466a7da8304" />  

### 1. Atendimento ao Cliente (principal problema)

O atendimento é o motivo mais recorrente de churn nas regiões **Centro-Oeste** e **Sudeste**.

<img width="749" height="220" alt="image" src="https://github.com/user-attachments/assets/560efa2d-4ca0-4c59-9e5a-641155b55d5d" />  

  
**Destaques:**

- Na **região Centro-Oeste**, muitos cancelamentos ocorreram entre **clientes com contratos longos (até 23 meses)**, o que sugere que o problema pode ser recente — é improvável
  que um cliente permaneça por quase dois anos enfrentando atendimento ruim.

- No **Sudeste**, há padrão semelhante com clientes mais antigos, o que também demanda investigação interna.  

**Hipótese levantada:**

_Houve troca na equipe ou sistema de atendimento nessas regiões?_  

<img width="749" height="209" alt="image" src="https://github.com/user-attachments/assets/928198ac-a66f-4e1e-a6b5-46d544ed533c" />  

Além disso, **54,84% dos atendimentos foram classificados como “demoradosˮ ou “muito longosˮ**, o que reforça a percepção negativa. 
Porém, **não está claro se a insatisfação se deve ao tempo de espera ou à falta de solução** — o que reforça a necessidade de uma análise qualitativa complementar.  

<img width="747" height="280" alt="image" src="https://github.com/user-attachments/assets/f8a0893e-18a8-4ea1-bb94-29d3f9f1e9ac" />  

### 2. Qualidade das Motos

Com **27,19%** dos casos, a **qualidade das motos** é o segundo principal fator de churn.

A análise cruzou dados de **profissão dos clientes** e **frequência de manutenção:**

- Os **entregadores de aplicativo** são os mais impactados, com a qualidade da moto sendo o principal motivo de cancelamento.
- Para **mototaxistas**, esse fator é o segundo maior, mas com percentual muito próximo do primeiro.

<img width="748" height="226" alt="image" src="https://github.com/user-attachments/assets/4790a453-8e40-47ed-a574-1eeebcbd8a91" />  

**Hipótese principal:**

_As motos podem não estar preparadas para o ritmo de uso intenso e diversificado desses profissionais — muitos trechos diários, terrenos variados, longas distâncias._  

Nas regiões **Nordeste (40,43%)** e **Sul (60%)**, a qualidade da moto aparece como principal motivo de cancelamento, especialmente entre entregadores.
A análise da **frequência de manutenção** não indicou correlação com os cancelamentos por qualidade. Ou seja, independentemente da manutenção ser mensal, trimestral ou inexistente, **o churn por qualidade da moto persiste**.  

<img width="750" height="426" alt="image" src="https://github.com/user-attachments/assets/fc0ef6f2-464a-49d3-89d3-5b255f30719e" />  

A **sazonalidade** também revela um aumento dos cancelamentos por esse motivo entre **agosto** e **fevereiro**, o que pode indicar **desgaste acumulado, e fortalecer a hipótese**.  

<img width="751" height="299" alt="image" src="https://github.com/user-attachments/assets/52dc25f7-a860-4be3-86e8-3527956ee24e" />

### 3. Custo do Plano

Com **23,04% dos casos**, o custo do plano afeta principalmente os **clientes com até 6 meses de contrato**, que representam cerca de 30% dos cancelamentos.  

<img width="739" height="389" alt="image" src="https://github.com/user-attachments/assets/186cbc93-2359-4745-81b7-1ee8b4a6037a" />

Essa dor é particularmente forte na **região Nordeste**, onde o preço aparece como o segundo maior fator de churn, e especialmente entre **entregadores de aplicativo**.  

<img width="744" height="483" alt="image" src="https://github.com/user-attachments/assets/4b6aec54-77f2-4361-8239-6b923d729a03" />

## Resumo: Churn Controlável

**Principais Motivos**  

<img width="638" height="177" alt="image" src="https://github.com/user-attachments/assets/1ada44d0-bb66-45c3-811b-c36c6d908f3e" />  

**Regiões Críticas**  

1. Nordeste (27,33%)
2. Centro-Oeste (22,67%)
3. Sudeste (22,67%)

Juntas, concentram **72,67% dos cancelamentos controláveis**.  

### Matriz de Risco - Churn

<img width="748" height="445" alt="image" src="https://github.com/user-attachments/assets/0cde3c17-ceb7-4442-bd28-676c82ffa5e5" />  

## Estratégia para Redução do Churn

### Foco Principal

Baseado na análise, os pilares da estratégia são:

1. Atendimento ao Cliente (prioridade 1)
2. Qualidade das Motos (prioridade 2)
3. Custo do Plano / Fatores Financeiros (prioridade 3)  

## Ações Prioritárias

### 1. Atendimento ao Cliente

**Inspiração: Nubank**

- Plataforma integrada de atendimento (modelo Shuffle).
- Comunidade online gamificada (modelo NuCommunity).
- Treinamento contínuo dos atendentes (Xpeers).

### 2. Qualidade das Motos

- Sistema de recomendação de motos por perfil.
- Coleta ativa de feedback técnico.
- Manutenção preventiva direcionada, com base em uso e histórico.

### 3. Custo do Plano / Financeiro

- Expansão do programa de pontos (modelo Localiza).
- Classificação de clientes por níveis (Bronze a Premium).
- Diárias gratuitas com pontos + bônus no 3º e 6º mês.

## Alocação do Orçamento – R$ 500.000

<img width="749" height="229" alt="image" src="https://github.com/user-attachments/assets/dae7be5d-65d3-465e-b44d-0102dce86a93" />  

### Garantia de Impacto:

- Acompanhamento por KPIs mensais (churn, NPS, engajamento).
- Testes A/B para promoções e ações.
- Feedback contínuo dos clientes sobre novas iniciativas.

## Conclusão

A estratégia se concentra nos principais fatores identificados e prioriza intervenções de alto impacto e execução rápida. 
Com a **alocação estratégica do orçamento de R$ 500.000 e monitoramento contínuo**, a empresa pode atingir — ou até superar — a meta de **redução de 10% no churn nos próximos 6 meses**.

# Cenário de Crise

**Situação:**

- Uma nova concorrente entrou no mercado oferecendo aluguel de motos **20% mais barato**.  
- O número de **inadimplentes aumentou 15%** nos últimos dois meses.  

## 1. Ajustes no Plano de Retenção

Diante desse cenário, os pilares da estratégia original se mantêm, mas é necessário adaptá-los com foco em **valor percebido e flexibilidade de pagamento**:

a. **Reforço do Programa de Fidelidade com Benefícios de Curto Prazo**

- Aumentar o foco nos benefícios não financeiros (como motos com manutenção garantida, atendimento rápido, acesso a motos favoritas, etc.).
- Criar promoções sazonais com descontos temporários para clientes ativos, para competir com a concorrente no curto prazo, sem alterar o preço-base.
- Dobrar pontos ou oferecer diárias bônus em meses estratégicos (ex: mês 3 e 6, para desestimular o churn no início do contrato.)

b. **Comunicação mais agressiva sobre diferenciais**

- Mostrar com clareza nas campanhas e canais próprios que a empresa oferece:
  - Atendimento mais eficiente
  - Moto adequada ao perfil do cliente
  - Programa de fidelidade que dá retorno prático
  - Garantia de manutenção e segurança

## 2. Estratégias para Inadimplência

a. **Perfilamento dos inadimplentes**

- Segmentar inadimplentes entre:
  - **Ocasional (1º atraso)**: cliente que ainda pode ser recuperado com abordagens leves.
  - **Recorrente (2+ meses)**: clientes com histórico de risco maior.  
 
b. **Ações para reduzir inadimplência sem comprometer lucratividade**

<img width="740" height="352" alt="image" src="https://github.com/user-attachments/assets/345cf10e-7c02-4460-b94f-908d41571045" />  











​
