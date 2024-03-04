<h1><a href="https://web.dio.me/project/trabalhando-com-machine-learning-na-pratica-no-azure-ml/learning/88f82571-5450-40a9-9f4d-253416f2530e?back=/track/microsoft-azure-ai-fundamentals&tab=undefined&moduleId=undefined"><img src="https://hermes.dio.me/lab_projects/badges/87d332d0-5198-4a2f-b159-38c8c2976954.png" align= "left" width= "180" alt="Imagem do bootcamp Trabalhando com Machine Learning na Prática no Azure ML"></a>
<font color= "Gray" size= "4"> 
<h1>Desafio de projeto 1</font></font>
<font color= red>
<h1><font size= "6">Trabalhando com Machine Learning na Prática no Azure ML</font></h1></h1>
</font>

<font color= "yellow" size= "2">

-   Objetivo
</font>
<font size= 2 color= gray>

1. Criar um novo repositório no github com um nome a sua preferência
2. Criar um modelo de previsão com seus devidos pontos de extremidade configurados
3. Escrever o passo a passo desse processo em um readme.md de como você chegou nessa etapa
4. Salvar nesse repositório o readme.md e o arquivo .json de pontos de extremidade
5. Compartilhar conosco o link desse repositório através do botão 'entregar projeto'


# <font color= blue> Passo a passo</font>
<font color= gray> *Todos os passos e parâmetros a seguir foram baseados nas aulas do projeto e pelo **[link](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)** indicado.*


### 1º- Acessar o ***[Portal Azure](https://portal.azure.com/)***


### 2º- ***[Criar uma conta](https://unicast.com.br/posts/criando-uma-conta-gratuita-no-azure/#:~:text=1.1%20Criando%20sua%20conta%20gratuita,cadastro%20ou%20criar%20uma%20nova.)***, ***[Criar Workspace](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)***, acessar o ***[Estúdio do Machine Learning](https://ml.azure.com/?azure-portal=true)***.


### 3º- Acessar o menu, no canto superior direito.


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-01.png" width= "800">


### 4º- Selecionar a opção "ML automatizado". Em seguida "Novo trabalho de ML automatizado".


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-02.png" width= "800">


### 5º- Preencher parametros como exemplo abaixo e depois clicar em "Avançar".


-   **Nome do trabalho:** mslearn-bike-automl
-   **Nome do experimento:** Seleciona "criar novo"
-   **Novo nome do experimento:** mslearn-bike-rental
-   **Descrição:** Aprendizado de maquina automatizado para previsão de alugue de bicicletas.


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-03.png" width= "800">


### 6º- Selecionar tipo de tarefa como "Regressão", clicar em "Criar" dados, preencher como abaixo e depois clica em "Avançar".


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-04.png" width= "800">


-   **Nome:** aluguel_de_bicicletas
-   **Descrissão:** Dados históricos de aluguel de bicicletas.
-   **Tipo:** Tabular


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-05.png" width= "800">


### 7º- Seleciona a opção "De arquivos da web" e clica em "Avançar".


