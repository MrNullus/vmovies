# vMovie

vMovie é um webapp desenvolvido com Vue.js que consome a API OMDb (The Open Movie Database). Ele permite que os usuários pesquisem por filmes pelo nome, exibindo uma lista de resultados e possibilitando visualizar detalhes específicos sobre cada filme.

## Funcionalidades principais
- Pesquisa de filmes por título utilizando a OMDb API.
- Exibição de informações detalhadas dos filmes, como ano de lançamento, elenco, sinopse e classificação.
- Interface moderna e responsiva, garantindo uma experiência agradável em diversos dispositivos.

## Pré-requisitos
- Node.js (versão 14 ou superior) instalado.
- Gerenciador de pacotes npm ou yarn.

## Configuração do projeto
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/vmovie.git
   cd vmovie
   ```
2. Instale as dependências:
   ```bash
   npm install
   ```

## Executando o ambiente de desenvolvimento
Para iniciar o servidor de desenvolvimento com recarga automática:
```bash
npm run serve
```
Acesse o aplicativo em [http://localhost:8080](http://localhost:8080).

## Construção para produção
Para compilar o projeto e otimizá-lo para produção:
```bash
npm run build
```
Os arquivos otimizados estarão na pasta `dist/`.

## Configuração da API OMDb
Este projeto utiliza a OMDb API. Para funcionar corretamente, você precisará de uma chave de API válida.
1. Acesse [OMDb API](http://www.omdbapi.com/) e obtenha sua chave de API.
2. Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:
   ```env
   VUE_APP_OMDB_API_KEY=sua-chave-de-api
   ```
3. Certifique-se de que a chave de API está configurada antes de rodar o projeto.

## Tecnologias utilizadas
- Vue.js
- HTML5 e CSS3
- JavaScript (ES6+)
- Fetch API para requisições HTTP

## Personalização
Consulte a [Documentação de Configuração do Vue CLI](https://cli.vuejs.org/config/) para ajustes adicionais na configuração do projeto.

## Contribuindo
Contribuições são bem-vindas! Siga as etapas abaixo para contribuir:
1. Faça um fork do repositório.
2. Crie um branch para sua feature/bugfix: `git checkout -b minha-feature`.
3. Commit suas alterações: `git commit -m 'Minha nova feature'`.
4. Envie seu branch: `git push origin minha-feature`.
5. Abra um pull request no GitHub.

## Licença
Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.

---

**Deploy do Projeto**

**Link do Projeto:** 
