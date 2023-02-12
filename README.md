<h1 align="center">Desafio Lighthouse</h1>
<p align="justify">Este desafio de ciência de dados visa desenvolver a resolução do Desafio proposto pela Indicium no programa Lighthouse. 
As informações e detalhes do Desafio seguem no arquivo de word "[Lighthouse] Desafio Cientista de Dados - Manutenção preventiva". </p>
<p align="justify">
O projeto foi desenvolvido no notebook em python e suas bibliotecas de análises, visualizações e modelagens preditiva.<br>
O modelo criado realiza a predição de falhas em máquinas a partir de variáveis da base dados. <br> 
Ele identifica possíveis falhas através da função 'function_transform_type' armazenada em arquivo pickle, esta função utiliza outras funções e modelos preditivos, também armazenados em arquivos pickle. A função recebe os seguintes dados (descrição no arquivo word): udi product_id, type air_temperature_k, process_temperature_k, rotational_speed_rpm e torque_nm tool_wear_min e retorna o tipo de falha prevista ou sem falha.
</p>

Segue as informações dos arquivos presentes neste repositório:  
* Analise_Modelagem.ipynb - Notebook em python com análises e o desenvolvimento do modelo de machine learning.  

* desafio_manutencao_preditiva_treino.csv - base de dados de treino para analise e treino do modelo.  

* desafio_manutencao_preditiva_teste.csv - base de dados do desafio para realizar a predição.  

* requirements.txt - arquivo com as informações e versões dos pacotes necessários para rodar o projeto.  

* predicted.csv - arquivo com a predição realizada pelo modelo desenvolvido.  

* label_failure.pkl - arquivo com a função que transforma a variável alvo categórica em numérica, e também retorna da variável numérica para a categórica.  

* function_transform_type.pkl - arquivo com a função que transforma a variável categórica "type" em variável binária.  

* detect_failure.pkl - arquivo com o modelo 1 que prevê se a máquina falhará ou não.  

* detect_type_failure.pkl - arquivo com o modelo 2 que a partir das máquinas que foram previstas com falhas prediz qual o tipo da falha.  

* function_failure_prediction.pkl - arquivo com a função que realiza as transformações necessárias nas variáveis e retorna a predição utilizando os modelos 1 e 2.  
