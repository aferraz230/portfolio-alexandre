# Portfólio de Alexandre Ferraz

**Aluno:** Alexandre Ferraz  
**Atividade:** Evolução do Portfólio — Agenda 15  
**Curso:** Desenvolvimento de Sistemas

---

## 1. Descrição do projeto

Este projeto consiste no desenvolvimento de um portfólio pessoal para apresentar minha trajetória como estudante de Desenvolvimento de Sistemas, meus conhecimentos em programação e os projetos desenvolvidos durante meus estudos.

O site foi desenvolvido utilizando HTML, CSS, Bootstrap e JavaScript, com um layout responsivo e navegação entre as seções.

O portfólio está organizado nas seguintes seções:

- **Perfil:** apresentação pessoal e identificação do estudante.
- **Habilidades:** apresentação das linguagens e ferramentas estudadas.
- **Projetos:** exibição automática dos repositórios públicos do GitHub.
- **Contato:** acesso ao perfil pessoal no GitHub.

## 2. Tecnologias utilizadas

- **HTML5:** estruturação do conteúdo da página.
- **CSS3:** personalização visual, animações e efeitos.
- **Bootstrap 5.3.3:** construção do layout responsivo, menu, cards e carrossel.
- **JavaScript:** criação dinâmica dos elementos e integração com a API.
- **GitHub REST API:** consulta dos repositórios públicos.
- **Fetch API:** comunicação com a API do GitHub.
- **Devicon:** utilização de ícones das linguagens e tecnologias.

## 3. Links do projeto

- **Perfil GitHub:** https://github.com/aferraz230
- **Repositórios pessoais:** https://github.com/aferraz230?tab=repositories
- **Repositório deste portfólio:** https://github.com/aferraz230/portfolio-alexandre
- **Site publicado no GitHub Pages:** https://aferraz230.github.io/portfolio-alexandre/

## 4. Projetos apresentados

A seção de projetos consulta os repositórios públicos da minha conta GitHub.

Entre os projetos desenvolvidos e documentados estão:

- **consumo-energia:** calculadora em Python que estima o consumo mensal de energia elétrica de um aparelho e o custo aproximado.
- **sistema_compras:** sistema em Python para calcular descontos progressivos conforme o valor da compra.
- **consumo-agua:** programa em Python que classifica o consumo de água de imóveis.
- **pesquisa_opiniao:** pesquisa em Python para registrar respostas e contabilizar opiniões sobre atendimento.
- **controle_niveis_agua:** simulação em Python do monitoramento de um reservatório, utilizando listas, funções e Colorama.
- **Portal_Entretenimento:** página web desenvolvida com HTML e CSS, organizada em seções de entretenimento.
- **meus_sites_favoritos:** página HTML com imagens e links para sites favoritos.

A listagem é dinâmica e pode apresentar outros repositórios públicos da conta, conforme os critérios de filtragem implementados.

## 5. Funcionamento do projeto

O site utiliza o Bootstrap para organizar os elementos e adaptar a apresentação a diferentes tamanhos de tela.

O menu de navegação permite acessar diretamente as seções Perfil, Habilidades, Projetos e Contato.

Na página inicial, foi implementado um carrossel com três banners, que alternam automaticamente a cada cinco segundos, utilizando o componente Carousel do Bootstrap.

A seção de projetos possui integração com a API pública do GitHub. Quando a página é carregada, o JavaScript realiza uma consulta aos repositórios públicos da conta `aferraz230`.

Os dados recebidos são convertidos para JSON, filtrados e utilizados para montar automaticamente os cards dos projetos.

Cada card apresenta:

- Nome do repositório.
- Descrição do projeto.
- Linguagem de programação principal.
- Quantidade de estrelas.
- Link para acessar o repositório original.

Quando ocorre alguma falha na consulta à API, o site apresenta uma mensagem alternativa com acesso ao perfil do GitHub.

## 6. Recurso novo adicionado

### Integração automática com a API pública do GitHub

