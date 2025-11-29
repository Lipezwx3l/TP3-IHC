# Introdução
Nesta seção são apresentadas as telas finais do protótipo do aplicativo Foca & Revisa, destacando sua proposta visual, funcionalidade e alinhamento com princípios de usabilidade, acessibilidade e comunicabilidade.

Lembrando que as telas representam visualmente as funcionalidades do aplicativo, mas apenas a navegação entre telas e a alternância de tema estão funcionando. As demais ações, como iniciar o timer, tocar sons ou salvar metas, são simuladas apenas visualmente, pois ainda não foram implementadas, mas irei explicar as telas como se ja estivessem implementadas todas as funcionalidades.

As interfaces foram desenvolvidas com foco em:

✔ Experiência Intuitiva – o usuário compreende facilmente como interagir com os elementos da tela;

✔ Feedback Visível – o sistema informa estados, ações e progresso (tempo, metas, reprodução de sons, itens salvos);

✔ Acessibilidade Inclusiva – contraste adequado, modo escuro, ícones universais e navegação simplificada;

✔ Coerência Visual – padronização de cores, ícones, tipografia e espaçamento.

# 1. Tela Inicial – Timer Pomodoro
![Imagem do WhatsApp de 2025-11-28 à(s) 22 53 27_160e36cf](https://github.com/user-attachments/assets/bbcd9973-d1e2-4844-8bab-0f7b9055a507)

Figura 1 - Timer Pomodoro,
A tela inicial concentra a principal funcionalidade do app: a técnica Pomodoro para focar nos estudos.
## Elementos principais:


| Elemento                           |         Funcões                      | Justificativa de design                                    |
| ---------------------------------- | ------------------------------------- | ----------------------------------------------------------------------- |
| **Timer circular** com 25:00       | Exibe tempo restante de foco          | Mensagem clara e visual, reforça a contagem e o progresso               |
| **Botão “Iniciar” (vermelho)**     | Inicia visualmente o cronômetro       | Botão com cor de destaque chamando para ação principal (Call-to-Action) |
| **Indicador de Meta (1/10)**       | Mostra metas planejadas e concluídas  | Motivação e gamificação: feedback visual imediato                       |
| **Ícone de menu lateral (☰)**      | Acesso a configurações e outras telas | Reconhecido universalmente, reflete um menu expandível                  |
| **Ícone de troca de tema (☀️/🌙)** | Alterna entre modo claro e escuro     | Recurso de acessibilidade e preferência visual                          |
| **Barra inferior de navegação**    | Alternar entre Início, Sons e Metas   | Facilita navegação; sempre visível e consistente                        |
| **Logo Foca & Revisa**             | Identidade visual do app              | Gera confiança, familiaridade e coesão de marca                         |



# 2. Tela de Sons Ambientais
![Imagem do WhatsApp de 2025-11-28 à(s) 22 53 37_e234684f](https://github.com/user-attachments/assets/d0faa0da-629b-4d81-9931-285413730bc0)

Figura 2 - Tela de Sons,
Tela para registrar e organizar os objetivos de estudo.

| Elemento                                             |            Funções                      | Justificativa de design               |
| ---------------------------------------------------- | --------------------------------------- | ---------------------------------------------------- |
| **Ícone de alto-falante + título “Sons Ambientais”** | Identifica a função da tela             | Comunicação imediata e intuitiva                     |
| **Cards com imagens (fogo, mar, chuva, vento)**      | Representam os tipos de som disponíveis | Uso de metáforas visuais (Design semântico)          |
| **Botão Play ▶** em cada card                        | Simula acionamento do som               | Indica claramente a ação associada a cada card       |
| **Layout em grade (2x2)**                            | Organização dos cards                   | Facilita toque e visualização; evita poluição visual |
| **Barra inferior de navegação**                      | Permite voltar para Início ou Metas     | Consistência de navegação em todas as telas          |

# 3. Tela de Metas e Organização
![Imagem do WhatsApp de 2025-11-28 à(s) 22 53 50_d6118703](https://github.com/user-attachments/assets/129e47ba-1dd6-4c04-9ae9-179f27e762e1)

Figura 3 - Tela de Metas,
Permite registrar, escolher e visualizar metas de estudo do dia

A Tela de Metas tem como objetivo registrar e selecionar as tarefas que o usuário deseja realizar naquele dia, funcionando como um planejador diário. O usuário pode escrever uma meta usando o campo “Fazer uma Atividade”, tocar no botão Adicionar e essa meta passa a aparecer abaixo, na listagem de tarefas.

Nessa lista, o usuário pode marcar quais tarefas ele realmente pretende cumprir no dia (como, por exemplo, Revisar Conteúdo, Estudar Matemática, Preparar Apresentação). Ao clicar em Salvar, as tarefas selecionadas são registradas visualmente como Metas do Dia.

Como isso se conecta com a Tela Inicial (Timer Pomodoro):

Quando o usuário marca uma tarefa como meta (exemplo: Revisar Conteúdo) e salva, ela passa a ser considerada uma meta ativa do dia;

Na Tela Inicial, essa meta aparece no contador de progresso como 1/10, indicando que uma meta foi definida;

Se o usuário selecionar três metas na tela de tarefas, a Tela Inicial passa a exibir 3/10;

O sistema permite um limite máximo de 10 metas por dia, ajudando a manter organização sem sobrecarregar o usuário.


