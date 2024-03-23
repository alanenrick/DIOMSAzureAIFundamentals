<h1><a href="https://x.gd/77Uz6"><img src="https://x.gd/I9Qlv" align= "left" width= "160" alt="Imagem do desafio: Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados"></a>
<h1>Desafio de projeto 4
<font color= red>
<h1>
Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados</h1>
</font>
</font>
</h1>

<ul>

# <li>Apresentação </li>

<p>Este projeto tem como objetivo mostrar como usar o recurso do "**Azure AI Search**" para indexação e consulta de dados.</p> 
<p>Após concluir o projeto seguindo os passos pode se ter algumas ideias de aplicação para este recurso.</p>
<p>Uma delas seria para uso em uma rede de franquias, na qual pode se obter rapidamente através de uma breve busca varios dados das franquias de uma determinada localidade, saber quais franquias são melhores e piores avaliadas e o motivo. Entre outras aplicações. Ou seja o principal uso desse recurso seria por empresas independente do tamanho da mesma.</p>

# <li>Objetivo</li>

<ol>

#### <li>Criar um novo repositório no github com um nome a sua preferência</li>

#### <li>Criar um um arquivo readme.md descrevendo o passo a passo para se configurar uma pesquisa, assim como seus insights, possibilidades de ferramentas que se beneficiam com esse tipo de ferramenta e aprendizados adquiridos durante o processo.</li>

#### <li>Compartilhar conosco([Dio][5]) o link desse repositório através do botão 'entregar projeto'.</li>

</ol>

# <li>Passo a passo</li>

*Todos os passos e parâmetros a seguir foram baseados nas aulas do projeto e pelo link<sup>**[1][]**</sup> indicado.*

*Mantenhanha  o idioma do **Microsoft Azure** em inglês, pois os nomes dos recursos aparecem diferente quando muda o idioma, pode acabar atrapalhando.*

<ol>

### <li>Acessar o ***[Portal Azure][2]*** e ***[Criar uma conta][4]***.</li>


### <li>Clicar em "**create a resource**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/01.png" width= "900">


### <li>Pesquisar por "**Azure AI Search**" e clicar em "**Create**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/02.png" width= "900">


### <li>Preencher lacunas conforme abaixo e depois clicar em "**Review + create**".

<ul>
<li><strong>Subscription</strong>: <em>Sua inscrição do Azure</em>.</li>
<li><strong>Resource group</strong>: <em>Selecionar um existente ou criar um novo</em>.</li>
<li><strong>Service name</strong>: <em>Criar um nome único</em>.</li>
<li><strong>Location</strong>: <em>Escolher uma região disponível</em>.</li>
<li><strong>Pricing tier</strong>: Basic</li>
</ul>

###

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/03.png" width= "900">
</li>

### <li>Ir em "**Create a resource**", "**AI + Machine learning**" e em "**Azure AI services**" clicar em "**Create**"</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/04.png" width= "900">


### <li>Preencher lacunas conforme abaixo e clicar em "**Review + Create**".</li>

<ul>
<li><strong>Subscription</strong>: <em>Sua inscrição do Azure</em>.</li>
<li><strong>Resource group</strong>: <em>O mesmo usado no "<strong>Azure AI Search</em>.</li>
<li><strong>Region</strong>: <em>The same location as your Azure AI Search resource</strong>"</em>.</li>
<li><strong>Name</strong>: <em>Criar um nome único</em>.</li>
<li><strong>Pricing tier</strong>: Standard S0</li>
<li><strong>By checking this box I acknowledge that I have read and understood all the terms below</strong>: Selecionar</li>
</ul>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/05.png" width= "900">


### <li>Ir no menu no lado superior esquerdo e depois em "**Storage acounts**" e em "**Create**".</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/06
.png" width= "900">


### <li>Preencher lacunas conforme abaixo e clicar em "**Review + create**"</li>

