# AdaTrade (API - 3º Semestre)

<div align="center">
  <img width="800" alt="AdaTrade Banner" src="https://github.com/equipeAdalove/API-SEMESTRE3/raw/Sprint-1/Documenta%C3%A7%C3%A3o/assets/Banner%20-%20projeto.png" />
</div>

<br>

## 📖 Sobre o Projeto
O **AdaTrade** é uma plataforma web focada no monitoramento do comércio exterior dos estados brasileiros, desenvolvida pela **Equipe AdaLove** como parte do projeto de Aprendizagem por Projeto Integrado (API) do 3º Semestre. O objetivo principal do projeto foi criar uma ferramenta interativa com base em dados abertos do Ministério do Desenvolvimento, Indústria, Comércio e Serviços.
O sistema fornece aos tomadores de decisão dados claros e acessíveis, permitindo a identificação de municípios em ascensão, estagnação ou declínio no mercado internacional.

## 🎯 O Desafio
Como equipe, nosso maior desafio foi processar uma base de dados pública massiva e integrá-la a uma interface fluida (Dashboard) que permitisse buscas por código NCM, filtros de período (2014-2024), visualização de mapas de calor e análises de vias de transporte.

Como **Desenvolvedora (Dev Team)** com foco na qualidade dos dados e na experiência do usuário, meu desafio central foi garantir que as informações fornecidas à aplicação fossem precisas e que o usuário final soubesse como extrair o máximo valor da ferramenta:
* **Integridade da Base:** Lidar com arquivos brutos contendo valores nulos, registros duplicados e vias de transporte irrelevantes.
* **Tratamento Analítico:** Aplicar técnicas estatísticas para remover anomalias (outliers) que poderiam distorcer as análises financeiras.
* **Capacitação do Usuário:** Traduzir a complexidade técnica da plataforma em um guia compreensível, garantindo que economistas e gestores pudessem navegar e exportar dados com facilidade.

Confira o vídeo de demonstração da versão final (Sprint IV):
* 🖥️ **Demonstração:**
<div align="center">
  <video src="https://github.com/user-attachments/assets/5b22543a-625d-454c-a67b-ff6f0971a1fb" width="600" controls>
  </video>
</div>

## 👩‍💻 Minha Atuação
Durante o projeto, atuei garantindo a preparação do insumo técnico e a acessibilidade da ferramenta para o usuário. Minhas principais responsabilidades incluíram:
* 🧹 **Limpeza e Tratamento de Dados (Pandas & Google Colab):** Desenvolvi scripts em Python no Google Colab para acessar, limpar e normalizar os arquivos CSV de importação e exportação. Implementei a eliminação de registros irrelevantes (como transporte postal e "em mãos") e apliquei a técnica de Intervalo Interquartil (IQR) para tratar outliers em colunas críticas como peso líquido e valor FOB.
* 📊 **Consolidação para o Backend:** Consolidei as bases limpas em arquivos finais padronizados, estruturando os dados para a persistência no banco de dados relacional PostgreSQL.
* 📘 **Manual do Usuário:** Fui a responsável exclusiva pelo desenvolvimento do manual do usuário, elaborando um guia completo que detalha desde a navegação inicial até funcionalidades avançadas, como a comparação de estados, busca por NCM, visualização de mapas de calor e exportação para Power BI.
* 🤝 **Trabalho em Equipe:** Participei ativamente das metodologias ágeis (Scrum), alinhando as entregas de dados com as necessidades das equipes de Backend e Frontend ao longo das Sprints.

## 💻 Habilidades durante o projeto:
<h3>Hard Skills:</h3>
  <table>
    <tr>
      <th width="300px">Tecnologia / Metodologia</th>
      <th width="100px">Nota</th>
      <th width="200px">Classificação</th>
    </tr>
    <tr>
      <td>Node.js & NestJS (API REST)</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
    <tr>
      <td>Modelagem ORM</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
    <tr>
      <td>Python & Data Prep</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>React & Vite</td>
      <td>★★★☆☆</td>
      <td>Entendi</td>
    </tr>
    <tr>
      <td>TypeScript</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td>HTML5 / CSS3</td>
      <td>★★★★☆</td>
      <td>Sei fazer com ajuda</td>
    </tr>
    <tr>
      <td> Git / Scrum (Dev. Team)</td>
      <td>★★★★★</td>
      <td>Sei fazer com autonomia</td>
    </tr>
  </table>

<h3>Soft Skills:</h3>
  <table>
    <tr>
      <th width="300px">Habilidade</th>
      <th width="200px">Classificação</th>
    </tr>
    <tr>
      <td>Proatividade</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>Trabalho em Equipe</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>Comunicação Assertiva</td>
      <td>★★★★☆</td>
    </tr>
    <tr>
      <td>Organização e Planejamento</td>
      <td>★★★☆☆</td>
    </tr>
    <tr>
      <td>Resiliência</td>
      <td>★★★☆☆</td>
    </tr>
  </table>
<br>

## 🛠️ Tecnologias Utilizadas
A plataforma e a rotina de dados foram construídas utilizando ferramentas modernas focadas em escalabilidade e precisão:

* **Pipeline de Dados:** Python, Pandas, Google Colab, Prophet
* **Frontend:** React.js, Vite, TypeScript, Tailwind CSS
* **Backend:** NestJS, Prisma ORM
* **Banco de Dados:** PostgreSQL, Docker
* **Design e Documentação:** Figma
* **Ferramentas Ágeis e Versionamento:** Git, GitHub

<div style="display: flex; gap: 10px; margin-top: 15px;">
    <img align="center" alt="Python" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg">
    <img align="center" alt="Pandas" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pandas/pandas-original.svg">
    <img align="center" alt="React" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/react/react-original.svg">
    <img align="center" alt="TypeScript" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg">
    <img align="center" alt="Tailwind" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg">
    <img align="center" alt="NestJS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nestjs/nestjs-original.svg">
    <img align="center" alt="PostgreSQL" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-plain.svg">
    <img align="center" alt="Git" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg">
    <img align="center" alt="Figma" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/figma/figma-original.svg">
</div>
