# :checkered_flag: Tributo Fácil

Permite o cálculo e análise de impostos, descontos trabalhistas, dentre outros cálculos tributários que estejam de acordo com a legislação brasileira.

## :technologist: Membros da equipe

- João Antonio Arrais Alcantara-582991
- João Victor Veríssimo Oliveira-579811

## :bulb: Objetivo Geral
    Fornecer ferramentas que possibilitam calcular de forma simples diversos impostos e descontos que estejam sob a legislação brasileira.

## :eyes: Público-Alvo
    Jovens e adultos que tem dificuldade de entender como funcionam os cálculos tributários brasileiros, além de profissionais da área da contabilidade e dos direitos trabalhistas que terão uma ferramenta que poderá facilitar certas situações no trabalho.

## :star2: Impacto Esperado
    Contribuir para o entendimento e benefícios de se ter noção de tais assuntos tributários, bem como automatizar cálculos mais difíceis de serem feitos manualmente para trabalhadores de áreas que englobem o tema.

## :people_holding_hands: Papéis ou tipos de usuário da aplicação

- **Usuário Não Logado:** Acesso rápido à ferramenta para cálculos simples e pontuais que não necessitam de um login
- **Usuário Padrão (Logado):** Trabalhador ou pessoa física que possui conta no sistema, para situações em que é necessário ter dados salvos dentro da ferramenta para usos recorrentes
- **Administrador:** Responsável pela manutenção do sistema, que será necessária com base nas possíveis mudanças nos cálculos que podem vir a acontecer periodicamente.

> Tenha em mente que obrigatoriamente a aplicação deve possuir funcionalidades acessíveis a todos os tipos de usuário e outra funcionalidades restritas a certos tipos de usuários.

## :triangular_flag_on_post:	 Principais funcionalidades da aplicação

**Funcionalidades acessíveis a todos os usuários (Visitantes):**
- Inserção de salário bruto e cálculo instantâneo do desconto de INSS.
- Cálculo de dedução do Imposto de Renda Retido na Fonte (IRPF).
- Simulação do salário líquido final.
- Exibição do extrato detalhado de quais faixas de imposto foram aplicadas.

**Funcionalidades restritas a usuários logados:**
- Criação de conta e autenticação no sistema.
- Cadastro de informações no perfil (número de dependentes, pensão alimentícia, descontos de plano de saúde) para preenchimento automático.
- Histórico de simulações salariais salvas na conta.
- Exportação do resultado do cálculo para PDF.

**Funcionalidades do Administrador:**
- Painel para atualização das tabelas de alíquotas e deduções do INSS e IRPF.

## :spiral_calendar: Entidades ou tabelas do sistema

- **Usuario:** Armazena os dados de acesso e o perfil (id, nome, email, senha, tipo_usuario, numero_dependentes).
- **Simulacao:** Registra o histórico de cálculos feitos pelos usuários logados (id, id_usuario, salario_bruto, valor_inss, valor_irpf, outros_descontos, salario_liquido, data_calculo).
- **TabelaImposto:** Entidade responsável por guardar as faixas de contribuição atualizadas da legislação (id, tipo_imposto, ano_vigencia, faixa_salarial_inicio, faixa_salarial_fim, aliquota, parcela_deduzir).