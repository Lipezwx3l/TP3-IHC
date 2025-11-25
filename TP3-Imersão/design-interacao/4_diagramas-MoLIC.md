# Diagramas MoLIC – Modelagem da Interação

## Visão Geral do Diagrama MoLIC Completo

O diagrama MoLIC modela a interação do usuário com um *sistema de produtividade e estudos*, composto por quatro funcionalidades principais:

1. *Sistema de Login e Acessibilidade*
2. *Técnica Pomodoro* 
3. *Flashcards para Estudos*
4. *Relatórios de Desempenho*

O fluxo inicia com a autenticação do usuário, passa pela configuração de acessibilidade, e então oferece um menu principal com as três ferramentas. Cada ferramenta possui seu próprio fluxo de interação, com cenas específicas e transições bem definidas.

<img width="3015" height="1027" alt="Diagrama sem nome" src="https://github.com/user-attachments/assets/eb4bc1a0-36be-4df3-b882-7cae2eefb208" />

---

### CENA 2: Fluxo de Login e Acessibilidade

*Descrição:* 
Esta cena representa o processo inicial de autenticação e personalização da experiência do usuário. O usuário precisa se identificar no sistema e configurar preferências de acessibilidade antes de acessar as funcionalidades principais.

*Elementos da Cena:*
- *Login:* Tela de autenticação onde usuário escolhe o método de login
- *Habilitar Acessibilidade:* Configuração opcional para adaptar a interface
- *Home:* Tela principal do sistema após autenticação bem-sucedida

*Transições:*
- *U: Entrar no sistema* → Inicia o processo de login
- *U: Identificar conta* → Submissão das credenciais
- *d: Login inválido* → Feedback de erro do sistema
- *U: Prosseguir* → Confirmação das configurações
- *d: Selecionado "não"* → Usuário recusa configuração de acessibilidade

*Papel no Fluxo:*
Esta cena estabelece a identidade do usuário no sistema e personaliza a experiência inicial, garantindo que as configurações de acessibilidade estejam adequadas antes do uso das funcionalidades principais.

<img width="569" height="813" alt="login" src="https://github.com/user-attachments/assets/5820c56d-a1d9-4029-8f1e-89140debb257" />

---

### CENA 2: Menu Principal (Home)

*Descrição:*
A home é o centro de controle do sistema, onde o usuário pode navegar entre as diferentes ferramentas disponíveis. A interface é adaptada conforme as preferências configuradas anteriormente.

*Elementos da Cena:*
- *Home:* Tela principal com opções de ferramentas
- *Executar Ferramenta:* Menu de seleção de funcionalidades

*Transições:*
- *U: Entrar na home* → Acesso à tela principal
- *U: Escolher função* → Início da seleção de ferramenta
- *U: Prosseguir* → Confirmação da ferramenta selecionada
- *U: Alternar escolha* → Volta ao menu de seleção
- *d: Cancelar ferramenta* → Retorno à home

*Papel no Fluxo:*
Atua como hub central, permitindo ao usuário navegar seamlessmente entre as diferentes funcionalidades do sistema mantendo o contexto da sessão.

![home](https://github.com/user-attachments/assets/f5cc3693-004a-4c2a-8e76-c12e4b034aee)

---

### CENA 3: Timer Pomodoro

*Descrição:*
Implementa a técnica Pomodoro para gestão do tempo, permitindo ao usuário definir ciclos de trabalho focado com diferentes durações e acompanhar o progresso.

*Elementos da Cena:*
- *Timer Pomodoro:* Configuração do ciclo de trabalho
- *Exibir contagem regressiva:* Interface do timer em execução
- *Pós-ciclo:* Tela de resultados e recomendações

*Transições:*
- *U: Escolher timer* → Inicia configuração do Pomodoro
- *U: Iniciar ciclo* → Começa a contagem regressiva
- *U: Pausar ciclo* → Interrompe temporariamente o timer
- *U: Finalizar ciclo* → Termina o ciclo antecipadamente
- *d: Ciclo concluído* → Timer finalizado naturalmente
- *d: Total focado* → Exibe métricas de produtividade

*Papel no Fluxo:*
Fornece uma estrutura para sessões de trabalho focado, ajudando o usuário a manter a produtividade através de intervalos regulares e métricas de acompanhamento.

![pomodoro](https://github.com/user-attachments/assets/4ab9f2b5-4a90-464a-a189-3f469101ce8a)

---

### CENA 4: Sistema de Flashcards

*Descrição:*
Sistema de estudo baseado em cartões de memorização, permitindo ao usuário revisar conteúdo de forma eficiente com diferentes categorias e acompanhamento de progresso.

*Elementos da Cena:*
- *Flashcards:* Seleção de baralhos de estudo
- *Exibir cartão:* Visualização individual dos cartões
- *Resultado de estudos:* Feedback do desempenho

*Transições:*
- *U: Usar flashcards* → Acesso ao sistema de estudo
- *U: Mostrar resposta* → Revela o verso do cartão
- *U: Marcar como "Lembrar"* → Classificação positiva
- *U: Marcar como "Errar"* → Classificação negativa
- *d: Próximo cartão* → Avança para o próximo item
- *d: Baralho concluído* → Finaliza a sessão de estudo
- *d: Desempenho do baralho* → Mostra estatísticas

*Papel no Fluxo:*
Facilita o aprendizado ativo e a memorização através de repetição espaçada, com métricas que ajudam o usuário a identificar pontos fracos.

<img width="363" height="643" alt="cards" src="https://github.com/user-attachments/assets/b98ae3d8-646a-424f-835a-ca2eb92b00b3" />

---

### CENA 5: Relatórios de Desempenho

*Descrição:*
Sistema de analytics que consolida e apresenta dados sobre o desempenho do usuário em diferentes métricas de produtividade e estudo.

*Elementos da Cena:*
- *Exibir relatórios:* Visão geral dos dados
- *Detalhamento:* Análise aprofundada por categoria
- *Exibir gráficos:* Visualizações dos dados

*Transições:*
- *U: Ver relatórios* → Acesso ao sistema de relatórios
- *U: Abrir relatório detalhado* → Expande informações específicas
- *U: Prosseguir* → Navegação entre visualizações
- *U: Retornar* → Volta à visão anterior
- *d: Exibir relatório detalhado* → Mostra análise aprofundada

*Papel no Fluxo:*
Fornece insights baseados em dados sobre os hábitos de estudo e produtividade do usuário, permitindo ajustes estratégicos na rotina.

<img width="284" height="578" alt="relatorio" src="https://github.com/user-attachments/assets/27214365-ad3e-42fe-ba70-6327c08d2a3a" />
