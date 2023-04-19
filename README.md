## [Projeto GuruBank99](https://www.guru99.com/live-testing-project.html)

Live Manual Testing Project: Online Software Testing Practice (tradução: Projeto de teste manual ao vivo: prática de teste de software on-line) um projeto desenvolvido pela Guru99 que tem duração de 13 dias(iniciado dia 13/04/2023), onde irei receber um e-mail com orientações a cada 24h para trabalhar no desenvolvimento de um sistema bancário. Nesse projeto irei criar e executar casos de teste e aprender sobre o processo de teste real em um ambiente corporativo.

O objetivo dessa prática é aprender como criar casos de teste para um aplicativo bancário, como testar um serviço da web, como executar casos de teste e relatar bugs, como superar problemas comuns que ocorrem em um projeto.

Este repositório será atualizado no decorrer da prática, acompanhe esse desenvolvimento!

13/04/2023 - O primeiro e-mail já chegou e ele contém o SRS(Especificação de Requisitos de Software) , devo ler o documento, analisar e entender as funcionalidades e começar a escrita dos casos de teste.

14/04/2023 - O e-mail contém mockups de algumas telas do projeto e um FAQ com possíveis perguntas que nós ,analistas de teste e qualidade, devemos fazer ao receber um documento como o SRS. A partir desse e-mail já consigo elaborar casos de teste, pois tenho os requisitos técnicos e agora com as telas consigo visualizar o caminho a ser seguido.

15/04/2023 - Revisei as técnicas de caixa-preta e decidir quais utilizar no projeto. Segundo o Syllabus versão 3.1 existem 5 técnicas:

•Particionamento de equivalência
•Análise de valor limite
•Teste de tabela de decisão
•Teste de transição de estado
•Teste de caso de uso

Irei utilizar a Tabela de Decisão,pois consigo visualizar as regras que cada campo deve seguir e elaborar os CT's(casos de teste) sem deixar que algo passe despercebido.

![WhatsApp Image 2023-04-17 at 13 52 34](https://user-images.githubusercontent.com/102709022/232555850-b1098014-a684-41ba-a0ba-cdd431e448c0.jpeg)

Recebi o e-mail, me informaram quais funcionalidades a equipe de desenvolvimento está implementando nessa primeiro versão então posso focar nelas:

Novo cliente,Editar cliente,Excluir cliente

Nova conta,Editar conta,Deletar conta


Mini extrato,Extrato personalizado



16/04/2023 - Iniciei a criação dos CT's. Recebi e-mail contendo o "gabarito" dos casos de teste dessas primeiras funcionalidades que estão sendo desenvolvidas.

Aqui um exemplo de CT's que elaborei para o campo PIN do formulário de Cadastro de novo cliente, utilizei Gherkin. Gherkin é bastante útil pois é um padrão de escrita, melhora a produtividade pois sabendo utilizar conseguimos otimizar o tempo na escrita dos testes e pode ser utilizado tanto na criação de testes manuais como de testes automatizados. Esquema de Cenário é uma palavra-chave do Gherkin, que informa que esse cenário irá utilizar um conjunto de dados para executar exemplos N vezes descrito em seu escopo. PS: só pode ser utilizado se a saída esperada for a mesma para todos os testes, que no caso abaixo é apresentar a mensagem "Campo inválido", não cadastrar o cliente e não prosseguir para a próxima tela.
![image](https://user-images.githubusercontent.com/102709022/232586251-cb3f03cd-a4fc-4c0a-abec-8cb84d7d2586.png)



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


19/04/2023 - Realizei as alterações necessárias no plano de teste incluindo a funcionalidade consulta de saldo. Recebi a versão 2.0 do sistema e a execução dos testes mostra que algumas falhas foram corrigidas,porém ainda temos falhas.








### Acessar arquivo específico

[Especificação de Requisitos de Software - Partes importantes traduzidas](https://github.com/julissy/Testes_GuruBank99/blob/main/SRS_GuruBank99_Traduzido_Partes_Importantes.pdf)

[Divisão das funcionalidades por prioridade - imagem inicial](https://github.com/julissy/Testes_GuruBank99/blob/main/GuruBank99_Funcionalidades_Prioridades.jpg)


[PlanodeTeste_GuruBank99_V1](https://github.com/julissy/Testes_GuruBank99/blob/main/PlanodeTeste_GuruBank99_V1.xlsx)

