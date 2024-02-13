## Detectar rostos no Vision Estudio

### Permite explorar os recursos de detecção de rostos em uma imagem sem a necessidade de escrever nenhum código. 

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

### Detectando rostos no Visio Studio

7. Abra no navegador o seguinte endereço: https://portal.vision.cognitive.azure.com
8. Em sua página inicial, selecione a guia Face e, em seguida, selecione o bloco Detectar rostos em uma imagem
Aperte no botão de checkbox, aceitando o termo de reconhecimento sobre essa demonstração (para mais detalhes leia todo o termo).
9. Podes selecionar qualquer uma das imagens para fazer análises e verificar os dados de detecção facial retornados.
10. Fazendo o download e utilizando os arquivos das próprias imagens dos servidores da Azure (disponível em https://aka.ms/mslearning-detect-faces), temos três tipos de imagens diferentes:

[Figura 1]

[Figura 2]

[Figura 3]

11. Fazendo o upload de cada um deles, podemos conferir seus respectivos retornos na tela de "atributos detectados", em que se retorna quantos rostos foram detectados e se as pessoas da foto estão utilizando máscara.

Figura 1

Rosto #1
Máscara facial: não 

Figura 2

Rosto #1
Máscara facial: não 
Rosto #2
Máscara facial: não 
Rosto #3
Máscara facial: não 

Figura 3 

Nenhum rosto detectado

O script utilizado para implementar a funcionalidade do programama está no formado JSON. Confira abaixo: 

```
[
  {
    "recognitionModel": "recognition_01",
    "faceRectangle": {
      "width": 93,
      "height": 144,
      "left": 324,
      "top": 95
    },
    "faceLandmarks": {
      "pupilLeft": {
        "x": 365.5,
        "y": 156.7
      },
      "pupilRight": {
        "x": 404.7,
        "y": 158.1
      },
      "noseTip": {
        "x": 396.8,
        "y": 183.8
      },
      "mouthLeft": {
        "x": 357.5,
        "y": 200.1
      },
      "mouthRight": {
        "x": 398.7,
        "y": 202.3
      },
      "eyebrowLeftOuter": {
        "x": 346.2,
        "y": 146.7
      },
      "eyebrowLeftInner": {
        "x": 381.6,
        "y": 145.9
      },
      "eyeLeftOuter": {
        "x": 358.1,
        "y": 156.6
      },
      "eyeLeftTop": {
        "x": 366,
        "y": 154.6
      },
      "eyeLeftBottom": {
        "x": 365.8,
        "y": 158.6
      },
      "eyeLeftInner": {
        "x": 372,
        "y": 157.1
      },
      "eyebrowRightInner": {
        "x": 400.1,
        "y": 147
      },
      "eyebrowRightOuter": {
        "x": 417,
        "y": 145.8
      },
      "eyeRightInner": {
        "x": 398.6,
        "y": 158.5
      },
      "eyeRightTop": {
        "x": 405,
        "y": 155.7
      },
      "eyeRightBottom": {
        "x": 404.9,
        "y": 159.9
      },
      "eyeRightOuter": {
        "x": 410.3,
        "y": 158.4
      },
      "noseRootLeft": {
        "x": 383,
        "y": 158.7
      },
      "noseRootRight": {
        "x": 395.2,
        "y": 159.2
      },
      "noseLeftAlarTop": {
        "x": 379.9,
        "y": 174.9
      },
      "noseRightAlarTop": {
        "x": 400.2,
        "y": 174.8
      },
      "noseLeftAlarOutTip": {
        "x": 373.8,
        "y": 182.8
      },
      "noseRightAlarOutTip": {
        "x": 402.9,
        "y": 183.2
      },
      "upperLipTop": {
        "x": 388.7,
        "y": 197.5
      },
      "upperLipBottom": {
        "x": 387.4,
        "y": 201.8
      },
      "underLipTop": {
        "x": 385.2,
        "y": 213.5
      },
      "underLipBottom": {
        "x": 384.1,
        "y": 220.1
      }
    },
    "faceAttributes": {
      "mask": {
        "type": "noMask",
        "noseAndMouthCovered": false
      }
    }
  }
]

```

#### Pronto! O exercício foi exercício!

#### Obrigado pela atenção!

**Referências:**

[Detectando rostos no Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html/) 

