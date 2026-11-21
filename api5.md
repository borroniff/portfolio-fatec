# SyncDesk (API - 5º Semestre)

<div align="center">
  <img width="800" alt="SyncDesk Banner" src="https://github.com/user-attachments/assets/d8c0d754-5f48-41a9-b6a5-14231dc1c92b" />
</div>

<br>

## 📖 Sobre o Projeto
O **SyncDesk** é um sistema desenvolvido pela **Titus Systems** como parte do projeto de Aprendizagem por Projeto Integrado (API) do 5º Semestre (em parceria com a [Pro4Tech](https://pro4tech.com.br)). A plataforma foi projetada para estruturar o atendimento, a triagem e o escalonamento de demandas entre solicitantes, atendentes e gestores.
O sistema centraliza o suporte ao cliente por meio de um chat estruturado, oferecendo aplicações específicas (**mobile e web**) que otimizam o fluxo de atendimento, garantem o histórico completo das interações e fornecem ferramentas administrativas e dashboards para maior controle da operação.<br>
<br>
🔗 Veja mais em: [https://github.com/Titus-System/SyncDesk](https://github.com/Titus-System/SyncDesk)

## 🎯 O Desafio
Como equipe, nosso desafio foi desenvolver uma solução multiplataforma (mobile e web) que centralizasse o atendimento ao cliente com registro completo de histórico, acompanhamento do ciclo de vida dos chamados (abertura, escalonamento e encerramento) e início de jornada por meio de triagem automatizada.

Como membro do time de desenvolvimento, atuei no desenvolvimento completo da **triagem automatizada**, com o desafio central de criar uma jornada inicial fluida e inteligente para o cliente, garantindo a estruturação eficiente e íntegra dos dados no banco.:
* **Arquitetura de Fluxos:** Mapear todas as possibilidades de interação inicial do solicitante para identificar o problema de forma ágil e sem atritos.
* **Lógica de Estados:** Construir um motor de conversação capaz de interpretar seleções do usuário e conduzir transições precisas no atendimento.
* **Persistência Híbrida:** Integrar o histórico dinâmico das conversas à criação formal de chamados estruturados, conectando bancos de dados distintos.

Confira os protótipos e a demonstração da solução:
* 🖥️ **Demonstração:**
> [https://youtu.be/ucNTISGGgis](https://youtu.be/ucNTISGGgis)

<details>
<summary>📱 <b>Ver Protótipos (App & Web)</b></summary>
<br>
<div align="center">
  <b>Protótipo App</b>
  <table>
    <tr>
      <th> <img width="200" alt="App 1" src="https://github.com/user-attachments/assets/a4428db6-a707-4fac-93b8-59de7b5b0a86" /> </th>
      <th> <img width="200" alt="App 2" src="https://github.com/user-attachments/assets/6b97af6d-a301-4cd0-b24c-20071eab19e4" /> </th>
      <th> <img width="200" alt="App 3" src="https://github.com/user-attachments/assets/09c9e51a-8aae-4737-9f5b-f7f56832a0ed" /> </th>
      <th> <img width="170" alt="App 4" src="https://github.com/user-attachments/assets/bc053dac-d68b-483e-8725-788eb8868b5c" /> </th>
    </tr>
  </table>
  <br>
  <b>Protótipo Web</b>
  <table>
    <tr>
      <th> <img width="280" alt="Web 1" src="https://github.com/user-attachments/assets/717f0d48-5042-4eb6-ab0f-ef78606e9398" /> </th>
      <th> <img width="240" alt="Web 2" src="https://github.com/user-attachments/assets/b853a915-f8f8-435d-bb73-91fc58f9b56d" /> </th>
      <th> <img width="280" alt="Web 3" src="https://github.com/user-attachments/assets/24915f7a-b063-49cc-85dd-9aad2757324c" /> </th>
    </tr>
    <tr>
      <td> <img width="280" alt="Web 4" src="https://github.com/user-attachments/assets/844cbcf6-757b-404f-8fd6-0b49748b8bfd" /> </td>
      <td> <img width="240" alt="Web 5" src="https://github.com/user-attachments/assets/0bacf5ca-990c-455a-aa66-961f1b0a66c2" /> </td>
      <td> <img width="280" alt="Web 6" src="https://github.com/user-attachments/assets/638160ef-fcb5-4f5f-99d8-0336cce50c22" /> </td>
    </tr>
  </table>
</div>
</details>

## 👩‍💻 Minha Atuação
Durante o projeto, atuei diretamente no desenvolvimento do chatbot de triagem automatizada, garantindo a integração entre a experiência do usuário e a arquitetura de dados. Minhas principais responsabilidades incluíram:
* 🗺️ **Concepção e Design de Fluxogramas:** Idealizei a jornada inicial do usuário, mapeando todas as possíveis interações e estruturando os fluxogramas da triagem automatizada para garantir uma identificação rápida do problema logo no primeiro contato.
* ⚙️ **Implementação da Máquina de Estados:** Desenvolvi a inteligência e o motor do chatbot utilizando o conceito de máquina de estados, permitindo processar adequadamente as respostas do usuário (como botões de seleção) e definir com precisão as transições e os próximos passos do atendimento.
* 🗄️ **Modelagem e Integração com Banco de Dados:** Estruturei e apliquei a lógica de persistência de dados do assistente para gravar o histórico completo das conversas, registrando mensagens dinâmicas no **MongoDB** e conectando os resultados da triagem à criação formal de chamados estruturados no **PostgreSQL**.
* 🤝 **Trabalho em Equipe:** Colaborei ativamente nas cerimônias ágeis (Scrum) e no alinhamento técnico entre as frentes de Back-end, Web e Mobile ao longo das Sprints.

<details>
<summary>👀 Visualizar o diagrama do <strong>chatbot</strong></summary>
  
```mermaid
flowchart TD
    A['Olá! Bem vindo ao SyncDesk! Para começarmos, verifiquei no seu cadastro e você possui os seguintes produtos disponíveis para manutenção. Selecione a opção que indica sobre o que você quer falar hoje:<br> 1-Produto A<br> 2-Produto B<br> 3-Produto C<br> 4-Desejo apenas tirar uma dúvida.<br> 5-Desejo uma liberação de acesso no Sync Desk.]
    A -->|1| B
    A -->|2| B
    A -->|3| B[Entendi. Como posso te ajudar hoje em relação ao Produto >produto escolhido< ? <br> 1-O sistema apresenta falhas.<br> 2-Quero solicitar uma nova função.]
    A -->|4| C[Entendi. Selecione, por favor, qual a sua dúvida: <br> 1-Qual o período restante para manutenção dos sistemas que eu já adquiri?<br> 2-Estou com dúvidas sobre como utilizar um dos meus sistemas.<br> 3-Como faço para solicitar um novo sistema?]
    A -->|5| D[Entendi. Por favor, envie uma mensagem respondendo as seguintes perguntas: 1-Essa liberação se refere à um novo perfil ou à edição de um perfil já existente? 2-Qual o email e empresa da pessoa que deve ser cadastrada? 3-Qual o motivo da solicitação? 4-Quais produtos essa pessoa deve ter vinculados à sua conta?]
    B -->|1| F[Por favor, explique da maneira mais detalhada possível o seu problema. Lembre-se: Se a descrição do problema não for clara e/ou faltarem informações, seu chamado poderá ser cancelado pelo time de suporte. Seja específico e detalhista.]
    B -->|2| G[Por favor, explique da maneira mais detalhada possível a nova funcionalidade que deseja. Lembre-se: Se a descrição da função não for clara e/ou faltarem informações, sua solicitação poderá ser cancelada pelo time de analistas. Seja específico e detalhista.]
    C -->|1| X[Verifiquei e esses são os seguintes prazos:<br> Produto A - Até dd/mm/aaaa<br> Produto B - Até dd/mm/aaa<br> Produto C - Até dd/mm/aaaa]
    C -->|2| J[Todos os nossos produtos possuem manual do usuário, onde você pode logar e acessa todas as informações neceesárias para a navegação. Verifique no sistema e tire todas as suas dúvidas por lá.]
    C -->|3| L[Você pode enviar um pedido através do nosso email xxxxx.com]
    D -->|Liberação solicitada| E[Aguarde, sua solicitação foi criada e será atribuída à um de nossos analistas. Você já pode acompanhar o tema pela tela 'Minhas demandas'. Obrigada!]
    L --> H
    F -->|Chamado criado| E
    G -->|Requisição solicitada| E
    X --> H[Ajudo em algo mais?<br> 1-Sim<br> 2-Não]
    J --> H
    H -->|Sim| A
    H -->|Não| I[Atendimento finalizado! Momento de avaliação do atendimento.]
````
</details>

## 💻 Habilidades durante o projeto:
<h3>Hard Skills:</h3>
  <table>
    <tr>
      <th width="300px">Tecnologia / Metodologia</th>
      <th width="100px">Nota</th>
      <th width="200px">Classificação</th>
    </tr>
    <tr>
      <td>Python & FastAPI</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Lógica de Máquina de Estados (Chatbot)</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
    <tr>
      <td>Modelagem NoSQL (MongoDB)</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Banco de Dados Relacional (PostgreSQL)</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>React, TypeScript & Tailwind CSS</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>Mobile (Expo / Flutter)</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
    <tr>
      <td>Docker & Testes (Pytest)</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
    <tr>
      <td>Git / Scrum (Dev. Team)</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
  </table>

<h3>Soft Skills:</h3>
  <table>
    <tr>
      <th width="300px">Habilidade</th>
      <th width="300px">Descrição</th>
    </tr>
    <tr>
      <td>Visão Sistêmica e Arquitetura de Fluxos</td>
      <td>Traduzir regras de negócio de atendimento em fluxogramas claros e estados lógicos sem brechas.</td>
    </tr>
    <tr>
      <td>Integração Multidisciplinar</td>
      <td>Conectar regras de triagem e persistência de dados com as equipes de Front-end Web, Mobile e Back-end.</td>
    </tr>
  </table>
<br>

## 🛠️ Tecnologias Utilizadas
A plataforma foi construída utilizando uma arquitetura moderna voltada para comunicação em tempo real, escalabilidade e multiplataforma:

* **Front-end & Design:** React.js, Vite, TypeScript, JavaScript, HTML5, Tailwind CSS, Figma
* **Mobile:** Expo, Flutter, Android Studio
* **Back-end & Real-time:** Python, FastAPI, Node.js, Socket.io
* **Banco de Dados & Armazenamento:** PostgreSQL, MongoDB, MinIO
* **Infraestrutura, Testes & Monitoramento:** Docker, Pytest, Grafana, Git, GitHub

<div style="display: flex; gap: 10px; margin-top: 15px; flex-wrap: wrap;">
    <img align="center" alt="Python" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg">
    <img align="center" alt="FastAPI" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/fastapi/fastapi-original.svg">
    <img align="center" alt="NodeJS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg">
    <img align="center" alt="React" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg">
    <img align="center" alt="TypeScript" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg">
    <img align="center" alt="Tailwind" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg">
    <img align="center" alt="Flutter" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/flutter/flutter-original.svg">
    <img align="center" alt="PostgreSQL" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-plain.svg">
    <img align="center" alt="MongoDB" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg">
    <img align="center" alt="Docker" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg">
    <img align="center" alt="Grafana" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/grafana/grafana-original.svg">
    <img align="center" alt="Git" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg">
    <img align="center" alt="Figma" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg">
</div>
<br>

## 🌐 Navegação

* 🔛 [Menu principal](https://github.com/borroniff/portfolio-fatec/blob/main/README.md)
* 🔙 [Projeto anterior](https://github.com/borroniff/portfolio-fatec/blob/main/api4.md)
* 🔜 [Próximo projeto](https://github.com/borroniff/portfolio-fatec/blob/main/api6.md)
