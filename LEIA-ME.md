# RPGpédia para Owlbear Rodeo

Extensão mínima que adiciona um botão chamado **RPGpédia** ao Owlbear Rodeo.
Ao clicar, tenta abrir `https://rpgpedia.com/colecoes` dentro do painel (Action Popover).

## Arquivos

- `manifest.json`: configuração da extensão.
- `icon.svg`: ícone do botão.

## Publicação

1. Publique estes arquivos em um serviço de hospedagem estática com HTTPS
   (por exemplo, GitHub Pages).
2. Mantenha `manifest.json` e `icon.svg` na raiz do endereço publicado.
3. No Owlbear Rodeo, use **Add Extension** e informe o endereço público de
   `manifest.json`.

## Observação importante sobre a incorporação

O painel do Owlbear é exibido em um iframe. A RPGpédia pode impedir a incorporação
por meio dos cabeçalhos HTTP `Content-Security-Policy: frame-ancestors` ou
`X-Frame-Options`. Se isso acontecer, o Owlbear poderá mostrar uma página em
branco ou um erro de bloqueio. Isso é uma restrição do site de destino; a extensão
não consegue removê-la. O comportamento precisa ser testado depois da publicação.

Este projeto não usa Supabase, login próprio, banco de dados ou armazenamento de NPCs.
