# Contribuir com o Guia da TI

Prefere não editar arquivos? Use o [formulário de sugestão](https://github.com/guia-da-ti/guia-da-ti-dados/issues/new?template=recurso.yml). Um mantenedor poderá transformar sua sugestão em PR.

1. Faça fork de `guia-da-ti/guia-da-ti-dados` e crie uma branch.
2. Copie um modelo de `templates/` para `data/<tipo>/<slug>.json`, usando a taxonomia de `taxonomy/index.json`. Remova `demo` ao cadastrar um recurso real e substitua os valores fictícios.
3. Informe apenas dados verificáveis. Não copie textos protegidos, dados pessoais privados, HTML ou scripts. Não invente informações ausentes.
4. Use a URL oficial HTTPS. Procure por nome e URL antes de criar um cadastro. Atualize o existente se já houver.
5. Execute `npm ci`, `npm run format`, `npm run validate` e `npm test`.
6. Abra um PR com a fonte das informações e aguarde revisão.

Para identificar recursos associados a um país, adicione `countries` com os códigos ISO de duas letras, por exemplo `"countries": ["US"]`. Marque o país do contexto ou público do recurso conforme a sua categoria e as fontes disponíveis. Não deduza o país pelo idioma. Esse campo é opcional.

Consulte os [tipos e caminhos de cadastro](docs/categories.md). As novas categorias usam o mesmo schema base. Crie a pasta do tipo quando adicionar o primeiro recurso. Uma pasta vazia não precisa de arquivo de exemplo. Não inclua arquivos `.gitkeep` dentro de `data/`, pois o validador aceita apenas registros JSON.

Os arquivos com `demo: true` são exemplos fictícios. Não use essa marca para recursos reais. A verificação automática valida formato e referências. A revisão humana confirma legitimidade, URLs, imagens e conteúdo.
