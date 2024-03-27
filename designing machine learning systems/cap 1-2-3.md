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

Em qualquer projeto de ML é importante escolher o formato certo para onde os obter, onde armazenar os dados usados, e como os processar. Diferentes tipos de dados precisam de diferentes tipos de cuidados, por exemplo os dados inseridos por usuários são perigosos, pois a chance de um usuário passar um dado no formato é grande, isso torna necessário que exista um cuidado maior ao desenvolver aplicações que usem esse tipo de dado. 
Já dados gerados pelo próprio sistema são importantes para conseguir ter informações sobre o desempenho do modelo, além disso é bastante usado para fazer "debug". Devido à natureza de como dados de log funcionam, dois problemas podem ocorrer: saber por onde começar a análise desses dados e onde armazenar esse grande volume de informações.  

Existem também os bancos de dados internos, onde é possível analisar o comportamento dos usuários e a partir disso tentar executar ações previamente e assim agilizar procedimentos mais demorados. Com isso finalmente chegamos

Existem também os bancos de dados internos, onde é possível analisar o comportamento dos usuários e a partir disso tentar executar ações previamente e assim agilizar procedimentos mais demorados. Com isso finalmente chegamos nos dados de first, second e third-party: 

First-party -> São os dados que a própria empresa já coleta sobre seus usuários ou clientes. 

Second-party-> São dados coletados a partir dos clientes de outra empresa, que geralmente os disponibiliza por um preço. 

Third-party -> Os dados são coletados diretamente do público que não são seus clientes diretos. 

Com o avanço da internet e o uso de computadores e smartphones, a coleta de dados de terceiros se tornou mais comum, facil e um modelo de negócio bem lucrativo. No entanto com essa facilidade, veio o problema com a privacidade do usuário. 

O formato no qual os dados são consumidos pode influenciar significativamente a quantidade de espaço necessário para seu armazenamento e, consequentemente, os custos envolvidos nesse processo. Diversos fatores devem ser considerados na escolha do formato de dados ideal, tais como: Legibilidade para humanos, padrões de acesso, e se é baseado em texto ou binário, o que mais uma vez influencia o tamanho de seus arquivos. 

O modelo dos dados vai descrever como os dados são representados, por exemplo em banco de dados são armazenadas as características e propriedades de um dado e como eles se relacionam com outros dados presentes na mesma base de dados. 

Modelo relacional -> Neste modelo, os dados são organizados em relações; cada relação é um conjunto de tuplas. Uma tabela é uma representação visual de uma relação, e cada linha de uma tabela constitui uma tupla. 

Modelo não relacional -> Existem dois tipos principais de modelos não relacionais 
são eles o modelo de documento e o modelo de gráfico.  

O modelo de documento visa usar casos em que os dados vêm em documentos independentes e existe raro relacionamento entre si.  

O modelo grafo vai na direção oposta, visando casos de uso onde os relacionamentos entre itens de dados são comuns. 


Normalmente, existem dois tipos de cargas de trabalho para as quais os bancos de dados são otimizados, processamento transacional e processamento analítico. 

Transacional -> Os bancos de dados transacionais são projetados para processar transações on-line e satisfazer os requisitos de baixa latência e alta disponibilidade. Geralmente os bancos de dados usam ACID (atomicity, consistency, isolation, durability), isso garante uma maior integridade da base de dados. 

Analítico -> Bancos de dados analíticos são projetados com a finalidade serem eficientes com consultas que permitem examinar os dados de diferentes pontos de vista. Chamamos esse tipo de processamento de online analytical processing (OLAP). 

ETL -> Quando dados são extraídos de diferentes fontes, primeiro são transformados no desejado formato antes de serem carregado no destino de destino, como um banco de dados ou um armazém de dados. 

Dentre os estilos mais populares de solicitações usados ​​para passar dados através de redes são REST (representational state transfer) e RPC (remote procedure call). Deles análise detalhada está além do escopo deste livro, mas uma diferença importante é que o REST foi projetado para solicitações em redes, enquanto o RPC “tenta fazer uma solicitação para um serviço de rede remoto é semelhante a chamar uma função ou método em sua linguagem de programação.” 

Já o tipo mais comum de transporte em tempo real é o pubsub, que é curto para publicação-assinatura  e fila de mensagens. No modelo pubsub, qualquer serviço pode publicar sobre diferentes tópicos em transporte em tempo real e qualquer serviço que assinantes de um tópico podem ler todos os eventos desse tópico. 

Existem duas formas de processar dados a primeira é via Batch processing e acontece quando pedaços inteiros de dados são processados em conjunto passando pelos mesmos procedimentos, a segunda é a stream processing e diz respeito ao processamento do dado antes mesmo dele chegar à base de dados, é geralmente usado em dados que mudam com muita frequência. 