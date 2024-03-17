# Design Machine Learning System

Capítulo 1
----------

Machine Learning ficou mais integrado nas nossas vidas nos últimos 5 anos, podendo estar presentes em diversos âmbitos sejam sociais (comunicação) ou profissional (melhorando a experiencia de usuários). No âmbito profissional, Machine Learning, pode ser usada como uma ferramenta poderosa e multe uso. É possível a utilizar esse recurso em produtos como corretor automático e mecanismo de busca online. 

O Machine Learn é uma abordagem para (1) aprender (2) padrões complexos a partir de (3) dados existentes e usar esses padrões para fazer (4) previsões sobre (5) dados não observados. Levando em consideração o âmbito de desenvolvimento de um produto com base em Machine Learn, é preciso ter consciência das necessidades que cada parte da equipe tem e tentar chegar a um ponto de equilíbrio.  

Também é preciso entender quando utilizar um modelo de Machine Learn, se o problema a ser resolvido é (1) repetitivo, (2) o impacto de predições erradas é baixo, (3) tem uma grande base de dados e (4) os padrões mudam constantemente, esse problema é ideal para ser resolvido usando Machine Learning. 

Por fim existem as características intrínsecas a modelos de Machine Learn, são ele: 
Base de dados -> Na fase de treinamento, a base de dados é limpa e bem organizada. Já na fase de produção, os dados recebidos podem estar desorganizados e geralmente são rotulados de forma incorreta.

Imparcialidade -> Dependendo do tipo de dado que é usado para treinar o modelo de Machine Learn, é possível que o seja desenvolvido um algoritmo enviesado, o que leva a problemas que podem afetar usuários inocentes.

Interpretação de resultados -> É importante para usuários, que lidam com atividades delicadas, compreendam os motivos pelos quais um modelo de Machine Learning toma determinada decisão. Assim, evita-se que pessoas sejam vítimas de um algoritmo enviesado.

Capítulo 2
----------

Além das métricas de Machine Learning, também existem as métricas de negócios. É necessário buscar um equilíbrio entre elas, caso contrário, o projeto de ML pode ter uma vida mais curta do que o esperado. Idealmente, um projeto de ML deve possuir quatro características principais: confiabilidade, escalabilidade, capacidade de manutenção e adaptabilidade.

Confiabilidade -> O sistema deve manter a execução correta na performance desejada, mesmo diante de adversidades como falhas de hardware ou software, e até mesmo erros humanos.

Escalabilidade -> Existem diversas maneiras pelas quais um projeto de ML pode crescer, e devem existir abordagens razoáveis para lidar com esse crescimento. Não se trata apenas de escalar ou desescalar recursos, mas também de gerenciar artefatos. Gerenciar cem modelos é muito diferente de gerenciar um único modelo, demandando toda uma estratégia de administração.

Capacidade de Manutenção-> Para garantir que o projeto possa ser mantido por um período indeterminado, é necessário aderir a certas práticas. Os modelos devem ser claros e reproduzíveis, permitindo que outros colaboradores compreendam e construam sobre o trabalho existente, mesmo na ausência do autor original.

Adaptabilidade -> Para se ajustar às mudanças nos dados e nos requisitos de negócios, o sistema deve possuir capacidade para identificar melhorias no desempenho, permitindo atualizações sem interrupção do serviço.

É importante ter em mente que o desenvolvimento de um sistema de ML é uma tarefa iterativa e, na maioria dos casos, um processo contínuo. Após a implementação, o sistema precisará ser continuamente monitorado e atualizado. O processo de desenvolvimento de um projeto de ML segue um fluxo definido em etapas interconectadas, incluindo o escopo do projeto, a engenharia de dados, o desenvolvimento do modelo de ML, a implantação, o monitoramento, a aprendizagem contínua e a análise de negócios.

Escopo do Projeto -> O projeto inicia com a definição do escopo, estabelecendo metas, objetivos e restrições, além de identificar e envolver as partes interessadas, estimar e alocar recursos.

Engenharia de Dados -> Como a maioria dos modelos de ML aprende com os dados, a engenharia desses dados é fundamental. A partir dos dados brutos, é necessário curar os dados de treinamento através de amostragem e geração de rótulos.

Implantação -> Após o desenvolvimento do modelo, é preciso disponibilizá-lo aos usuários, estando preparado para os desafios que essa ação acarreta.

Monitoramento e Aprendizagem Contínua -> Uma vez em produção, os modelos precisam ser monitorados quanto ao desempenho e adaptados a mudanças nos requisitos.

Análise de Negócios -> O desempenho do modelo deve ser avaliado em relação às metas de negócios, gerando insights que podem ser utilizados para eliminar projetos improdutivos ou definir novos.

Para entender melhor o tipo de modelo de ML a ser utilizado, é necessário compreender o problema e analisar suas necessidades. O tipo de problema determinará o modelo de ML a ser implementado, como classificação versus regressão, classificação binária versus multiclasse, e classificação multiclasse versus multirrótulo.

Classificação versus Regressão -> Os modelos de classificação categorizam os inputs em diferentes classes, enquanto os modelos de regressão geram valores contínuos.

Classificação Binária versus Multiclasse -> Quanto menos classes a classificar, mais simples é o problema. A classificação binária envolve apenas duas classes, enquanto a multiclasse envolve mais de duas.

Classificação Multiclasse versus Multirrótulo -> Na multiclasse, cada exemplo pertence a uma única classe, enquanto na multirrótulo um exemplo pode pertencer a múltiplas classes.

Para aprender, um modelo de ML necessita de uma função objetivo para orientar o processo de aprendizagem, também conhecida como função de perda, cujo objetivo é minimizar a discrepância entre as previsões do modelo e os rótulos verdadeiros, utilizando métricas como RMSE ou entropia cruzada.

Capítulo 3
----------