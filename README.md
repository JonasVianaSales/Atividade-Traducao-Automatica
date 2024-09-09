# Atividade Traducao Automatica
 
### 1 - Tente valores diferentes do argumento `num_examples` na função `load_data_nmt`. Como isso afeta os tamanhos do vocabulário do idioma de origem e do idioma de destino?

A quantidade de exemplos será afetada, pois em `tokenize_nmt(text, num_examples)`, o número de exemplos coloca um limite na quantidade de vezes que o loop irá rodar, e quantas sentenças serão categorizadas, respectivamente

### 2 - O texto em alguns idiomas, como chinês e japonês, não tem indicadores de limite de palavras (por exemplo, espaço). A tokenização em nível de palavra ainda é uma boa ideia para esses casos? Por que ou por que não?

Os métodos tradicionais não irão funcionar, pois as frases são reestruturas enquanto são escritas, pois as palavras não costumam ser a junção de vários caractéres em sequência, mas sim por símbolos com seus respectivos significados. Uma técnica de tokenização seria utilizando um vocabulário pre-pronto que possui a tokenização das palavras em sentenças.