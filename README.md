# Alarme IA

Aplicativo web instalável (PWA), em português, feito para celular.

## Recursos
- Relógio digital e data local.
- Criar, ativar, desativar e excluir alarmes.
- Repetição diária, dias úteis, fins de semana ou uma vez.
- Som de teste usando áudio do navegador.
- Pedido de permissão para notificações do navegador.
- Interface de assistente com sugestões locais demonstrativas.
- PWA com ícone, manifesto e cache offline.

## Publicar
1. Abra **Settings → Pages** no GitHub.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Selecione a branch `main` e a pasta `/ (root)`, depois salve.
4. Aguarde a publicação. O endereço costuma ser `https://diascliente95-wq.github.io/arlame-ia/`.

## Limitações importantes
- Alarmes em páginas web não são confiáveis quando o navegador/site está fechado, o sistema suspende a aba ou o celular aplica economia de bateria. Para alarmes críticos, use também o app Relógio nativo do Android.
- As notificações precisam de permissão do usuário e de um navegador compatível; elas não substituem alarmes nativos nem garantem execução em segundo plano.
- O assistente atual é uma demonstração local, não uma conexão com um modelo de IA externo.

## Conectar IA real com segurança
Crie um backend (por exemplo, função serverless) que receba a mensagem, chame o provedor de IA com a chave armazenada como variável de ambiente no servidor e devolva apenas a resposta necessária. Nunca coloque uma chave secreta no `index.html`, repositório público ou JavaScript enviado ao navegador. Adicione limites de uso e tratamento de erros antes de publicar.
