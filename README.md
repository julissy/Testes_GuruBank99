## [Projeto GuruBank99](https://www.guru99.com/live-testing-project.html)

Live Manual Testing Project: Online Software Testing Practice (tradução: Projeto de teste manual ao vivo: prática de teste de software on-line) um projeto desenvolvido pela Guru99 que tem duração de 13 dias(iniciado dia 13/04/2023), onde irei receber um e-mail com orientações a cada 24h para trabalhar no desenvolvimento de um sistema bancário. Nesse projeto irei criar e executar casos de teste e aprender sobre o processo de teste real em um ambiente corporativo.

O objetivo dessa prática é aprender como planejar e criar casos de teste para um aplicativo bancário, como testar um serviço da web, como executar casos de teste e relatar bugs, como superar problemas comuns que ocorrem em um projeto.

Este repositório será atualizado no decorrer da prática, acompanhe esse desenvolvimento!

13/04/2023 - O primeiro e-mail já chegou e ele contém o SRS(Especificação de Requisitos de Software) , devo ler o documento, analisar e entender as funcionalidades e começar a planejar a escrita dos casos de teste. Um planejamento bem elaborado otimiza o tempo gasto na execução dos testes.

14/04/2023 - O e-mail contém mockups de algumas telas do projeto e um FAQ com possíveis perguntas que nós ,analistas de teste e qualidade, devemos fazer ao receber um documento como o SRS. A partir desse e-mail já consigo elaborar casos de teste, pois tenho os requisitos técnicos e agora com as telas consigo visualizar o caminho a ser seguido.

15/04/2023 - Revisei as técnicas de caixa-preta e decidi quais utilizar no projeto. Segundo o Syllabus versão 3.1 existem 5 técnicas:

•Particionamento de equivalência

•Análise de valor limite

•Teste de tabela de decisão

•Teste de transição de estado

•Teste de caso de uso

Irei utilizar a Tabela de Decisão e Análise de valor limite,pois consigo visualizar as regras que cada campo deve seguir e elaborar os CT's(casos de teste) sem deixar que algo passe despercebido.

