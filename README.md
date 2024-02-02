# Requisitos-e-Arquiteturas-de-Software
Este Repositório contém informação relativa à Unidade Curricular de Requisitos e Arquiteturas de Software.
O objetivo do trabalho era passar pro todas as fases que envolvem a construção de um Sistema como levantamento de Requisitos, Modelação e implementação.
O trabalho foi desenvolvido por : 

###### PG53951 & João Pedro Vilas Boas Braga
###### PG51636 & Nsimba Teresa Armando
###### PG53791 & Duarte Gonçalves Parente
###### PG50006 & Juliana Ngoma Cesar Silvério
###### PG52672 & André Lucena Ribas Ferreira
###### A94942 & Miguel Velho Raposo
###### A91775 & José Pedro Batista Fonte
###### PG52675 & Carlos Eduardo da Silva Machado
###### PG52693 & Maria Francisca Mendes Lemos
###### A96075 & João Bernardo Teixeira Escudeiro
###### PG54162 & Rafael Picão Ferreira Correia
###### PG54093 & Miguel Ângelo Silva Senra



## Fase 1- Levantamento de Requisitos
A primeira fase do trabalho envolvia tarefas como a identificação dos stakeholders, o levantamento de requisitos e a identificação de restrições e  associados ao projeto, bem como a separação em requisitos funcionais e não funcionais.Em resumo o sistema deve permitir que os professores criem provas de avaliação eque as calendarizem, que os alunos as realizem (de forma devidamente calendarizada) eque essas provas sejam corrigidas, tendencialmente de forma automática.
Os stakeHolders do programa são :

+ Docente
+ Aluno
+ Técnico

Para além do levantamento de requisitos foram também identificados os use cases do sistema.
Os mais relevantes são 

+ Gestão de Provas
+ Agendar Teste
+ Iniciar Prova
+ Finalizar prova
+ Exportar resultados
+ Realizar Prova
+ Consultar Prova
+ Solicitar Reavaliação
+ Testar plataforma
+ Manutenção da Plataforma
+ Classificar Respostas

![Diagrama de Casos de Uso](https://github.com/jbtescudeiro16/Requisitos-e-Arquiteturas-de-Software/raw/main/Photos/Diag%20Use%20Cases.png)


Os use Cases estao descritos pormenorizadamente no relatorio da fase1 na pasta relatorios.
Realizamos também alguns diagramas como modelo de dominio e diagramas de sequencia/ use case , para ajudar a perceber melhor as entidades que estão relacionadas e as relações.
![Modelo Domínio](https://github.com/jbtescudeiro16/Requisitos-e-Arquiteturas-de-Software/raw/main/Photos/dominio.png)

O diagrama de atividades abaixo apresentdo demonstra os estados possíveis de uma prova desde que é criada ate ser corrigida.
![Diagrama de Atividade](https://github.com/jbtescudeiro16/Requisitos-e-Arquiteturas-de-Software/raw/main/Photos/ras-diag-maq-est.png)


## Fase 2- Modelação
Esta fase fornece uma visão geral das metas e objetivos da arquiteturaproposta, destacando a sua relevância no contexto do aprimoramento da experiência educacional
e na eficiência operacional da instituição.
Incialmente e como sugerido pelos docentes, realizamos uma decomposição funcional dos requisitos funcionais em grupos funcionais para que fosse mais fácil identificar os grupos funcionais e os respetivos microserviços.
Foram então identificados os grupos funcionais que estão presentes na figura abaixo.
![Grupos Funcionais](https://github.com/jbtescudeiro16/Requisitos-e-Arquiteturas-de-Software/raw/main/Photos/Functional%20Decomposition.png)

Dados como definidos os grupos funcionais definimos então os microsserviços, unindo alguns grupos funcionais que possuíam características semelhantes .

Após isto construímos diagramas de classes para cada um dos microsserviços, para que fosse possível estruturar através de um paradigma orientado a objetos os microserviços.
Construímos um diagrama de componentes para delinear a estrutura global do nosso sistema.

![Component](https://github.com/jbtescudeiro16/Requisitos-e-Arquiteturas-de-Software/raw/main/Photos/componentes.png)

Por fim realizamos um diagrama de deployment para ajudar a perceber como seria dado o deploy da aplicação e como está construído cada microsserviço.
![Deplyment](https://github.com/jbtescudeiro16/Requisitos-e-Arquiteturas-de-Software/raw/main/Photos/diagrama-deployment-teste.png)


## Fase 3- Implementação
Na terceira fase o objetivo seria implementar a solução baseado na arquitetura definida na fase anterior. Assim decidimos realizar apenas as operações correspondentes ao MVP exigido pelos docentes que continha as seguintes funcionalidades:



Passamos então para a implmentação dos microsserviços, bem como da API GATEWAY responsável por funcionar como ponte entre o Front-End e o Back-End .
Cada microsserviço utilizou a linguagem com a qual estava mais familiarizado.
O Front-End foi realizado em React, e o Back-End em javascript, bem como mongoDB ou java e MYSQL.
De seguida sáo apresentadas algumas fotografias correspondentes ao produto final em execução.
