---
título: Defina width e height nos elementos <img>
tags: intermediario, performance
---

Sempre especifique `width` e `height` nos seus elementos `<img>`. 

Isso assegura de que browsers modernos possam disponibilizar o espaço correto da imagem enquanto ela carrega, **prevenindo mudanças abruptas de layout**.

**Alternativa:** [reservar um espaço com tamanho proporcional da imagem](https://github.com/cssfloripa/dicas-de-css/blob/width-height-images/dicas/aspect-ratio-boxes.md).

```html
<img src="image.jpg">   ---->    <img src="image.jpg" width="320" height="480">
```

----

**Fonte:** [Tweet de Addy Osmani](https://twitter.com/addyosmani/status/1276779799198007301) 
