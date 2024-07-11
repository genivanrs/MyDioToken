# MyDioToken
Curso Feito na Plataforma da Digital Inovation One - DIO

MyDioToken é um token compatível com ERC-20 implementado em Solidity. Este contrato de token inclui funcionalidades básicas, como transferência de tokens, aprovação de permissões e transferência de tokens em nome de outro endereço.

## Descrição

MyDioToken é uma implementação simples do padrão ERC-20. O contrato inclui as seguintes funcionalidades:

- Transferência de tokens
- Aprovação de permissões
- Transferência de tokens de um endereço para outro usando permissões

## Instalação

Para usar o MyDioToken, você precisará dos seguintes softwares instalados:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [Truffle](https://www.trufflesuite.com/truffle)
- [Ganache](https://www.trufflesuite.com/ganache) (para testes locais)

Clone o repositório e instale as dependências:
git clone https://github.com/genivanrs/MyDioToken.git
cd MyDioToken
npm install

## Implantação do Contrato
Inicie o Ganache (para desenvolvimento local):

ganache-cli
Compile e implante o contrato usando Truffle:

truffle compile
truffle migrate
## Interagindo com o Contrato
Você pode interagir com o contrato implantado usando o console Truffle ou qualquer carteira Ethereum (por exemplo, MetaMask).

## Inicie o console Truffle:

truffle console

## Funções

totalSupply(): Retorna o total de tokens emitidos.

balanceOf(address account): Retorna o saldo de uma conta específica.

allowance(address owner, address spender): Retorna o número restante de tokens que o spender poderá gastar em nome do owner.

transfer(address recipient, uint256 amount): Transfere amount tokens para o recipient.

approve(address spender, uint256 amount): Define a quantidade de tokens que o spender está autorizado a gastar em nome do chamador.

transferFrom(address sender, address recipient, uint256 amount): Transfere amount tokens de sender para recipient usando o mecanismo de permissão.

## Eventos
Transfer(address indexed from, address indexed to, uint256 value): Emitido quando value tokens são movidos de uma conta (from) para outra (to).
Approval(address indexed owner, address indexed spender, uint256 value): Emitido quando a permissão de um spender para um owner é definida por uma chamada para approve.


