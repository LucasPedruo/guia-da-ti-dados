# Como escrever um cadastro

- Use uma descrição curta e concreta do que a pessoa vai encontrar.
- Informe apenas o que pode ser conferido na fonte oficial.
- Não use rankings, superlativos ou promessas de emprego.
- Não copie textos protegidos nem publique dados pessoais privados.
- Não inclua HTML, scripts ou imagens externas nesta versão.
- Escolha IDs existentes em `taxonomy/index.json`.
- Use `countries` (ISO 3166-1 alpha-2, como `US`) para associar o recurso ao seu contexto/público quando puder confirmar; país não é inferido pelo idioma.
- Atualize `updatedAt` quando revisar o conteúdo.
- Pesquise nome e URL antes de adicionar; corrija o cadastro existente quando houver duplicação.

Campos próprios de cada categoria entrarão gradualmente. Não invente localização para recursos online nem preencha campos ausentes por suposição.

## Localização de comunidades

Use `communityLocation` somente em comunidades. Informe o alcance confirmado: `regional` com `states` (siglas de UFs oficiais, por exemplo `["SP", "RJ"]`); `national` para atuação em todo o Brasil; ou `international` para comunidades globais ou de fora do Brasil. Nacional e internacional não usam `states`. Idioma e país não definem o alcance automaticamente. Os cadastros antigos sem este campo continuam válidos, mas não aparecem nos filtros por localização até serem revisados.

Novas sugestões de comunidades também exigem a categoria em `areas`, `communityPlatforms` (ao menos uma das plataformas do schema) e `communityModality` (`online`, `in-person` ou `hybrid`). Plataforma é o espaço usado como ninho; modalidade é como os encontros acontecem. Um grupo presencial pode usar WhatsApp como ninho. Campos antigos continuam opcionais para migração; novas sugestões no site exigem todos esses dados. Sem filtros, o site lista inclusive os cadastros ainda sem metadados.

## Categorias de conteúdo dos criadores

Perfis em creators e youtube usam creatorCategories para os tipos de conteúdo, separadamente de areas (assuntos técnicos). Os valores disponíveis são education (Tutoriais e educação), career (Carreira), humor (Humor), lifestyle (Lifestyle), news (Notícias), reviews (Análises e opiniões), projects (Projetos e bastidores) e other (Outra). É possível escolher várias categorias, sem repetições.

O formulário do Guia exige pelo menos uma categoria ao sugerir um perfil. Confirme as categorias com o conteúdo público do criador; não deduza Humor ou Lifestyle apenas por popularidade. Cadastros antigos sem classificação continuam válidos e aparecem como Categoria não informada até a revisão.
