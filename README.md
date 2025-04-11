# Plugin LocksAndLockpicking

LocksAndLockpicking é um plugin para Minecraft que adiciona funcionalidades para trancar portas, contêineres e outros blocos interativos. Também introduz mecânicas de arrombamento e gerenciamento de chaves para uma jogabilidade mais imersiva.

---

## Configuração

O arquivo de configuração do plugin está localizado em `src/main/resources/config.yml`. Abaixo estão as opções configuráveis:

| Opção                          | Descrição                                                                 | Valor Padrão |
|--------------------------------|---------------------------------------------------------------------------|--------------|
| `active-worlds`                | Lista de mundos onde o plugin está ativo.                                | `["world"]`  |
| `allow-lockpicking`            | Habilita ou desabilita o arrombamento.                                   | `true`       |
| `is-keychain-active`           | Habilita ou desabilita o recurso de chaveiro.                            | `true`       |
| `keychain-size`                | Número máximo de chaves que um chaveiro pode conter.                     | `9`          |
| `lockpicking-difficulty`       | Nível base de dificuldade para arrombamento.                             | `1`          |
| `door-inventory-gui-title`     | Título para a interface gráfica do inventário de portas.                 | `"\uDAFF\uDFF8\uE971"` |
| `keysmithing-table-gui-title`  | Título para a interface gráfica da mesa de chaveiro.                     | `"\uDAFF\uDFC4\uE963"` |
| `lockpick-minigame-title`      | Título para a interface gráfica do minijogo de arrombamento.             | `"\uDAFF\uDFF8\uE964"` |
| `key_smithing-table`           | Identificador para o mobiliário da mesa de chaveiro.                     | `"itemsadder:lockpick_table"` |
| `online-cops-needed-for-lockpick` | Número mínimo de jogadores com permissão de polícia online para permitir arrombamento. | `2` |

---

## Permissões

O plugin utiliza um sistema baseado em permissões para controlar o acesso às suas funcionalidades. Abaixo está uma lista de permissões:

| Permissão               | Descrição                                                                 |
|-------------------------|-------------------------------------------------------------------------|
| `lockpick.override`     | Permite ignorar todos os bloqueios e restrições.                       |
| `lockpick.pick`         | Permite que jogadores tentem arrombar fechaduras.                      |
| `lockpick.craft`        | Permite que jogadores fabriquem ferramentas de arrombamento.           |
| `lockpick.crowbar`      | Permite que jogadores fabriquem e utilizem pés de cabra.               |
| `lockpick.police`       | Marca um jogador como policial para restrições de arrombamento.        |

---

## Comandos

O plugin fornece os seguintes comandos:

| Comando                  | Descrição                                                                 |
|--------------------------|-------------------------------------------------------------------------|
| `/betterlocks`           | Comando base do plugin. Exibe instruções de uso se nenhum argumento for fornecido. |
| `/betterlocks getitems`  | Dá ao jogador itens relacionados ao plugin (ex.: ferramentas de arrombamento, chaves). |
| `/betterlocks reload`    | Recarrega a configuração do plugin.                                     |

---

## Funcionalidades

- **Portas e Contêineres Trancáveis**: Jogadores podem trancar portas e contêineres usando chaves ou cadeados.
- **Arrombamento**: Jogadores com as permissões apropriadas podem tentar arrombar fechaduras.
- **Gerenciamento de Chaveiro**: Jogadores podem armazenar várias chaves em um chaveiro para maior conveniência.
- **Fabricação Personalizada**: Receitas para ferramentas de arrombamento, chaves e cadeados estão incluídas.
- **Função de Polícia**: A presença de policiais online pode restringir tentativas de arrombamento para manter o equilíbrio.

---

## Instalação

1. Coloque o arquivo JAR do plugin na pasta `plugins` do seu servidor.
2. Inicie o servidor para gerar o arquivo de configuração padrão.
3. Edite o arquivo de configuração (`config.yml`) conforme necessário.
4. Recarregue ou reinicie o servidor para aplicar as alterações.

---

## Suporte

Para problemas ou solicitações de funcionalidades, abra uma issue no [repositório GitHub](https://github.com/your-repo/LocksAndLockpicking).
