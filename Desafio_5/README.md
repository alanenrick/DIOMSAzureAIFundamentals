<h1><a href="https://x.gd/GIELw"><img src="https://x.gd/gEbZi" align= "left" width= "160" alt="Imagem do desafio: Explorando os Recursos de IA Generativa com Copilot e OpenAI"></a>
<h1>Desafio de projeto 5
<font color= red>
<h1>Explorando os Recursos de IA Generativa com Copilot e OpenAI</h1>
</font>
</font>
</h1>

<h3 id="sum">Sumário</h3>

<ul Align="justify">

<nav>


<li><a href="#intro">Introdução</a></li>
<li><a href="#obj">Objetivo</a></li>
<li><a href="#passo">Passo a passo</a></li>

<ol>
<li><a href="#passo1">Acessar o Portal Azure e criar uma conta</a></li>
<li><a href="#passo2">Recursos</a></li>
<li><a href="#passo3">Criar recurso "Azure AI services"</a></li>
<li><a href="#passo4">Editando e criando recurso</a></li>
<li><a href="#passo5">Portal Vision Studio</a></li>
<li><a href="#passo6">Definir recurso como padrão</a></li>
<li><a href="#passo7">Acessar "Extract text from images"</a></li>
<li><a href="#passo8">Criar imagens com "Copilot"</a></li>
<li><a href="#passo9">Testar imagens no recurso</a></li>
<ol>
<li><a href="#img1">Imagem 01</a></li>
<li><a href="#img2">Imagem 02</a></li>
<li><a href="#img3">Imagem 03</a></li>
<li><a href="#img4">Imagem 04</a></li>
</ol>
<li><a href="#passo10">Testar recuso com "copilot"</a></li>
<ol>
<li><a href="#img11">Imagem 01</a></li>
<li><a href="#img22">Imagem 02</a></li>
<li><a href="#img33">Imagem 03</a></li>
<li><a href="#img44">Imagem 04</a></li>
</ol>

</ol>
<li><a href="concl">Conclusão</a></li>
<li><a href="#links">Links úteis</a></li>
</ul>
</nav>

#

<ul Align="justify">

<h1 id="intro"><li>Introdução </li></h1>

<h6 align= right><a href="#sum">&#00012</a></h6>

<p>Este desafio de projeto tem como objetivo mostrar como usar o recurso do "<em>Vision Studio</em>" para extrair texto de imagens. Porém pode-se ir além do proposto, usando o "<em>Copilot</em>" para geração de imagens e também para extrair texto de imagem.</p> 
<p>Após a conclusão do projeto seguindo os passos pode se ter algumas idéias de aplicações para estes recursos.</p>
<p>Uma delas seria uso dos recursos do "<em>Vision Studio</em>" em empresas para fazer a transcrição de documentos(uma foto de uma nota fiscal) para análise e, se for o caso, armazenamento em banco de dados. Já para o "<em>Copilot</em>" as possibilidades são inumeras desde a geração de imagens, interpretação de imagens com sugestão de pesquisa, tirar dúvidas, entre outras possibilidades.</p>

<h1 id="obj"><li>Objetivo</li></h1>

<h6 align= right><a href="#sum">&#00012</a></h6>

<ol>

<li>Criar um novo repositório no github com um nome a sua preferência;</li>

<li>Criar um arquivo README.md descrevendo o passo a passo para extração de texto de uma imagem, assim como seus insights, possibilidades de aplicações que se benefíciariam com esse tipo de ferramenta e aprendizados adquiridos durante o processo;</li>

<li>Compartilhar com a <a href="https://x.gd/GIELw">Dio</a> o link do <a href="https://github.com/alanenrick/DIOMSAzureAIFundamentals/tree/main/Desafio_5">repositório</a> através do botão '<em>entregar projeto</em>'.</li>

</ol>

<h1 id="passo"><li>Passo a passo</li></h1>

<h6 align= right><a href="#sum">&#00012</a></h6>

*Todos os passos e parâmetros a seguir foram baseados nas aulas do projeto e pelo link<sup>**[1][]**,**[2][6]**,**[3][9]**</sup> indicado.*

*Mantenhanha  o idioma do **Microsoft Azure** em inglês, pois os nomes dos recursos aparecem diferente quando muda o idioma, pode acabar atrapalhando.*

<ol>

<h3 id= "passo1"><li>Acessar o <em><a href= "https://portal.azure.com">Portal Azure</a></em> e <em><a href= "https://unicast.com.br/posts/criando-uma-conta-gratuita-no-azure/#:~:text=1.1%20Criando%20sua%20conta%20gratuita,cadastro%20ou%20criar%20uma%20nova.">Criar uma conta</a></em>.</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<h3 id= "passo2"><li>Clicar em "<em>create a resource</em>".</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/01.png" width= "900">

<h3 id= "passo3"><li>Na aba "<em>AI + Machine learning</em>", ir em "<em>Azure AI services</em>" clicar em "<em>Create</em>". </li><h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/02.png" width= "900">

