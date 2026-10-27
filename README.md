# Garimpo Pro — versão web instalável

## O que inclui
- Cadastro e edição de peças, custos, datas, status, observações.
- Lucro líquido, margem e ROI para peças vendidas; lucro estimado para estoque.
- Resumo de capital em estoque, dinheiro recuperado e lucro acumulado.
- Meta mensal de lucro.
- Busca, filtros, ordenação e exclusão.
- Backup JSON e restauração.
- PWA com cache offline após a primeira visita/instalação.

## Instalar no Moto G75
A instalação PWA precisa estar publicada em um endereço HTTPS. A pasta local não pode ser instalada como app com funcionamento offline completo.
1. Publique estes arquivos em um site HTTPS estático (por exemplo, GitHub Pages).
2. No Moto G75, abra o endereço no Chrome.
3. Aguarde a página carregar completamente uma vez com internet.
4. Menu ⋮ do Chrome → **Instalar app** (ou **Adicionar à tela inicial**, dependendo da versão).
5. Abra o ícone Garimpo Pro na tela inicial. O service worker guarda a interface para uso offline.
6. Faça um backup em **Backup e dados → Exportar backup** regularmente. Guarde o JSON em Arquivos/Drive/outro local seguro.

## Restaurar
Abra o app, use **Restaurar backup** e escolha o arquivo JSON. A restauração substitui os dados atuais, então exporte um backup dos dados atuais antes de restaurar, se quiser mantê-los.

## Importante
Os registros ficam no armazenamento local do navegador (localStorage), não em uma conta na nuvem. Limpar os dados do Chrome, desinstalar/limpar dados do app ou perder o aparelho pode apagar os registros; o backup exportado é a proteção. Evite abrir o app em abas anônimas.

## Limitações
Esta entrega é uma PWA instalável, não um APK Android e não inclui widget nativo de tela inicial. Um widget nativo exige um projeto Android (Kotlin/Java) e compilação/assinatura de APK. O atalho da PWA é o caminho mais simples para manter a ferramenta acessível na tela inicial.
