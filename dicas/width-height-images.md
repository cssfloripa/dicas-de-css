---
título: Defina width e height nos elementos <img>
tags: intermediario, performance
---

Sempre especifique `width` e `height` nos seus elementos `<img>`. 

Isso assegura de que browsers modernos possam disponibilizar o espaço correto da imagem enquanto ela carrega, **prevenindo mudanças abruptas de layout**.

**Alternativa:** [reservar um espaço com tamanho proporcional da imagem](#).

```html
<img src="image.jpg">   ---->    <img src="image.jpg" width="320" height="480">
```
