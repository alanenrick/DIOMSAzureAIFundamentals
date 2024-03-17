<h1><a href="https://x.gd/6EjAG"><img src="https://x.gd/7iI6U" align= "left" width= "160" alt="Imagem do bootcamp Trabalhando com Machine Learning na Prática no Azure ML"></a>
<font color= "Gray" size= "4"> 
<h1>Desafio de projeto 3</font></font>
<font color= red>
<h1><font size= "6">
Análise de Sentimentos com Language Studio no Azure AI</font></h1>
</font>

<font color= "yellow" size= "2">Objetivo </font>

<font size= 2 color= gray>


<ol>

#### <li>Criar um novo repositório no github com um nome a sua preferência.</li>

#### <li>Criar uma pasta chamada 'inputs' e criar um documento de texto com algumas sentenças</li>

#### <li>Criar um arquivo chamado readme.md , deixar alguns prints que descreva o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo após a IA analisar suas sentenças.</li>

#### <li>Compartilhar conosco([Dio][5]) o link desse repositório através do botão 'entregar projeto'.</li>

</ol>


# <font color= blue> Passo a passo</font>

*Todos os passos e parâmetros a seguir foram baseados nas aulas do projeto e pelo link<sup>**[1][]**</sup> indicado.*

*Mantenhanha  o idioma do **Microsoft Azure** em inglês, pois os nomes dos recursos aparecem diferente quando muda o idioma, pode acabar atrapalhando.*

<ol>

### <li>Acessar o ***[Portal Azure][2]*** e ***[Criar uma conta][4]***.</li>


### <li>Clicar em "**create a resource**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/01.png" width= "900">


### <li>Clicar em "**AI + Machine Learning**", em "**Language service**" clicar em "**Create**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/01.png" width= "900">


### <li>Clicar em "**Continue to create your resource**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/02.png" width= "900">


### <li>Preencher lacunas conforme abaixo e depois clicar em "**Review + create**".</li>

*   **Subscription:** Selecionar sua subscrição do Azure.

*   **Resource group:** Selecionar um recurso existente ou criar um novo.

*   **Region:** East US.

*   **Name:** Escolher um nome único.

*   **Pricing tier:** "Free F0" ou "S", se  "Free F0", não estiver disponível.

*   **By checking this box I acknowledge that I have read and understood all the terms below:** Selecionar.


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/03.png" width= "900">


### <li>Clicar em "**Create**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/04.png" width= "900">


### <li>Aguardar "**Your deployment is complete**" e depois abrir o "[**Portal Language Studio**][3]".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/05.png" width= "900">


### <li>Ao abrir o portal automaticamente aparecerá o formulário. Preencher conforme abaixo e clicar em "**Done**"</li>

*   **Azure directory:** Escolher diretório padrão, ou um de sua preferência.

*   **Azure subscription:** Selecionar sua subscrição do Azure.

*   **Resource type:** "Language".

*   **Resource name:** Selecionar o recurso de linguagem criado anteriormente.(Se não aparecer, aguardar de 05 a 10 min e tentar novamente.).


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/06.png" width= "900">


### <li>Ir em "**Classify text**" e selecionar "**Analyze sentiment and mine opinions**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Imagens/07.png" width= "900">


### <li>Usar um texto com opinião de sua preferência.</li>

#### *   O texto selecionado foi uma opinião da [Mariana Seidel][6] na plataforma da [DIO](https://www.dio.me/). Transcrito no arquivo [.txt](https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Inputs/Input_Depoimento.txt).


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Inputs/Input_Depoimento.png" width= "900">


#### *   Selecionar idioma do texto, colar o texto, marcar a caixa "**I acknowledge...**" e clicar em "**Run**".


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Outputs/Output_Depoimento-01.png" width= "900">


#### *  Em "**Result**" aparecerá o resultado da análise.

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_3/Outputs/Output_Depoimento-02.png" width= "900">


</ol>


# <font color= blue>Links utéis e Fontes de pesquisa</font>

-   [Portal Azure][2], acessado em 15/03/2024 às 19:10.
-   [Portal Language Studio][3], acessado em 15/03/2024 às 19:20.
-   <sup>**1**</sup> Passo a passo ["Analyze reviews in Language Studio"][1], acessado em 15/03/2024 às 19:15.
-   [Depoimento da Mariana Seidel sobre a DIO][6], acessado em 15/03/2024 às 20:30.
 



[1]: https://aka.ms/ai900-text-analysis

[2]: https://portal.azure.com

[3]: https://language.cognitive.azure.com/?azure-portal=true

[4]: https://unicast.com.br/posts/criando-uma-conta-gratuita-no-azure/#:~:text=1.1%20Criando%20sua%20conta%20gratuita,cadastro%20ou%20criar%20uma%20nova.

[5]: https://web.dio.me/lab/analise-de-sentimentos-com-language-studio-no-azure-ai/learning/f6884c74-e7aa-4700-a84b-a3446e0b6d8d

[6]: https://www.linkedin.com/feed/update/urn:li:activity:7052234566513606656/?actorCompanyId=15157373