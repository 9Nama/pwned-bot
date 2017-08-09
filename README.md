# PWNED-Bot 🤖

Ola eu sou o bot de exemplo da nama, aqui você aprende sobre webhook e como ligar eles em seus bots, se ainda não tem acesso ao nosso beta, entre em [nama.ai](http://www.nama.ai/beta), para começar precisamos de algumas coisinhas:

-- Ruby 2.2.2

Clone este projeto e siga os passos abaixo:

- Renomeie o arquivo .env-default para .env e substitua pelas suas configurações (se você não tem acesso ao beta e as keys, peça o seu [aqui](http://www.nama.ai/beta) )

-  Execute a instalação do bundler e das dependências do projeto:

```
$ gem install bundler
$ bundle install
```

### Comandos básicos:

- preparar zip do bot e enviar para a pasta compartilhada 
```
$ bundle exec ruby scripts/zip_bot.rb prepare
```
- atualizar intenções e preparar treinamento
```
$ bundle exec ruby scripts/intent_manager.rb update_and_train
```
- atualizar e associar as entidades
```
$ bundle exec ruby scripts/entities_manager.rb update_and_associate
```
### Ferramentas de debug:

- debugar intenções
```
$ bundle exec ruby scripts/intent_manager.rb predict
> im.predict "texto a ser testado"
```
- debugar entidades
```
$ bundle exec ruby scripts/entities_manager.rb parse INTENT_ASSOCIADA "TEXTO A SER TESTADO"
```
