<h1><a href="https://web.dio.me/lab/reconhecimento-facial-com-azure-ml-transformando-imagens-em-dadosa-no-azure-ml/learning/b643df31-5345-4fb4-9be4-478fe43a93e4"><img src="https://hermes.dio.me/lab_projects/badges/f38a62b8-2880-4fd2-82ff-ba263ce97cdb.png" align= "left" width= "160" alt="Imagem do bootcamp Trabalhando com Machine Learning na Prática no Azure ML"></a>
<font color= "Gray" size= "4"> 
<h1>Desafio de projeto 2</font></font>
<font color= red>
<h1><font size= "6">
Reconhecimento Facial e transformação de imagens em Dados no Azure ML</font></h1>
</font>

<font color= "yellow" size= "2">Objetivo </font>

<font size= 2 color= gray>

1. Criar um novo repositório no github com um nome a sua preferência.
2. Criar uma pasta chamada 'inputs' e salvar as imagens que você utilizou.
3. Criar uma pasta chamado 'output' e salvar os resultados de reconhecimento de texto nessas imagens.
4. Criar um arquivo chamado readme.md , deixar alguns prints, descrever o processo, alguns insights e possibilidades que você aprendeu durante o conteúdo.
5. Compartilhar conosco([Dio][]) o link desse repositório através do botão 'entregar projeto'.


# <font color= blue> Passo a passo</font>

*Todos os passos e parâmetros a seguir foram baseados nas aulas do projeto e pelos links<sup>**[1][],[2][],[3][]**</sup> indicados.*
*Mantenhanha  o idioma do **Microsoft Azure** em inglês, pois os nomes dos recursos aparecem diferente quando muda o idioma, pode acabar atrapalhando.*

<ol>

### <li>Acessar o ***[Portal Azure][]*** e ***[Criar uma conta][6]***.</li>


### <li>Clicar em "**create a resource**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/01.png" width= "800">


### <li>CLicar em "**AI + Machine Learning**", em "**Azure AI Services**" clicar em "**create**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/02.png" width= "800">


### <li>Preencher lacunas e clicar em "**Review + create**" e depois em "**create**".</li>
#### -   **Subscription:** Selecione a sua.
#### -   **Resource group:** selecione uma existente ou crie um novo.
#### -   **Region:** East US.
#### -   **Name:** crie um novo.
#### -   **Pricing tier:** Standard S0.
#### -   **By checking this box I acknowledge that I have read and understood all the terms below:** selecionar.

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/03.png" width= "800">


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/04.png" width= "800">


### <li>Acessar [Portal Vision Studio][], clicar em "**View all resources**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/05.png" width= "800">


### <li>Selecionar o recurso criado e clicar em "**Select as default resource**" e retorne a pagina principal.</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/06.png" width= "800">



## <li>[Detectar faces em uma imagem<sup>1</sup>][1] </li>

<ol>

### <li>Clicar em "**Face**" e em "**Detect faces in an image**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/07.png" width= "800">


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/08.png" width= "800">


### <li>Testar com uma imagem padrão</li>

#### -   **I acknowledge...**: Selecionar.
#### -   Clicar em uma imagem padrão.
#### -   Se em "**Detected attributes**" aparecer o resultado, pular para o "_passo 7.3_".

<img src= "https://raw.gith
ubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/09.png" width= "800">


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/10.png" width= "800">

#### -    Se retornar um erro como na imagem acima, seguir próximos passos:

<ol>

#### -  Retornar para página principal.
#### -  Clicar em "**View all resources**".

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/11.png" width= "800">

#### -  Expandir menu ao lado da barra de pesquisa e clicar em "**Create a new resource**".
<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/12.png" width= "800">

#### - Preencher lacunas e clicar em "**Create resource**". Após criar recusro, selecionar e definir como padrão(igual ao _passo 6_).

<ol>

##### <li>**Name:** Criar um nome.</li>
##### <li>**Subscription:** Selecionar a sua.</li>
##### <li>**Resource group:** Selecione um existente.</li>
##### <li>**Location:** East Us.</li>
##### <li>**Price tier:** S0.</li>
</ol>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/13.png" width= "800">

#### - Ir em "**Face**", "**Detecte face in an image**" e testar novamente.(Se der erro novamente feche o navegador, aguarde um tempo e abra o Azure novamente.).

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/14.png" width= "800">
</ol>


### <li>Após testar clicar em "**Browse for a file**" selecionar uma imagem de sua preferência.</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/14.png" width= "800">

#### - A imagem selecionada foi da "[Grande Família][4]".  
<font size= "1">_Observa-se que foram detectadas 12 faces, incluindo a que está no porta retrato._</font>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/output/output-face-grandefamilia.png" width= "800">

</ol>

## <li>[Extrair texto de uma imagem<sup>2</sup>][2] </li>

<ol>

### <li>Na tela principal clicar em "**Optical character recognition**" e em "**Extract text from images**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/15.png" width= "800">

### <li>Selecionar uma imagem padrão e testar. </li>
<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/16.png" width= "800">


### <li>Após testar clicar em "**Browse for a file**" selecionar uma imagem de sua preferência.</li>

#### A imagem selecionada foi com o texto de "[João 8:32][5]"
<font size= "1">_Observa-se que foram detectado todos os textos de forma correta, exceto o "@" que foi detectado como "O"._</font>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/output/output-text-joao832.png" width= "800">

</ol>


## <li>[Criando legenda para uma imagem<sup>3</sup>][3] </li>

<ol>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/17.png" width= "800">


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/Imagens/18.png" width= "800">


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_2/output/output-caption-grandefamilia.png" width= "800">

</ol>

</ol>

# <font color= blue>Links utéis e Fontes de pesquisa</font>

-   [Portal Azure][], acessado em 06/03/2024 às 16:10.
-   [Vision Studio][], acessado em 06/03/2024 às 16:20.
-   <sup>**1**</sup> Passo a passo ["Detect faces in the Vision Studio"][1], acessado em 06/03/2024 às 16:15.
-   <sup>**2**</sup> Passo a passo ["Extract text from images in the Vision Studio"][2], acessado em 06/03/2024 às 16:40.
-   <sup>**3**</sup> Passo a passo ["Generate captions for an image"][3], acessado em 06/03/2024 às 16:50.
-   Link da [imagem da Grande Família][4], acessado em 06/03/2024 às 16:25.
-   Link da [imagem João 8:32][5], acessado em 06/03/2024 às 16:45.




[1]: https://aka.ms/ai900-face
[2]: https://aka.ms/ai900-ocr
[3]: https://aka.ms/ai900-image-analysis
[Portal Azure]: https://portal.azure.com/
[Portal Vision Studio]: https://portal.vision.cognitive.azure.com/
[Dio]: https://web.dio.me/lab/reconhecimento-facial-com-azure-ml-transformando-imagens-em-dadosa-no-azure-ml/learning/b643df31-5345-4fb4-9be4-478fe43a93e4
[4]: https://odia.ig.com.br/_midias/jpg/2019/01/19/grandefamilia_840x560-9369560.jpg
[5]: https://i.pinimg.com/736x/81/52/28/81522842c73e11498379f4015a0190b8.jpg
[6]: https://unicast.com.br/posts/criando-uma-conta-gratuita-no-azure/#:~:text=1.1%20Criando%20sua%20conta%20gratuita,cadastro%20ou%20criar%20uma%20nova.