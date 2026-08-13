---
title: "Ajustando Tamanho das Imagens"
nav_order: 1
parent: "Azure DevOps"
---

No Azure DevOps, quando você quer incorporar imagens na descrição de um item de trabalho, na wiki ou em qualquer outro campo de texto formatado, o Azure DevOps usa a sintaxe Markdown.

No Markdown padrão, não há um meio nativo de especificar dimensões para uma imagem. No entanto, para especificar um tamanho para a sua imagem, você pode usar tags HTML no lugar da sintaxe Markdown.

Aqui está um exemplo de como você pode definir o tamanho de uma imagem usando tags HTML:

```html
<img src="https://upload.wikimedia.org/wikipedia/commons/a/ab/Cynefin_framework_2022.jpg" alt="Cynefin framework - Wikipedia" width="500" height="300"/>
```

Neste exemplo, a imagem terá uma largura de 500 pixels e uma altura de 300 pixels. Você pode ajustar os valores `width` e `height` conforme necessário.

Coloque esse código no campo de texto formatado do Azure DevOps onde você deseja que a imagem apareça e ela será renderizada no tamanho especificado.

Porém, note que quando você define explicitamente a largura e a altura da imagem, você pode distorcer a imagem se não manter a proporção original. Se quiser manter a proporção, defina apenas um dos valores (largura ou altura) e deixe o outro valor ajustar automaticamente. Por exemplo:

```html
<img src="https://upload.wikimedia.org/wikipedia/commons/a/ab/Cynefin_framework_2022.jpg" alt="Cynefin framework - Wikipedia" width="500"/>
```

Neste caso, apenas a largura é definida, e a altura se ajustará proporcionalmente.