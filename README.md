# Analista de URLs
###
O objetivo deste projeto é otimizar a extração de informações e a síntese de conteúdos de vídeos do YouTube de forma ágil. A solução consiste em um assistente baseado em Inteligência Artificial, desenvolvido para interpretar e processar dados diretamente de URLs.

**` Escolha do Modelo de Linguagem `** <br>
Durante a fase de planejamento, foi avaliada a implementação da API da OpenAI. No entanto, o modelo GPT-4 exige um aporte financeiro inicial mínimo (créditos de $5 USD) para a ativação da chave de API.
Visando a viabilidade econômica e a redução de custos operacionais, optei pela utilização do modelo Gemini 2.5 Flash, da Google

**` Desenvolvimento e Arquitetura`** <br>
A lógica do assistente foi estruturada a partir de estudos sobre agentes de IA e análise de arquiteturas de sistemas similares, como assistentes de planejamento de viagens. Com base nessas referências, a solução foi modelada especificamente para atuar como um Analista de URLs do YouTube, capaz de processar o conteúdo audiovisual e retornar insights estruturados ao usuário.

**` Configuração `** <br>
1. Gerenciamento de Dependências<br>
O sistema depende de bibliotecas externas para o processamento de dados e integração com modelos de linguagem. Todas as especificações estão listadas no arquivo requirements.txt. Para instalá-las, utilize o gerenciador de pacotes pip:

```Bash
pip install -r requirements.txt
```

2. Configuração de Variáveis de Ambiente<br>
Por diretrizes de segurança e boas práticas de desenvolvimento, as credenciais de acesso não devem ser expostas no código-fonte. O projeto utiliza um arquivo de configuração de ambiente (.env) para gerenciar chaves sensíveis.

Criação do arquivo: Certifique-se de que o arquivo .env esteja presente na raiz do diretório.

Atribuição da Chave: Insira sua credencial da Google AI API seguindo o padrão abaixo:

```Snippet de código
GOOGLE_API_KEY=sua_chave_aqui
```

Importante: Recomenda-se a inclusão do arquivo .env no seu .gitignore para evitar a exposição inadvertida de suas credenciais em repositórios públicos.

