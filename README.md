# Webpack: Manipulando módulos na sua webapp

![Webpack](https://github.com/andermelo/alura-webpack/blob/master/assets/images/webpack.png)

> Códigos e projetos desenvolvidos durante o curso da [Alura](https://alura.com.br)

## Sumário

1. [Introdução](#introducao)
1. Preparando o build de produção
1. Webpack Dev Server e configuração
1. Tratando arquivos CSS como módulos
1. Importando scripts
1. Boas práticas


## Introdução

> Apesar de o Webpack ser altamente customizável, sua aplicação é voltada para Single Page Applications. Essas páginas que não recarregam durante seu uso tendem a carregar todos os scripts e arquivos CSS que dependem logo no primeiro carregamento e toda mudança de troca de página é feita por um sistema de rotas que manipula a única página carregada trocando seu conteúdo. Para o usuário, essa aplicação se comporta como se fosse uma aplicação nativa, pelo não carregamento durante o uso.

> Por mais fabulosa que essa abordagem possa ser para o usuário, se o escopo da aplicação for grande, o primeiro carregamento será sofrível, primeiro pelo tempo de download de arquivos JS e CSS gigantes (concatenados e minificados) além do tempo para que o interpretador JavaScript realize o parser desses arquivos. Esse problema já não acontece com aplicações web tradicionais, pois cada página carrega os scripts e arquivos CSS de que precisam. Webpack soluciona esse problema das Single Page Applications.