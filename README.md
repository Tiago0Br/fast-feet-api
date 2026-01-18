# Fast Feet API

Projeto de API para uma transportadora fictícia. Esse projeto está sendo desenvolvido como um desafio da Formação de Node.js da Rocketseat

## Funcionalidades da aplicação

- A aplicação deve ter dois tipos de usuário, entregador e/ou admin
- Deve ser possível realizar login com CPF e Senha
- Deve ser possível realizar o CRUD dos entregadores
- Deve ser possível realizar o CRUD das encomendas
- Deve ser possível realizar o CRUD dos destinatários
- Deve ser possível marcar uma encomenda como aguardando (Disponível para retirada)
- Deve ser possível retirar uma encomenda
- Deve ser possível marcar uma encomenda como entregue
- Deve ser possível marcar uma encomenda como devolvida
- Deve ser possível listar as encomendas com endereços de entrega próximo ao local do entregador
- Deve ser possível alterar a senha de um usuário
- Deve ser possível listar as entregas de um usuário
- Deve ser possível notificar o destinatário a cada alteração no status da encomenda

## Regras de negócio

- Somente usuário do tipo admin pode realizar operações de CRUD nas encomendas
- Somente usuário do tipo admin pode realizar operações de CRUD dos entregadores
- Somente usuário do tipo admin pode realizar operações de CRUD dos destinatários
- Para marcar uma encomenda como entregue é obrigatório o envio de uma foto
- Somente o entregador que retirou a encomenda pode marcar ela como entregue
- Somente o admin pode alterar a senha de um usuário
- Não deve ser possível um entregador listar as encomendas de outro entregador

## Roadmap

- [ ] Criar os dois tipos de usuário: `admin` e `entregador`
- [ ] Implementar um sistema de login com CPF e Senha
- [ ] Desenvolver o CRUD (Criar, Ler, Atualizar, Deletar) dos entregadores, com acesso restrito a usuários `admin`
- [ ] Desenvolver o CRUD dos destinatários, com acesso restrito a usuários `admin`
- [ ] Desenvolver o CRUD das encomendas, com acesso restrito a usuários `admin`
- [ ] Implementar a funcionalidade para alterar a senha de qualquer usuário, com acesso restrito a usuários `admin`
- [ ] Implementar a funcionalidade para marcar uma encomenda como "aguardando" (disponível para retirada)
- [ ] Implementar a funcionalidade para um entregador registrar a "retirada" de uma encomenda
- [ ] Implementar a funcionalidade para marcar uma encomenda como "entregue", exigindo o envio de uma foto e garantindo que apenas o entregador que a retirou possa fazer a marcação
- [ ] Implementar a funcionalidade para marcar uma encomenda como "devolvida"
- [ ] Desenvolver a listagem de encomendas com endereços próximos à localização do entregador
- [ ] Desenvolver a listagem das entregas de um entregador, garantindo que ele só possa ver as suas próprias
- [ ] Implementar o envio de notificação ao destinatário a cada alteração no status da sua encomenda