# Screen-Match-v2
![PHP Version](https://img.shields.io/badge/PHP-v^8.5.0-blue?logo=php&labelColor=fff)
![Composer Version](https://img.shields.io/badge/Composer-last-blue?labelColor=ccc&logo=composer&logoColor=blue)
![Docker Version](https://img.shields.io/badge/Docker-last-blue?labelColor=ccc&logo=docker&logoColor=blue)
![Git Version](https://img.shields.io/badge/git-last-red?labelColor=ccc&logo=git&logoColor=red)

## Sumário

- [Sobre o projeto](#sobre-o-projeto)
- [Pré requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Uso do CLI](#uso-do-cli)

## Sobre o projeto
Aplicação PHP CLI para simular a consulta de filmes e séries de uma plataforma de streaming, retornando as seguintes informações:

### Filmes
1 - ID  
2 - Título  
3 - Título original  
4 - Ano de lançamento  
5 - Gêneros  
6 - Duração em minutos  
7 - Nota no IMDB  

### Séries
1 - ID  
2 - Título  
3 - Título original  
4 - Ano de lançamento  
5 - Ano de conclusão  
6 - Gêneros  
7 - Temporadas  
8 - Episódios  
9 - Duração média por episódio  
10 - Nota no IMDB  

## Evolução e Objetivos
O projeto está em fase de refatoração para corrigir e melhorar na aplicação os pilares do paradigma orientado a objetos do projeto original (Screen-Match) presente nesta conta do GitHub e também tornar o uso mais flexível e fácil com o Docker

## Pré requisitos
- Docker

## Instalação
`./screen-match instalar`

## Uso do CLI
| Comando | Descrição | Exemplo |
| :--- | :--- | :--- |
| `listar` | Lista todos os filmes ou todas as séries do banco de dados, conforme o argumento ("filmes", "series", "todos"), com suas informações. | `./screen-match listar filmes` |
| `genero` | Retorna todos os filmes e séries que pertencem ao gênero informado. A busca ignora acentos e diferenças entre maiúsculas e minúsculas ("acao" encontra "Ação"). | `./screen-match genero drama` |
| `obter` | Retorna todas as informações do filme ou da série pesquisado pelo título original ou o atual. A busca deve ser parcial. | `./screen-match obter hunter` |
