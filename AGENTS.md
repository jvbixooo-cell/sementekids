# Arquitetura

Este projeto publica um site estático recebido em um arquivo ZIP. A exigência do usuário é preservar o site sem alterações visuais ou de conteúdo.

- `public/index.html`: página completa em português, com CSS e JavaScript incorporados; contém carrosséis, perguntas frequentes, notificações e links de compra.
- `public/images/`: imagens WebP originais.
- `public/js/`: scripts de rastreamento fornecidos no arquivo original.
- `netlify.toml`: publica `public` sem compilação.

## Convenções e decisões

Preserve textos, preços, links, estilos, imagens, comportamento e integrações originais, salvo solicitação explícita. Mantenha caminhos relativos aos assets. Não introduza um framework ou uma etapa de compilação para esta página estática. Os metadados de compartilhamento ficam no head do HTML; não defina og:image, pois a plataforma o fornece. Não exponha credenciais nos arquivos ou logs.
