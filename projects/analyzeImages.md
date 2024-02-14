![Cor](https://github.com/fanzz293/projeto2_ml-ai900/blob/main/assets/dio.jpeg?raw=true)

## Analise de imagens no Vision Studio

### É uma ferramenta capaz de compreender o conteúdo e o contexto da imagem e extrair informações nela contidas através de experiências de teste integradas ao Vision Studio. 

### Criando um recurso de serviços de IA do Azure

1. Entre com sua conta microsoft a partir do portal https://portal.azure.com
2. Clique no botão da barra ao lado criar um recurso. Faça uma pesquisa através da barra de endereço, escrevendo "serviços de IA do Azure". Após feita a pesquisa, em cima do mesmo nome, clique em criar. Preencha o formulário com os seguintes dados: 

![o](https://github.com/fanzz293/projeto2_ml-ai900/blob/main/assets/Figura%202%20-%20Formul%C3%A1rio.jpg?raw=true)
 
* Assinatura: sua assinatura
* Grupo de recursos: Selecione ou crie um grupo de recursos com um nome exclusivo
* Região: Brasil
* Nome: Insira o nome da instância
* Nível de preços: Padrão S0

3. Aperte na caixa onde há a confirmação sobre os termos.
Selecione revisar + criar e depois criar e aguarde a conclusão da implantação.

### Conectando seu recurso de serviço de IA do Azure com o Vision Studio

4. Em outra guia no navergador, digite o endereço https://portal.vision.cognitive.azure.com.

5. Com sua conta logada, clique em "view all resources". 
Na página "selecione um recurso para trabalhar", procure pelo recurso criado.

![9](https://github.com/fanzz293/projeto2_ml-ai900/blob/main/assets/figura%204.jpg?raw=true)

6. Selecione o recurso clicando no box e em seguida, no botão abaixo "selecionar como recurso padrão". 
Em seguida, feche a aba. 

### Gerar legendas para uma imagem

7. Em um navegador, acesse https://portal.vision.cognitive.azure.com.

8. Em sua página inicial, selecione o guia "Análise de Imagens e, em seguida, selecione a seção adicionar legendas às Imagens

![Ponto](https://raw.githubusercontent.com/fanzz293/projeto2_ml-ai900/3729b333bc3169abf8358a57273f50c7279ac422/assets/Figura%203.1.jpg)

9. Aperte no botão de checkbox, aceitando o termo de reconhecimento sobre essa demonstração (para mais detalhes leia todo o termo).
Podes selecionar qualquer uma das imagens para fazer análises e verificar os dados de detecção facial retornados.

10.  Nesse exercício será utilizada uma das imagens da própria Azure para experimento. [Clique aqui para baixar o arquivo compactado.](https://aka.ms/mslearn-images-for-analysis/). Você pode também utilizar outros arquivos de sua preferência.

A imagem a ser utilizada será essa: 

![o](https://github.com/fanzz293/projeto2_ml-ai900/blob/main/inputs/analysis/store-camera-1.jpg?raw=true)

11. Carregue a imagem arrastando-a para a caixa "Arrastar e soltar arquivos aqui" ou navegando até ela em seu sistema de arquivos.

Observe o texto da legenda gerado, a saída será a seguinte:

![o](https://github.com/fanzz293/projeto2_ml-ai900/blob/main/outputs/outputAnalizeImages.jpg?raw=true)

#### A funcionalidade Legenda fornece uma única frase em linguagem natural que descreve o conteúdo da imagem.

12. Em seguida, use a mesma imagem para executar legendas densas. Retorne à [homepage do Vision Studio](https://portal.vision.cognitive.azure.com/). Vá em adicionar legendas densas. 

![Ps](https://raw.githubusercontent.com/fanzz293/projeto2_ml-ai900/3729b333bc3169abf8358a57273f50c7279ac422/assets/Figura%203.2.jpg)

**Legendas densas**

##### Descrição: Esse recurso vai retornar mais dados sobre a imagem, cobrinodo outros objetos detectados na respectiva imagem. Cada objeto detectado inclui uma delimitação que define uma área selecionada com as coordenadas de pixel dentro da imagem. 

**Marcando imagens**

#### As tags de extração são baseadas em milhares de objetos reconhecíveis, incluindo seres vivos, cenários e ações.

1. Vá no [endereço do Vision Studio](https://portal.vision.cognitive.azure.com/) e selecione o bloco Extrair marcas comuns de imagens na guia Análise de imagem.

![p](https://raw.githubusercontent.com/fanzz293/projeto2_ml-ai900/3729b333bc3169abf8358a57273f50c7279ac422/assets/Figura%203.3.jpg)

2. Em Escolha o modelo que você deseja experimentar, deixe Produto pré-criado versus modelo de intervalo selecionado. Em Escolha seu idioma, selecione Inglês ou um idioma de sua preferência.

3. Abra a pasta que contém as imagens que foram baixadas e localize o arquivo chamado store-image-2.jpg, ou alguma outra imagem de sua prefeência.

4. No painel ao lado é mostrado as tags extraídas e suas respectivas pontuações de confiança, que medem o grau de probabilidade de um objeto representar realmente o que está na imagem. 

**Detecção de objetos** 

#### A detecção de objetos detecta e extrai caixas delimitadoras com base em milhares de objetos reconhecíveis e seres vivos.

1.  Vá no [endereço do Vision Studio](https://portal.vision.cognitive.azure.com/) e selecione o bloco Detectar objetos comuns em imagens na guia Análise de imagem.

![p](https://raw.githubusercontent.com/fanzz293/projeto2_ml-ai900/3729b333bc3169abf8358a57273f50c7279ac422/assets/Figura%203.4.jpg)

2. Em Escolha o modelo que você deseja experimentar, deixe Produto pré-criado versus modelo de intervalo selecionado.

3. Abra e carregue a pasta que contém as imagens que foram baixadas ou qualquer outro de sua preferência. A imagem que será utilizada no exemplo é "store-camera-3.jpg".

4. No painel de atributo detectados, observe a lista de objetos detectados e suas pontuações de confiança.

5. Passe o cursor do mouse sobre os objetos na lista Atributos detectados para realçar a caixa delimitadora do objeto na imagem.

#### Movendo o controle deslizante "Valor de limite" até que se atinja o valor da probabilidade estabelecida para aquele, podemos ter a noção do que acontece com os objetos na lista. O controle deslizante de limite especifica que somente objetos identificados com uma pontuação de confiança ou probabilidade maior que o limite devem ser exibidos.

#### Obrigado por visualizar

**Referências:**

[Gerar legenda para uma imagem](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html/) 