<h3 id= "passo4"><li>Preencher Lacunas. </li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<ul>
<li><strong>Subscription</strong>: Selecionar sua subscrição. </li>
<li><strong>Resource group</strong>: Selecionar um recurso existente ou criar um novo. </li>
<li><strong>Region</strong>: East US. </li>
<li><strong>Name</strong>: Criar um nome único. </li>
<li><strong>Pricing tier</strong>: Standard S0. </li>
<li><strong>By checking this box I acknowledge that I have read and understood all the terms below</strong>: Selecionar. </li>

</ul>

#### Clicar em "<em>Review + create</em>".

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/03.png" width= "900">

#### Clicar em "<em>Create</em>".

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/04.png" width= "900">

#### Aguardar "<em>Deployment</em>", completo.

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/05.png" width= "900">

<h3 id="passo5"><li>No <a href="https://portal.vision.cognitive.azure.com/">"<em>Portal Vision Studio</em>"</a>, clicar em "<em>View all resources</em>". </li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/06.png" width= "900">

<h3 id="passo6"><li>Selecionar o recurso criado e clicar em "<em>Select as default resource</em>".</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/07.png" width= "900">

<h3 id="passo7"><li> Na tela principal ir na aba "<em>Optical character recognition</em>" e selecionar "<em>Extract text from images</em>".</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Imagens/08.png" width= "900">

#### Testar recurso com uma imagem padrão.

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_test.png" width= "900">

<h3 id="passo8"><li>Criando imagens com o "<a href="https://copilot.microsoft.com/"><em>Copilot</em></a>".</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>


<p>Foi usado o "<em>Copilot</em>" para gerar as imagens.</p>
<p>A frase usada foi um trecho bíblico, do Salmo 23 em inglês:</p>
<p>“The Lord is my Shepherd; I shall not want. He maketh me to lie down in green pastures: he leadeth me beside the still waters.”</p>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/input_copilot_01.png" width= "900">

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/input_copilot_02.png" width= "900">

<h3 id="passo9"><li>Testando recurso com as imagens criadas.</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<ol>
<h3 id=img1><li>Imagem 01</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/01.jpg"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/01.jpg" width= "300"></a>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_01.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_01.png" width= "900"></a>

<h3 id=img2><li>Imagem 02</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/02.jpg"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/02.jpg" width= "300"></a>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_02.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_02.png" width= "900"></a>

<h3 id=img3><li>Imagem 03</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/03.jpg"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/03.jpg" width= "300"></a>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_03.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_03.png" width= "900"></a>

<h3 id=img4><li>Imagem 04</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/04.jpg"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Inputs/04.jpg" width= "300"></a>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_04.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/output_04.png" width= "900"></a>

</ol>

<h3 id="passo10"><li>Testando mesmo recurso com "<em>Copilot</em>".

<h6 align= right><a href="#sum">&#00012</a></h6>

<ol>

<h3 id=img11><li>Imagem 01</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_01.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_01.png" width= "900"></a>

<h3 id=img22><li>Imagem 02</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_02.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_02.png" width= "900"></a>

<h3 id=img33><li>Imagem 03</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_03.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_03.png" width= "900"></a>

<h3 id=img44><li>Imagem 04</li></h3>

<h6 align= right><a href="#sum">&#00012</a></h6>

<a href="https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_04.png"><img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_5/Outputs/Copilot_04.png" width= "900"></a>

</ol>
</ol>

<h1 id="concl"><li>Conclusão</li></h1>

<h6 align= right><a href="#sum">&#00012</a></h6>

<p>Com base nos resultados obtidos com o recurso "<em>Extract text from images</em>" pode se observar que, provavelmente, devido a fonte usada no text da imagem, há varios erros no reconhecimento ortográfico. O mesmo não ocorre usando o "<em>Copilot</em>" que ,durante a análise da imagem, faz a correlação do texto identificado com outros textos existentes e corrige a sintaxe, além disso gera uma descrição do tipo de texto que foi analisado e a que ele se refere.</p>

<h1 id="links"><li>Links utéis e Fontes de pesquisa</li></h1>

<h6 align= right><a href="#sum">&#00012</a></h6>

-   [Portal Azure][2], acessado em 28/03/2024 às 18:15.
-   [Portal Vision Studio][7], acessado em 28/03/2024 às 18:20.
-   [Copilot][8], acessado em 28/03/2024 às 18:30.
-   <sup>**1**</sup> Passo a passo ["Read text in Vision Studio"][1], acessado em 28/03/2024 às 18:15.
-   <sup>**2**</sup> Passo a passo ["Explore generative AI with Microsoft Copilot"][6], acessado em 28/03/2024 às 18:15.
-   <sup>**3**</sup> Passo a passo ["Explore generative AI with Microsoft Copilot"][9], acessado em 28/03/2024 às 18:30.

</ul>


[1]: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html

[2]: https://portal.azure.com

[3]: https://github.com/alanenrick/DIOMSAzureAIFundamentals/tree/main/Desafio_5

[4]: https://unicast.com.br/posts/criando-uma-conta-gratuita-no-azure/#:~:text=1.1%20Criando%20sua%20conta%20gratuita,cadastro%20ou%20criar%20uma%20nova.

[5]: https://x.gd/GIELw

[6]: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/12-generative-ai.html

[7]: https://portal.vision.cognitive.azure.com/

[8]: https://copilot.microsoft.com/

[9]: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/12-generative-ai.html