# Contribuir com o Guia da TI

Prefere não editar arquivos? Use o [formulário de sugestão](https://github.com/LucasPedruo/guia-da-ti-dados/issues/new?template=recurso.yml). Um mantenedor poderá transformar sua sugestão em PR.

1. Faça fork de `LucasPedruo/guia-da-ti-dados` e crie uma branch.
2. Copie um modelo de `templates/` para `data/<tipo>/<slug>.json`, usando a taxonomia de `taxonomy/index.json`. Remova `demo` ao cadastrar um recurso real e substitua os valores fictícios.
3. Informe apenas dados verificáveis. Não copie textos protegidos, dados pessoais privados, HTML ou scripts. Não invente informações ausentes.
4. Use a URL oficial HTTPS. Procure por nome e URL antes de criar um cadastro; atualize o existente se já houver.
5. Execute `npm ci`, `npm run format`, `npm run validate` e `npm test`.
6. Abra um PR com a fonte das informações e aguarde revisão.

Os arquivos com `demo: true` são exemplos fictícios. Não use essa marca para recursos reais. A verificação automática valida formato e referências; a revisão humana confirma legitimidade, URLs, imagens e conteúdo.
