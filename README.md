# SixMe — site público

Site institucional estático da SixMe para apresentação da integração com Google Drive e disponibilização de links públicos no Google Auth Platform / OAuth consent screen.

## URLs de produção

- Início: https://www.sixme.com.br/
- Privacidade: https://www.sixme.com.br/privacidade/
- Termos: https://www.sixme.com.br/termos/

Hospedagem: Railway, serviço conectado ao branch `main` deste repositório para deploy automático a cada push. Arquivos HTML e CSS sem build ou variáveis secretas.

## DNS / Locaweb

Cadastrar no painel de zona DNS os registros CNAME e TXT **exatos** emitidos pelo Railway para `www.sixme.com.br`. O domínio raiz `sixme.com.br` exige redirecionamento HTTP para o `www` ou DNS com suporte a CNAME flattening / ALIAS; Locaweb não oferece esse recurso para o apex. Não criar registro A arbitrário nem substituir MX/TXT de e-mail.

## Antes de enviar ao Google para verificação

- Confirmar que `privacidade@sixme.com.br` recebe mensagens.
- Revisar a política contra os escopos OAuth realmente solicitados, fluxos de acesso, fornecedores e prazos reais de retenção/exclusão.
- Verificar propriedade de `sixme.com.br` no Google Search Console.
- Inserir as três URLs acima na configuração de branding do app OAuth.
- Validar HTTPS e acesso público sem login.
