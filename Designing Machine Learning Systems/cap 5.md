Neste capítulo, é discutida a importância crítica da engenharia de recursos no desenvolvimento de modelos de aprendizado de máquina (ML). Ele começa citando um artigo de 2014 sobre a previsão de cliques em anúncios no Facebook, que destaca como ter os recursos certos é mais crucial do que técnicas algorítmicas avançadas, como ajuste de hiper parâmetros. A engenharia de recursos é apresentada como uma etapa fundamental que pode impulsionar significativamente o desempenho dos modelos de ML, até mais do que arquiteturas de modelos de última geração. 

Importância da Engenharia de Recursos 

É fundamental investir tempo e esforço na engenharia de recursos, como destaco ao longo deste capítulo. A melhor maneira de aprender sobre isso é através da experiência prática e do estudo de casos de sucesso, como as equipes vencedoras de competições do Kaggle. Além disso, é ressaltado que a engenharia de recursos muitas vezes requer conhecimento especializado do domínio, e todos, mesmo os não engenheiros, devem ser capazes de contribuir para esse processo. 

Identificação das Melhores Práticas 

Ao longo deste capítulo, identifiquei que as melhores práticas para a engenharia de recursos: 

Divisão de Dados por Tempo 

É recomendado dividir os dados por tempo em conjuntos de treinamento, validação e teste, em vez de uma divisão aleatória. Essa abordagem evita vazamentos de dados e garante que o modelo seja testado em condições realistas. 

Oversampling Após a Divisão 

Se houver necessidade de fazer oversampling dos dados, é crucial realizá-lo após a divisão para evitar vazamentos de informações do conjunto de teste para o conjunto de treinamento. 

Escala e Normalização Após a Divisão 

A escala e normalização dos dados devem ser feitas após a divisão, utilizando apenas as estatísticas do conjunto de treinamento, para prevenir vazamentos de dados. 

Uso de Estatísticas do Conjunto de Treinamento 

Ao escalar recursos ou tratar valores ausentes, é fundamental utilizar apenas as estatísticas derivadas do conjunto de treinamento para evitar viés. 

Envolvimento de Especialistas do Domínio 

A colaboração com especialistas do domínio é essencial para identificar e criar recursos úteis, trazendo insights valiosos que melhoram a qualidade dos recursos. 

Rastreamento da Linhagem dos Dados 

Manter um registro de como os dados foram gerados, coletados e processados ajudam a compreender o modelo e diagnosticar problemas. 

Compreensão da Importância dos Recursos 

Saber quais recursos são mais importantes para o modelo ajuda a otimizar e simplificar o modelo, concentrando-se nos aspectos críticos dos dados. 

Uso de Recursos que Generalizam Bem 

Escolher recursos que são propensos a funcionar bem em dados não vistos é crucial para a construção de modelos robustos e generalizáveis. 

Importância das Práticas 

Essas práticas são fundamentais para a criação de modelos de ML mais precisos, robustos e generalizáveis. Ao evitar vazamentos de dados e envolver conhecimento do domínio, os modelos se tornam mais representativos do problema real que estão tentando resolver. Além disso, a atenção à importância e generalização dos recursos ajuda a simplificar os modelos, focando nos aspectos mais críticos dos dados, o que pode levar a melhorias significativas no desempenho do modelo. 

Conclusão 

Em resumo, a engenharia de recursos é uma etapa crucial no desenvolvimento de modelos de ML. A adoção dessas melhores práticas pode aumentar significativamente as chances de sucesso de um projeto de ML. 