O principal recurso novo implementado foi a integração do portfólio com a API pública do GitHub.

Diferentemente de uma página convencional, em que os projetos precisariam ser cadastrados manualmente no código HTML, este portfólio consulta diretamente os repositórios públicos da conta e apresenta as informações automaticamente.

Esse recurso permite que novos projetos públicos sejam apresentados no portfólio sem a necessidade de criar manualmente novos cards no HTML.

### Como o recurso foi implementado

A implementação foi realizada utilizando JavaScript e as seguintes etapas:

1. **Configuração do usuário:** definição do nome de usuário do GitHub que será consultado.
2. **Consulta à API:** utilização de `fetch()` para acessar a API REST pública do GitHub.
3. **Programação assíncrona:** utilização de `async/await` para aguardar a resposta da consulta.
4. **Conversão dos dados:** utilização de `resposta.json()` para converter os dados recebidos.
5. **Filtragem:** utilização de `filter()` para excluir repositórios que sejam forks ou estejam vazios.
6. **Ordenação:** utilização de `sort()` para organizar os projetos conforme a data da última atualização.
7. **Criação dos cards:** utilização da função `criarCard()` e dos métodos `document.createElement()` para construir os elementos HTML dinamicamente.
8. **Tratamento de erros:** utilização de `try/catch` para identificar falhas e apresentar uma mensagem alternativa ao visitante.

Dessa forma, a seção de projetos é atualizada conforme os dados disponibilizados pela API do GitHub.

## 7. Recursos visuais adicionais

- **Animação nos cards:** efeito `:hover` com elevação e sombra ao passar o mouse sobre os projetos.
- **Transições CSS:** utilização de `transition` e `transform` para suavizar os efeitos visuais.
- **Carrossel com efeito fade:** utilização da classe `carousel-fade` do Bootstrap.
- **Navegação suave:** utilização de `scroll-behavior: smooth` para melhorar a movimentação entre as seções.
- **Layout responsivo:** utilização do sistema de grid do Bootstrap para adaptar o conteúdo a diferentes dispositivos.

## 8. Estrutura dos arquivos

A organização principal do projeto é:

```text
portfolio/
│
├── index.html
├── README.md
│
└── imagens/
    ├── perfil.png
    ├── slide1.svg
    ├── slide2.svg
    ├── slide3.svg
    ├── projeto1.svg
    ├── projeto2.svg
    └── projeto3.svg
```

O arquivo `index.html` contém a estrutura da página, os estilos CSS e os scripts JavaScript.

A pasta `imagens` armazena os arquivos visuais utilizados no portfólio.

## 9. Como executar o projeto

1. Baixe ou clone o repositório.
2. Abra a pasta do projeto no Visual Studio Code.
3. Abra o arquivo `index.html` utilizando o Live Server ou diretamente no navegador.
4. Mantenha a conexão com a internet ativa para carregar o Bootstrap, o Devicon e consultar a API do GitHub.

## 10. Publicação no GitHub Pages

O projeto está publicado utilizando o GitHub Pages.

- **Endereço do site:** https://aferraz230.github.io/portfolio-alexandre/
- **Repositório:** https://github.com/aferraz230/portfolio-alexandre

Para configurar a publicação:

1. Acesse as configurações do repositório em **Settings**.
2. Entre na opção **Pages**.
3. Selecione **Deploy from a branch**.
4. Escolha a branch `main` e a pasta `/ (root)`.
5. Salve as configurações e aguarde a publicação.

## 11. Observações

A integração utiliza a API pública do GitHub, portanto apresenta somente repositórios públicos.

Repositórios privados não são exibidos. A API também possui limites de requisições para consultas sem autenticação.

---

## 👨‍💻 Autor

**Alexandre Ferraz**

🎓 Estudante de Desenvolvimento de Sistemas.

🚀 Sempre aprendendo e evoluindo na área de tecnologia.

---

💧 Projeto desenvolvido para fins de estudo e aprendizado em programação.
