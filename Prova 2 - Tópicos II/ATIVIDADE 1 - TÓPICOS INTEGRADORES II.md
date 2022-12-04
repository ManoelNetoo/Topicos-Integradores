# TÓPICOS INTEGRADORES II

ALUNO: MANOEL BELMIRO DA SILVA NETO

MATRÍCULA: 01485731

CURSO: ANÁLISE E DESENVOLVIMENTO DE SISTEMAS

PROFESSOR: DAIVID LEAL


1 – Por que devemos fazer testes automatizados nas aplicações que desenvolvemos?

R = Os testes servem para reduzir o número de erros em um código-fonte, nos testes, o sistema é otimizado com precisão e agilidade, é nessa hora que é possível encontrar bugs, falhas de segurança e qualquer outro problema que prejudique o uso da aplicação. O processo é feito simulando casos de uso reais e avaliando se todas as funcionalidades entregam o que é esperado. Em outras palavras, o teste é o momento e que a equipe avalia se o programa funciona como esperado e se registra pequenos problemas e falhas de segurança.

2 – O que são testes unitários?

R = Basicamente, os testes unitários consistem em verificar o comportamento das menores unidades em sua aplicação. Em linguagens orientadas a objetos isso seria uma classe ou até mesmo um método de uma classe. Os testes unitários precisam funcionar de forma isolada, porque precisam funcionar rapidamente, todo conjunto de testes unitários de uma aplicação precisa funcionar em minutos, de preferência em segundos, é por esse motivo que os testes unitários não podem utilizar nenhum processo ou sistema externo, nenhuma operação de E/S (input/output) de qualquer tipo (banco de dados, rede, console, arquivo) exceto registro de falhas nos testes e talvez a leitura da configuração padrão de alternância de recursos no início de uma execução de testes.

3 – O que são testes automatizados?

R = Os testes automatizados são um tipo de avaliação de código-fonte que tem como base a verificação de várias características de uma aplicação, tudo isso sem a interferência de quem está criando o sistema. É possível identificar bugs e brechas de segurança em alguns instantes, basta criar um número adequado de máquinas virtuais para validar a integridade do código-fonte e identificar como ele responde a vários cenários de uso.

4 – Escolha uma pirâmide de testes e descreva com suas palavras cada secção da pirâmide.

R = Existem algumas divisões diferentes quando se trata da pirâmide de testes, mas vou utilizar a mais comum que é a de Martin Fowler, ela é representada por três níveis principais e um "nível extra".

níveis são:

BASE: Basicamente, nessa camada os testes automatizados de unidade são feitos da mesma forma como já foi explicado anteriormente, mas nessa fase a quantidade de testes precisa ser maior do que as fases acima da pirâmide.

MEIO: Nessa divisão, existe a fase de teste de serviços. Nessa camada, são executados todos os testes considerados a nível de serviço, alguns exemplos de testes que são executados nessa camada são as API's, integração e contrato. Nessa camada, os testes podem ser desenvolvidos e executados tanto pelo desenvolvedor, quanto pelo QA (Quality Assurance).

Utilizando o exemplo de API's, o teste de API está entre a camada de teste unitário e de UI (User Interface) e podem ser automatizados em paralelo com o desenvolvimento. Eles realizam a validação de múltiplos cenários e garantem que o conteúdo do Json de retorno esteja correto.

Já os testes de contrato basicamente têm como objetivo garantir que o conteúdo fornecido não tenha sido modificado. Podemos dizer que tem a finalidade de validar se o contrato acordado foi ou não quebrado. Esse teste deve validar se o schema (coleções de objetos dentro de um determinado banco de dados) permanece o mesmo, garantindo assim a integridade dos dados na comunicação entre client/server. A essência dos testes de contrato não é afirmar a funcionalidade. O que querem alcançar é a verificação da semântica. Se o produtor e o consumidor podem se comunicar com sucesso no ambiente de produção.

TOPO: Nessa camada são feitos os testes automatizados a nível de interface do usuário. Esse tipo de teste simula o comportamento do usuário no sistema. Os testes de alto nível (Que está no topo da pirâmide) é como uma segunda linha de defesa de testes. Se você tiver uma falha em um teste de alto nível, não apenas você tem um bug no seu código funcional, você também tem um teste de unidade que está faltando ou está incorreto. Assim, é aconselhado que antes de corrigir um bug exposto por um teste de alto nível, você deve replicar o bug com um teste de unidade.

MANUAL TESTING: Nessa fase são feitos os testes manuais como exploratórios e de aceite. São executados em menor quantidade comparando com as outras fases de teste.