-   **URL da Web:** [https://aka.ms/bike-rentals](https://aka.ms/bike-rentals)


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-06.0.png" width= "800">


### 8º- Preenche campos conforme abaixo e clica em "Avançar".


-   **Formato de arquivo:** Delimitado
-   **Delimitador:** Vírgula
-   **Codificação:** UTF-8
-   **Cabçalho de coluna:** Somente o primeiro arquivo tem cabeçalhos
-   **Ignorar linhas:** Nenhuma


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-06.1.png" width= "800">


### 9º- Em preencher conforme a seguir e clicar em "Avançar".


-   Seleciona todos exceto "path".


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-06.2.png" width= "800">


### 10º- Revisar se está tudo correto e clica em "criar".


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-07.png" width= "800">


### 11º- Seleciona "aluguel_de_bicicletas" e clica em " Avançar".


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-08.png" width= "800">


### 12º- Preencher como abaixo e clicar em "Exibir definições de configuração adicionais".


-   **Coluna de destino:** Rentals(integer)


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-10.png" width= "800">


### 13º- Preencher e clicar em "Salvar"


-   **Métrica primária:** NormalizedRootMeanSquaredError
-   **Desmarca as três opções.**
-   **Modeslos permitidos:** RandomForest, LightGBM


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-09.png" width= "800">


### 14º- Definir Limites e "Avançar".

-   **Limites:**
    -   **Máximo de avaliações:** 3
    -   **Máximo de avaliações simultâneas:** 3
    -   **Máximo de nós:** 3
    -   **Limite de pontução de métrica:** 0.085
    -   **Tempo limite do experimento(minutos):** 15
    -   **Tempo limite de iteração(minutos):**  15
    -   **Habilitar encerramento antecipado:** Selecionar


-   **Validar e testar:**
    -   **Tipo de validação:** Divisão de validação de treinamento
    -   **Validação de percentual de dados:** 10
    -   **Dados de teste:** Nenhum


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-11.png" width= "800">


### 15º- Preencher conforme abaixo e "Avançar".


-   **Selecione o tipo de computação:** Sem servidor
-   **Tipo de máquina virtual:** CPU
-   **Tipo de máquina virtual:** Dedicado
-   **Tamanho da máquina virtual:** Standard_DS3_V2
-   **Numero de instâncias:** 1


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-12.png" width= "800">


### 16º- Revisar dados e "Enviar trabalho de treinamento"


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-13.png" width= "800">


### 17º- Aguardar status como Concluido.


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-14.png" width= "800">


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-15.png" width= "800">


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-16.png" width= "800">


### 18º- Selecionar "Tarefas(Jobs)", abrir submenu da tarefa e selecionar a tarefa com a tag "<font color= green>Melhor</font>".


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-17.png" width= "800">


### 19º- Selecionar "Modelo", Selecionar "Implantar" e definir o nome como "preveralugueis". 


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-18.png" width= "800">


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-19.png" width= "800">


### 20º- Selecionar "Ponto de extremidade", Selecionar "preveralugueis" e clicar em "testar"


<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-20.png" width= "800">


### 21º- Parâmetros utilizados no teste e o resultado obtido:


-   **Parâmetros:**
```
{
  "Inputs": {
    "data": [
      {
        "day": 15,
        "mnth": 6,
        "year": 2024,
        "season": 2,
        "holiday": 0,
        "weekday": 1,
        "workingday": 1,
        "weathersit": 2,
        "temp": 0.3,
        "atemp": 0.3,
        "hum": 0.3,
        "windspeed": 0.3
      }
    ]
  },
  "GlobalParameters": 1.0
}
```

-    **Resultado:**
```
{
  "Results": [
    387.9179371881571
  ]
}
```

<img src="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_1/Imagens/Desafio_1_passo-21.png" width= "800">


# <font color= blue>Links utéis e Fontes de pesquisa</font>


-   [Portal Azure](https://portal.azure.com)
-   [Estúdio do Machine Learning](https://ml.azure.com/?azure-portal=true)
-   [Fonte de instruções do projeto](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html)<sup><font size= "1,5">(Fornecido pela aula do Bootcamp)</font></sup>. Acessado em 04/03/2024
-   [Todos os Desafios de Projeto.](https://web.dio.me/topics/vamos-resolver-os-desafios-juntos?back=%2Ftrack%2Fmicrosoft-azure-ai-fundamentals&page=1&order=oldest)<sup><font size= "1,5">(Artigo Usado para entender como entregar o projeto)</font></sup>. Acessado em 04/03/2024.
-   [Arquivo .csv com os dados](https://aka.ms/bike-rentals)
-   [Sintaxe básica de gravação e formatação no GitHub](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup><font size= "1,5">(Usado para tirar na edição deste README)</font></sup>. Acessado em 04/03/2024.