![WhatsApp Image 2023-04-17 at 13 52 34](https://user-images.githubusercontent.com/102709022/232555850-b1098014-a684-41ba-a0ba-cdd431e448c0.jpeg)

Recebi o e-mail, fui informada quais funcionalidades a equipe de desenvolvimento está implementando nessa primeiro versão então posso focar nelas:

Novo cliente,Editar cliente,Excluir cliente

Nova conta,Editar conta,Deletar conta


Mini extrato,Extrato personalizado



16/04/2023 - Iniciei a criação dos CT's. Recebi e-mail contendo o "gabarito" dos casos de teste dessas primeiras funcionalidades que estão sendo desenvolvidas.

Aqui um exemplo de CT's que elaborei para o campo PIN do formulário de Cadastro de novo cliente, utilizei Gherkin. Gherkin é bastante útil pois é um padrão de escrita, que melhora a produtividade pois sabendo utilizar conseguimos otimizar o tempo na escrita dos testes e pode ser utilizado tanto na criação de testes manuais como de testes automatizados. Esquema de Cenário é uma palavra-chave do Gherkin, que informa que esse cenário irá utilizar um conjunto de dados para executar exemplos N vezes descrito em seu escopo. PS: só pode ser utilizado se a saída esperada for a mesma para todos os testes, que no caso abaixo é apresentar a mensagem "Campo inválido", não cadastrar o cliente e não prosseguir para a próxima tela.
![WhatsApp Image 2023-04-17 at 16 05 27](https://user-images.githubusercontent.com/102709022/233801378-a3095bd9-377a-4801-b34e-497cf3227525.jpeg)


17/04/2023 - Recebi E-mail contendo as credenciais para acessar a primeira versão do Sistema e iniciar a execução dos testes nas primeiras funcionalidades que foram desenvolvidas. Utilizarei minha planilha que contém um padrão para documentar os testes executados.

ID: Identificação do Caso de Teste
Critério de aceite: Informa os passos a serem realizados para a execução do teste
Prioridade: Identificação de prioridade para a correção do teste
Severidade: Identificação do nível de severidade do teste para o funcionamento do Sistema
Resultado esperado: Informa o que deve ocorrer após o usuário agir
Resultado obtido: Informa a saída obtida após a execução do teste
Defeito: Descreve o defeito ocorrido caso tenha algum erro.
Status: Informa em qual estado o teste está.


![WhatsApp Image 2023-04-17 at 14 55 24](https://user-images.githubusercontent.com/102709022/232570349-c0520aca-32a4-4894-b641-0b15798dc670.jpeg)

18/04/2023 - Após iniciar a primeira bateria de teste foi verificado que a integração entre os módulos não havia sido feita da maneira correta, isso só foi possivel pois realizei o Teste de sanidade que tem como objetivo determinar se a funcionalidade proposta funciona aproximadamente como esperado. Se o teste de sanidade falhar, a compilação é rejeitada para economizar tempo e custos envolvidos em um teste mais rigoroso. Com isso não dei prosseguindo aos testes e pude focar em começar a adequar os testes para a versão 2.0.

Recebi E-mail contendo as alterações que o cliente pediu no software e o "gabarito" dos testes.

Através desse link você terá acesso a versão 1.0 dos Casos de testes até a funcionalidade Extrato personalizado  [PlanodeTeste_GuruBank99_V1](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V1.xlsx). A versão 1.0 não está totalmente modificada pois a partir do acesso ao sistema pude adaptar os testes, implementarei essas modificações na Versão 2.0. 


19/04/2023 - Realizei as alterações necessárias no plano de teste [PlanodeTeste_GuruBank99_V2](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V2.xlsx) incluindo a funcionalidade consulta de saldo. É possivel verificar que no plano existem testes de **unitário/componente** e testes de **integração**. Recebi a versão 2.0 do sistema e a execução dos testes mostra que algumas falhas foram corrigidas,porém ainda temos falhas. Também é possivel perceber que definiram as mensagens de erro para cada campo, com isso tive que alterar os Casos de teste onde utilizei Esquema de Cenário, os casos de teste para o campo PIN foram alterados. 


![image](https://user-images.githubusercontent.com/102709022/233801575-5df7660f-8cd8-44fe-ab08-234de907998e.png)


![image](https://user-images.githubusercontent.com/102709022/233798283-28998c3a-328e-41e5-8991-176d1c68d3c2.png)


20/04/2023 - A versão 3.0 sairá em 2 dias e todas as funcionalidades serão implementadas, devo começar a preparar Testes de sistema para me certificar que todo o sistema está funcionando corretamente.
As funcionalidades que serão implementadas:

 Gerente:

Alterar a senha,
Depósito,
Cancelamento,
Transferência de fundos,


Cliente:

Consulta de saldo,
Transferência de fundos,
Mini extrato,
Declaração personalizada,
Alterar a senha.

21/04/2023 - Os **testes de sistema** já estão sendo elaborados:



![image](https://user-images.githubusercontent.com/102709022/233757476-7ff00328-b1c8-433d-b455-8aef395589f8.png)

22/04/2023 - A adaptação e modificação dos **testes de sistema** continuam sendo feito, amanhã a Versão 3 do sistema vai ser liberada.

![image](https://user-images.githubusercontent.com/102709022/234442156-9a8e5444-1c70-41c3-acf4-7f868e9f9899.png)


23/04/2023 - Enviaram a Versão 3.0 para a realização dos testes, novas mudanças na documentação(SRS) também foram inseridas para a versão 4 do sistema, testes de API devem ser elaborados para testar se os parâmetros obrigatórios estão sendo respeitados, se o **STATUS CODE** corresponde a response enviada.
Deixo o [PlanodeTeste_GuruBank99_V3](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V3.xlsx) disponivel.  


24/04/2023 - Os testes de API foram elaborados, utilizarei o Postman para a execução dos testes, uma ferramenta poderosa que tem a opção de testes para verificação, as alterações no [PlanodeTeste_GuruBank99_V4](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V4.xlsx) foram realizadas, aguardo a liberação da Versão 4 para iniciar as execuções.

![image](https://user-images.githubusercontent.com/102709022/234446439-470c7238-4830-4aee-88df-cbd5aef113cc.png)



25/04/2023 - Versão 4 liberada e testes executados, algumas falhas permanecem mas posso concluir que minha criatividade e habilidade para planejamento, uso de técnicas, criação de cenários e casos de teste tiveram um ganho imensurável! 
Saio desse projeto mais experiente e pronta para novos desafios!


Se você chegou até aqui, meu muito obrigada por ter tirado um tempinho para acompanhar esse repositório. Deixa uma :star2: caso tenha gostado e tenha se sentido incentivado(a) a realizar essa prática!
Caso precise de alguma ajuda pode entrar em contato comigo.

PS: Por questões de otimização os planos de testes já estão com os casos executados.

PS2: Inclui uma evidência no Plano de teste 4, espero que ao realizar o download ele não esteja desconfigurado.


### Acessar arquivo específico

[Especificação de Requisitos de Software - Partes importantes traduzidas](https://github.com/julissy/Testes_GuruBank99/blob/main/SRS_GuruBank99_Traduzido_Partes_Importantes.pdf)

[Divisão das funcionalidades por prioridade - imagem inicial](https://github.com/julissy/Testes_GuruBank99/blob/main/GuruBank99_Funcionalidades_Prioridades.jpg)


[PlanodeTeste_GuruBank99_V1](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V1.xlsx)


[PlanodeTeste_GuruBank99_V2](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V2.xlsx)


[PlanodeTeste_GuruBank99_V3](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V3.xlsx)


[PlanodeTeste_GuruBank99_V4](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V4.xlsx)
