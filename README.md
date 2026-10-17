# EJNHUB — landing page

Landing page estática em português para apresentar o EJNHUB. O conteúdo público foi conferido no site da Escola Jovens de Negócios e na tela de login do EJNHUB em 17/10/2026. Os blocos que lembram interfaces são ilustrações conceituais, sem dados reais de usuários. A área interna não foi consultada.

## Executar

```bash
cd /workspace/ejnhub_lp
python3 -m http.server 4173
```

Abra `http://localhost:4173`. Não há dependências de instalação nem etapa de build. Os links de acesso apontam para o login oficial: `https://ejnhub.escolajovensdenegocios.com/login`.

## Referências de identidade visual

- Site EJN: https://escolajovensdenegocios.com/
- Login EJNHUB: https://ejnhub.escolajovensdenegocios.com/login
- A composição de cartões, cantos arredondados, títulos com destaque e contraste de blocos foi inspirada na imagem fornecida pelo solicitante. A paleta foi adaptada ao verde e amarelo da EJN.
- Logo, fotos e fontes locais em `assets/` foram obtidos do site oficial da EJN. Essas imagens pertencem ao Instituto.

## Publicação

Um push na branch `main` executa `.github/workflows/pages.yml`, que envia os arquivos estáticos ao GitHub Pages. O endereço esperado após a ativação do Pages é `https://institutoejn.github.io/ejnhub_lp/`. Os caminhos de CSS, JavaScript e imagens são relativos ao diretório do projeto.

### Ativação inicial do GitHub Pages

O repositório precisa ter o Pages habilitado uma vez em **Settings → Pages → Build and deployment → Source: GitHub Actions**. Depois, reexecute o workflow **Publicar EJNHUB LP no GitHub Pages** em **Actions**. O token padrão de Actions não habilita Pages automaticamente; a configuração inicial exige essa ação de quem administra o repositório.
