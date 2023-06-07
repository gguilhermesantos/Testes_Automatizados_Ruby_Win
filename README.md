# Teste automatizado de frontend em Ruby

Este projeto tem o intuito de aprender a configurar e desenvolver automação de frontend em Ruby com framework Selenium. Neste repositório contém algumas checagens básicas que serão utilizadas para validar fluxos críticos,. Foram incluidos, testes de API, porém ainda nao desenvolvido.

## Configurações e instalacoes iniciais

### Sistema

Essa automação foi desenvolvida no sistema Windows (Windows 10) e os comandos abaixo podem não específicos para este sistema.

### Baixe o repositório

Faça o download deste [repositório](https://github.com/gguilhermesantos/Testes_Automatizados_Ruby_Win).
ou utilize o comando de clone `git clone https://github.com/gguilhermesantos/Testes_Automatizados_Ruby_Win.git`

### Instale o Google Chrome

A instalação do Google Chrome pode ser realizada através do [site](https://www.google.com/intl/pt-BR/chrome/)

### Instale o Cmder (Opcional)

Caso tenha dificuldade da ultilização do Windows, é possível utilizar esta aplicação para simular comandos de de sistemas Unix.

[Download Cmder](https://cmder.app/).

### Instale o Ruby

Para instalar o Ruby, acesse o site [RubyInstaller](https://rubyinstaller.org/downloads/).

Para baixar utilizando linha de comando, basta utilizar o comando:

`sudo apt-get install ruby-full`

### Cabybara, cucumber e selenium

Faça a instalação dessas bibliotecas:

No arquivo `Gemfile` acrescentar as dependencias utilizadas:

```
source "https://rubygems.org"

gem 'capybara'
gem 'cucumber'
gem 'json'
gem 'rspec
gem 'selenium-webdriver',       '3.4.0'
```

Para baixar as dependências utilize os comandos:

```sh
gem install bundler
bundle install
```

Note que elas foram especificadas no arquivo 'Gemfile.lock'.
Caso dê erro ao instalar as dependências, delete o arquivo 'Gemfile.lock' e repita a operação anterior.

## Rodando o teste

Para rodar o teste, foi criado a seguinte tag `cucumber --tags @nomedoteste`. Dessa forma, basta digitar essa tag na linha de comando que o teste será iniciado automaticamente.

## Observações

A escrita dos passos do arquivo .feature foi feita em Português, porém, por padrão, eles são feitos em Inglês e, para funcionar corretamente, note que o comando `#language: pt` foi inserido no arquivo.

O código foi comentado para melhor entendimento do que está sendo checado em cada etapa.