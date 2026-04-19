1. Por que a Secret aparece como ***?
Porque o GitHub Actions mascara automaticamente secrets por segurança, evitando expor dados sensíveis. Já variáveis comuns aparecem normalmente.

2. O Job 2 consegue ler BUILD_VERSION do Job 1? Por quê?
Não. Porque variáveis de job só existem dentro do próprio job. Cada job roda em um ambiente isolado, então não compartilham variáveis automaticamente.