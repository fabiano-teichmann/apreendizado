# ETL x ELT
ETL os dados são extraídos transfonado e carregados

ELT Extrai carrega salvando no target de destino, para depois transforma

# Integration runtime
Integration runtime é o cluster onde vai ser rodado a dag. Por padrão o data factory cria um run time que está mais proximo o possível da origem do dado. Para sua execução ser mais rápida o possível tendo as seguintes categorias:

### Self-Hosted

Quando é on premisse 
Executar a atividade de cópia entre um armazenamento de dados de nuvem e um armazenamento de dados na rede privada.
Expedir as seguintes atividades de transformação para recursos de computação na rede virtual local ou do Azure: atividades de Hive do HDInsight (BYOC, Traga Seu Próprio Cluster), de Pig do HDInsight (BYOC), de MapReduce do HDInsight (BYOC), de Spark do HDInsight (BYOC), de Streaming do HDInsight (BYOC), de Batch Execution (clássico) do Estúdio do ML, de Recurso de Atualização do Estúdio do ML (clássico), de Procedimento Armazenado, de U-SQL do Data Lake Analytics, atividade personalizada do .Net (executado no Lote do Azure), atividade de pesquisa e atividade de obtenção de metadados.

### Azure

A Azure provisiona toda a arquitetura 
O Integration Runtime do Azure dá suporte à conexão a armazenamentos de dados e computa serviços com endpoints públicos acessíveis. Habilitando a rede virtual gerenciada, o Azure Integration Runtime dá suporte à conexão para armazenamentos de dados usando o serviço de vínculo privado no ambiente de rede privada. 

### Azure Server Integration Services (SSIS) package in Azure

É entregue como empacotamento 

# Linked services
São as conexões com as diversas fontes de dados, pode ser banco de dados sql, nosql, salesforce, sap arquivos em ftp.

# Dataset
São a fonte de dados, por exemplo uma tabela do banco de dados que foi adicionado ao linked service.