<ul>
<li><strong>Subscription</strong>: <em>Sua inscrição do Azure</em>.</li>
<li><strong>Resource group</strong>: <em>Usar o mesmo do "<strong>Azure AI Search</strong>"</em>.</li>
<li><strong>Region</strong>: <em>Usar o mesmo do "<strong>Azure AI Search</em>.</li>
<li><strong>Name</strong>: <em>Criar um nome único</em>.</li>
<li><strong>Pricing tier</strong>: Standard S0</li>
<li><strong>By checking this box I acknowledge that I have read and understood all the terms below</strong>: Selecionar</li>
</ul>

###

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/07.png" width= "900">

### <li>Em "**Strorage accounts**", selecionar o recurso recém criado.</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/08.png" width= "900">

###

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/09.png" width= "900">

### <li>Na lista à esquerda selecionar "**configuration**"</li>

Mudar a configuração "**Allow Blob anonymous access**" para "**Enabled**" e selecione "**Save**"

###

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/10.png" width= "900">

### <li>Na lista à esquerda selecionar "**Containers**" e em "**+ Container**"</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/11.png" width= "900">


### Preencher e clicar em "**Create**".

<ul>
<li><strong>Name</strong>: search-coffee</li>
<li><strong>Public access level</strong>: Container (anonymous read access for containers and blobs)</li>
<li><strong>Advanced</strong>: <em>Sem mudanças</em>.</li>
</ul>

###
<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/12.png" width= "900">

### <li>Selecionar o container criado e clicar em "**Upload**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/13.png" width= "900">

### Utilizar os arquivos disponibilizados no [Link][3].

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/14.png" width= "900">

### <li>Ir ao recurso do "**AI Search**" e clicar em "**Import data**"</li>


<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/15.png" width= "900">

###

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/16.png" width= "900">

### <li>Na aba "**Connect to your data**", em "**Data Source**", selecionar "**Azure Blob Storage**". Peencher conforme abaixo:</li>

<ul>
<li><strong>Data Source</strong>: Azure Blob Storage</li>
<li><strong>Data source name</strong>: search-coffee</li>
<li><strong>Data to extract</strong>: Content and metadata</li>
<li><strong>Parsing mode</strong>: Default</li>
<li><strong>Connection string</strong>: *Select <strong>Choose an existing connection</strong>. Selecionar o "storage account" criado anteriormente.</li>
<li><strong>Managed identity authentication</strong>: None</li>
<li><strong>Container name</strong>: <em>this setting is auto-populated after you choose an existing connection</em>.</li>
<li><strong>Blob folder</strong>: <em>Deixar em branco</em>.</li>
<li><strong>Description</strong>: Reviews for Fourth Coffee shops.</li>
</ul>

### Clicar "**Next: Add cognitive skills (Optional)**".

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/17.png" width= "900">

### <li>Na aba "**Attach AI Services**", selecionar seu recurso "**Azure AI services**"</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/18.png" width= "900">

### <li>Na aba "**Add enrichments**", preenche conforme abaixo:</li>

<ul>

<li><strong>Skillset name</strong>: <em>coffee-skillset</em>.</li>
<li><strong>Enable OCR and merge all text into merged_content field</strong>: Selecionar.

<blockquote>
<strong>Nota:</strong>
É importante habilitar <strong>Enable OCR</strong> para ver as opções completas.
</blockquote>
<li><strong>Source data field</strong>: <em>merged_content</em>.</li>
<li><strong>Enrichment granularity level</strong>: <em>Pages (5000 character chunks)</em></li>
<li><strong>Enable incremental enrichment</strong>: <em>Não selecionar.</em></li>

### Selecionar os campos conforme a seguir:

<table>

<tr>
<th>Cognitive Skill</th>
<th>Field name</th>
</tr>
<tr>
<td>Extract location names</td>
<td>locations</td>
</tr>
<tr>
<td>Extract key phrases</td>
<td>keyphrases</td>
</tr>
<tr>
<td>Detect sentiment</td>
<td>sentiment</td>
</tr>
<tr>
<td>Generate tags from images</td>
<td>imageTags</td>
</tr><tr>
<td>Generate captions from images</td>
<td>imageCaption</td>
</tr>

</table>
</ul>

###

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/19.png" width= "900">

### Na aba "**Save enrichments to a knowledge store**", selecionar:

<ul>
<strong>
<li>Managed identity authentication: </strong>None<strong></li>
<li>Image projections</li>
<li>Documents</li>
<li>Pages</li>
<li>Key phrases</li>
<li>Entities</li>
<li>Image details</li>
<li>Image references</li>
</strong>
</ul>

###

<blockquote>
<strong>Nota:</strong>
Se aparecer o campo "<strong>Storage Account Connection String</strong>".
<ul>
<li>Clicar em "<strong>Choose an existing connection</strong>". Selecionar o criado ateriormente para esse projeto.</li>
</ul>
</blockquote>

### <li>Selecionar "<strong>Azure blob projections: Document</strong>". Deixar  "<strong>Container name</strong>" e "<strong>knowledge-store Power BI</strong>" preenchidos automaticamente. Não mudar nome do container.</li>
### Clicar em "**Next: Customize target index**".

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/20.png" width= "900">

### <li>Na aba "**Customize target index**".</li>
<ul>
<li>Alterar "<strong>Index name</strong>": <em>coffee-index</em>.</li>
<li>Definir "<strong>Key</strong>": <em>metadata_storage_path</em>.</li>
<li>Deixar "<strong>Suggester name</strong>" em branco e "<strong>Search mode</strong>" preenchido automaticamente.</li>
<li>Revisar configurações padrão. Selecionar "<strong>filterable</strong>" para todos os campos selecionados por padrão.</li>
</ul>

### Clicar em "<strong>Next: Create an indexer</strong>".

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/21.png" width= "900">

### <li>Na aba "**Create an indexer**".</li>
<ul>
<li><strong>Indexer name</strong>: <em>coffee-indexer</em>.</li>
<li><strong>Schedule</strong>: <strong>Once</strong>.</li>
</ul>

###
<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/22.png" width= "900">

### <li>Expandir aba "<strong>Advanced options</strong>". Marcar "<strong>Base-64 Encode Keys</strong>" e clicar em "**submit**".</li>
  
<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/23.png" width= "900">

### <li>No recurso criado do "**Azure AI search**", na aba "**Overview**", ir em "**Search explorer**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/27.png" width= "900">

### <li>Na aba "**Search explorer**" mudar a visão para "**{ } JSON view**".</li>

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/28.png" width= "900">

### <li>No "<strong>JSON query editor</strong>", copiar e colar:</li>

<pre><code>{
    "search": "*",
    "count": true
}
</code></pre>

###  Retornou o resultado [.JSON](https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Outputs/result-search-1.json).

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/29.png" width= "900">

### <li>Pesquisar pela localização "Chicago": No "<strong>JSON query editor</strong>", copiar e colar:</li>

<pre><code>{
 "search": "locations:'Chicago'",
 "count": true
}
</code></pre>

###  Retornou o resultado [.JSON](https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Outputs/result-search-2.json).

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/30.png" width= "900">

### <li>Pesquisar por "Sentimento": No "<strong>JSON query editor</strong>", copiar e colar:</li>

<pre><code>{
 "search": "sentiment:'negative'",
 "count": true
}
</code></pre>

###  Retornou o resultado [.JSON](https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Outputs/result-search-3.json).

<img src= "https://raw.githubusercontent.com/alanenrick/DIOMSAzureAIFundamentals/main/Desafio_4/Imagens/31.png" width= "900">


</ol>

# <li>Links utéis e Fontes de pesquisa</li>

-   [Portal Azure][2], acessado em 20/03/2024 às 19:15.
-   <sup>**1**</sup> Passo a passo ["Explore an Azure AI Search index"][1], acessado em 20/03/2024 às 19:15.
 
</ul>


[1]: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html

[2]: https://portal.azure.com

[3]: https://github.com/alanenrick/DIOMSAzureAIFundamentals/raw/main/Desafio_4/reviews.zip

[4]: https://unicast.com.br/posts/criando-uma-conta-gratuita-no-azure/#:~:text=1.1%20Criando%20sua%20conta%20gratuita,cadastro%20ou%20criar%20uma%20nova.

[5]: https://x.gd/77Uz6