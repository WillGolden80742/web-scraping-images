# Download de Imagens e Background Images

Este projeto consiste em um script Javascript que permite fazer download de todas as imagens e background images de uma página web.

## Funcionalidades

- Faz download de todas as tags `<img>` em uma página
- Faz download de todas as imagens definidas como `background-image` no CSS
- Compacta todas as imagens em um arquivo ZIP para download
- Permite escolher entre baixar somente imagens, somente background images ou ambos

## Como Usar

1. Copie o código Javascript e cole no console do seu navegador na página desejada
2. Execute a função `downloadImagesOrBackgroundImagesOrBoth()`
3. Escolha entre baixar img, background-images ou ambos 
4. Um arquivo ZIP chamado `downloaded_images.zip` será gerado com todas as imagens

## Considerações

- As imagens são nomeadas com um prefixo `image_` ou `background_image_` e uma marca de tempo
- Após baixar as background images, um atributo `data-downloaded` é adicionado para não baixar a mesma imagem novamente
- O código depende da biblioteca JSZip para criar o arquivo ZIP das imagens
- Foi codificado em base64 e decodificado em runtime para facilitar a execução no console

## Créditos

Esse código utiliza a biblioteca [JSZip](https://stuk.github.io/jszip/) para zipar as imagens.
