---
title: "Variáveis de Ambiente"
nav_order: 3
parent: "Arquitetura — CPO"
---

Configurar variáveis de ambiente durante o runtime de um container, ao invés de codificá-las diretamente no container. Isso é uma boa prática, especialmente quando você tem informações sensíveis ou configurações que podem mudar entre ambientes (desenvolvimento, teste, produção, etc.).

Ao seguir estas etapas e práticas recomendadas, você pode manter sua aplicação flexível e suas informações sensíveis seguras:

1. **Defina as Variáveis de Ambiente em seu Código**

   No seu código React com Vite, você deve prefixar suas variáveis de ambiente com VITE_ para que elas sejam expostas à sua aplicação no lado do cliente. Por exemplo, para usar uma variável de ambiente chamada API_URL, você a chamaria de VITE_API_URL em seus arquivos de configuração e, em seguida, a acessaria em seu código JavaScript/TypeScript com import.meta.env.VITE_API_URL.

2. **Dockerfile**

   No seu Dockerfile, enquanto você constrói a imagem, você não precisa definir as variáveis de ambiente. No entanto, se você quiser definir valores padrão, pode fazer algo assim:
   ```dockerfile
   ENV NOME_DA_VARIAVEL valor_default
   ```

3. **Executando o Container**

   Quando você executa seu container, pode definir variáveis de ambiente usando o flag `-e`:
   ```bash
   docker run -e "NOME_DA_VARIAVEL=valor" nome_da_imagem
   ```
   Se você tiver muitas variáveis de ambiente, pode ser útil colocá-las em um arquivo e usar o flag `--env-file`:
   ```bash
   docker run --env-file ./path_to_env_file nome_da_imagem
   ```

4. **Orquestradores como Kubernetes**

   Se você estiver usando Kubernetes ou outro orquestrador, haverá uma maneira diferente de definir variáveis de ambiente. No Kubernetes, por exemplo, você usaria a seção `env` em sua definição de pod.

5. **Lembre-se de Não Versionar Arquivos Sensíveis**

   Se você estiver usando um arquivo para armazenar variáveis de ambiente (como um `.env`), certifique-se de que ele não seja versionado (por exemplo, adicione-o ao `.gitignore` se estiver usando Git). Isso é crucial para manter segredos e chaves API fora do controle de versão.

6. **Configurações Runtime vs. Build Time**

   Lembre-se de que a configuração no runtime é diferente da configuração no build time. Se você define variáveis de ambiente durante a construção da imagem Docker, elas são "assadas" na imagem e não podem ser alteradas no runtime sem reconstruir a imagem. Por isso, é útil para configurações que mudam entre ambientes para defini-las no runtime.

