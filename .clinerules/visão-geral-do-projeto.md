## Breve visão geral
- Este é um conjunto de diretrizes para o projeto de blog "My New Hugo Site", que usa o gerador de sites estáticos Hugo e o tema PaperMod.
- O idioma principal do site é o português do Brasil (pt-BR), conforme especificado no arquivo `hugo.toml`.

## Contexto do projeto
- O projeto é um blog pessoal construído com Hugo.
- A estrutura do projeto segue as convenções do Hugo, com diretórios como `archetypes`, `content`, `layouts`, `static`, e `themes`.
- O tema PaperMod é utilizado como um submódulo Git, o que facilita a manutenção e atualização do tema diretamente do seu repositório original.

## Stack de tecnologia
- **Gerador de Site Estático:** Hugo (a versão mínima recomendada pelo tema é a v0.146.0).
- **Tema:** PaperMod.
- **Linguagem de Conteúdo:** Markdown para as postagens do blog.
- **Linguagem de Template:** Go (templates HTML do Hugo).
- **Estilização:** CSS, com suporte a temas claro e escuro através de variáveis.
- **Busca:** A funcionalidade de busca no lado do cliente é implementada com Fuse.js.

## Fluxo de desenvolvimento
- O conteúdo do blog é criado em arquivos Markdown dentro do diretório `content`.
- A personalização do layout pode ser feita sobrescrevendo os templates do tema no diretório `layouts` na raiz do projeto.
- Para adicionar CSS personalizado, o arquivo `assets/css/extended/blank.css` pode ser usado para que os estilos sejam agrupados com os do tema.
- O deploy do site é automatizado via GitHub Actions para o GitHub Pages, como configurado em `themes/PaperMod/.github/workflows/gh-pages.yml`.

## Boas práticas de codificação
- Manter a estrutura de diretórios padrão do Hugo para organização.
- Utilizar os shortcodes disponíveis no tema PaperMod (como `collapse`, `figure`, `inTextImg`) para enriquecer o conteúdo.
- Seguir as convenções de nomenclatura para arquivos e diretórios.
- Gerenciar traduções e textos da interface através dos arquivos YAML no diretório `i18n`.
