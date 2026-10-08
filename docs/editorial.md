# Como escrever um cadastro

- Use uma descrição curta e concreta do que a pessoa vai encontrar.
- Informe apenas o que pode ser conferido na fonte oficial.
- Não use rankings, superlativos ou promessas de emprego.
- Não copie textos protegidos nem publique dados pessoais privados.
- Não inclua HTML, scripts ou imagens externas nesta versão.
- Escolha IDs existentes em `taxonomy/index.json`.
- Use `countries` (ISO 3166-1 alpha-2, como `US`) para associar o recurso ao seu contexto/público quando puder confirmar. País não é inferido pelo idioma.
- Atualize `updatedAt` quando revisar o conteúdo.
- Pesquise nome e URL antes de adicionar. Corrija o cadastro existente quando houver duplicação.

Campos próprios de cada categoria entrarão gradualmente. Não invente localização para recursos online nem preencha campos ausentes por suposição.

## Localização de comunidades

Use `communityLocation` somente em comunidades. Informe o alcance confirmado:

- `regional`, com `states` para as siglas de UFs oficiais, por exemplo `["SP", "RJ"]`.
- `national`, para atuação em todo o Brasil.
- `international`, para comunidades globais ou de fora do Brasil.

Nacional e internacional não usam `states`. Idioma e país não definem o alcance automaticamente. Os cadastros antigos sem este campo continuam válidos, mas não aparecem nos filtros por localização até serem revisados.

Novas sugestões de comunidades exigem a categoria em `areas`, `communityPlatforms` (uma ou várias plataformas do schema), `communityLinks` (um link público HTTPS para cada plataforma marcada), `communityAudience` (`general`, `male`, `female` ou `lgbt`) e `communityModality` (`online`, `in-person` ou `hybrid`). Plataforma é onde a comunidade conversa ou mantém seu espaço público. Modalidade descreve como os encontros acontecem. Um grupo presencial também pode usar WhatsApp.

Classifique o público pela proposta declarada pela comunidade. Não presuma gênero ou orientação dos participantes. Uma comunidade geral não é masculina. Links de plataformas não podem repetir a mesma plataforma nem incluir opções que não estejam em `communityPlatforms`. Registros antigos sem esses campos continuam válidos para migração e aparecem sem filtros. Campos ausentes não recebem classificação presumida. A FullDev aparece primeiro quando atende aos filtros. As demais comunidades são ordenadas alfabeticamente.

## Categorias de conteúdo dos criadores

Perfis em creators e youtube usam creatorCategories para os tipos de conteúdo, separadamente de areas (assuntos técnicos). Os valores disponíveis são education (Tutoriais e educação), career (Carreira), humor (Humor), lifestyle (Estilo de vida), news (Notícias), reviews (Análises e opiniões), projects (Projetos e bastidores) e other (Outra). Você pode escolher várias categorias, sem repetir a mesma opção.

O formulário do Guia exige pelo menos uma categoria ao sugerir um perfil. Confirme as categorias com o conteúdo público do criador. Não deduza Humor ou Estilo de vida apenas por popularidade. Cadastros antigos sem classificação continuam válidos e aparecem como Categoria não informada até a revisão.

## Quantidade de membros

`communityMembers` é opcional e exclusivo de comunidades. Informe `count` (inteiro não negativo), `checkedAt` (data da informação) e `moreThan: true` quando a informação for “mais de” esse número. Não preencha zero para representar um dado desconhecido. Não some contagens de plataformas diferentes como se fossem pessoas únicas. A contagem é informada e revisada, não um contador ao vivo.
