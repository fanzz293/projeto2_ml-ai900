## Ler texto no Vision Studio

### Essa é uma funcionalidade capaz de, seguindo o conceito  da visão computacional, detectar textos em imagens através de uma técnica conhecida como reconhecimento óptico de caractereres (OCR). 

### Criando um recurso de serviços de IA do Azure

1. Entre com sua conta microsoft a partir do portal https://portal.azure.com
2. Clique no botão da barra ao lado criar um recurso. Faça uma pesquisa através da barra de endereço, escrevendo "serviços de IA do Azure". Após feita a pesquisa, em cima do mesmo nome, clique em criar. Preencha o formulário com os seguintes dados: 

[Figura 3 - Campo de identificação]
 
* Assinatura: sua assinatura
* Grupo de recursos: Selecione ou crie um grupo de recursos com um nome exclusivo
* Região: Brasil
* Nome: Insira o nome da instância
* Nível de preços: Padrão S0

3. Aperte na caixa onde há a confirmação sobre os termos.
Selecione revisar + criar e depois criar e aguarde a conclusão da implantação.

### Conectando seu recurso de serviço de IA do Azure com o Vision Studio

4. Em outra guia no navergador, digite o endereço https://portal.vision.cognitive.azure.com.

[Figura 4: Select a resource to work with]

5. Com sua conta logada, clique em "view all resources". 
Na página "selecione um recurso para trabalhar", procure pelo recurso criado.

6. Selecione o recurso clicando no box e em seguida, no botão abaixo "selecionar como recurso padrão". 
Em seguida, feche a aba. 

### Extraindo texto de imagens no Vision Studio

1. Em um navegador, acesse https://portal.vision.cognitive.azure.com.

Na página inicial Introdução ao Vision, selecione a aba Reconhecimento óptico de caracteres e, em seguida, Extrair texto de imagens.

2. Marcando a caixa vazia em "experiências", você está aceitando a política de uso de recursos "lendo e marcando a caixa.

3. No portal, selecione "Procurar um arquivo" e se quiser, utilize imagens de seu interesse, desde que siga os critérios da lógica da funcionalidade como haver textos dentro de imagens, a partir de seu computador ou baixe o [pacote de imagens ocr-images.zip](https://aka.ms/mslearn-ocr-images/). A imagem utilizada será advert.jpg.

4. Confira a saída no painel "Atributos detectados". Qualquer texto encontrado na imagem é organizado em uma estrutura hierárquica de regiões, linhas e palavras.

[Figura 4.2]

#### Obrigado por visualizar

**Referências:**

[Lendo texto no Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html/) 

