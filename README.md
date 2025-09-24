Sistema Bancário Otimizado em Python

Este projeto consiste na refatoração e otimização de um sistema bancário simples desenvolvido em Python. O objetivo principal foi aprimorar a estrutura do código, modularizando as operações bancárias e adicionando funcionalidades de gerenciamento de clientes e contas correntes, tornando o sistema mais organizado, eficiente e de fácil manutenção.

Funcionalidades

O sistema bancário otimizado oferece as seguintes operações:

•
Depositar (d): Permite ao usuário realizar depósitos em sua conta, aumentando o saldo.

•
Sacar (s): Permite ao usuário realizar saques, respeitando limites de valor por operação e um número máximo de saques diários, além de verificar o saldo disponível.

•
Extrato (e): Exibe o histórico de todas as movimentações (depósitos e saques) e o saldo atual da conta.

•
Novo Usuário (nu): Permite cadastrar um novo cliente no sistema, solicitando CPF, nome completo, data de nascimento e endereço. Garante que não haja CPFs duplicados.

•
Nova Conta (nc): Permite criar uma nova conta corrente e vinculá-la a um usuário existente através do CPF. Cada conta recebe um número sequencial e é associada à agência padrão (0001).

•
Listar Contas (lc): Exibe todas as contas correntes cadastradas no sistema, mostrando agência, número da conta e nome do titular.

•
Sair (q): Encerra a execução do programa.

Como Usar

Para executar o sistema bancário, siga os passos abaixo:

1.
Certifique-se de ter o Python 3.x instalado em sua máquina.

2.
Salve o código fornecido como banco_otimizado.py.

3.
Abra um terminal ou prompt de comando na pasta onde o arquivo foi salvo.

4.
Execute o script Python com o comando:

5.
O menu de opções será exibido. Digite a letra correspondente à operação desejada e siga as instruções.

Estrutura do Código

O código foi refatorado para utilizar funções, o que melhora a organização e a reutilização. As principais funções são:

•
depositar(saldo, valor, extrato): Gerencia a operação de depósito.

•
sacar(saldo, valor, extrato, limite, numero_saques, limite_saques): Gerencia a operação de saque.

•
exibir_extrato(saldo, extrato): Exibe o extrato da conta.

•
criar_usuario(usuarios): Responsável pelo cadastro de novos usuários.

•
filtrar_usuario(cpf, usuarios): Função auxiliar para buscar um usuário pelo CPF.

•
criar_conta_corrente(agencia, numero_conta, usuarios, contas): Cria e vincula uma nova conta a um usuário.

•
listar_contas(contas): Lista todas as contas cadastradas.

As variáveis globais saldo, limite, extrato, numero_saques, LIMITE_SAQUES, AGENCIA, usuarios e contas são utilizadas para manter o estado do sistema.

Melhorias em Relação ao Código Original

•
Modularização: As operações foram encapsuladas em funções, tornando o código mais legível e fácil de manter.

•
Reutilização: As funções podem ser facilmente reutilizadas em outras partes do sistema ou em projetos futuros.

•
Gerenciamento de Clientes: Adição de um sistema para cadastrar usuários com CPF, nome, data de nascimento e endereço.

•
Gerenciamento de Contas: Implementação da criação de contas correntes vinculadas a usuários, com agência e número de conta.

•
Validação de CPF: Prevenção de cadastro de usuários com CPFs duplicados.

•
Listagem de Contas: Funcionalidade para visualizar todas as contas e seus titulares.

Este projeto demonstra a aplicação de boas práticas de programação para construir um sistema bancário mais robusto e escalável.

