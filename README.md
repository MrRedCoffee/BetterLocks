# Plugin BetterLocks

BetterLocks é um plugin para Minecraft que adiciona funcionalidades para trancar portas e contêineres. Também introduz mecânicas de arrombamento e gerenciamento de chaves para uma jogabilidade mais imersiva.

---

## Configuração

| Opção                          | Descrição                                                                 | Valor Padrão |
|--------------------------------|---------------------------------------------------------------------------|--------------|
| `active-worlds`                | Lista de mundos onde o plugin está ativo.                                | `["world"]`  |
| `allow-lockpicking`            | Habilita ou desabilita o arrombamento.                                   | `true`       |
| `is-keychain-active`           | Habilita ou desabilita o recurso do molho de chaves.                            | `true`       |
| `keychain-size`                | Número máximo de chaves que um chaveiro pode conter.                     | `9`          |
| `door-inventory-gui-title`     | Título para a interface gráfica do inventário de portas.                 | `"\uDAFF\uDFF8\uE971"` |
| `keysmithing-table-gui-title`  | Título para a interface gráfica da mesa de chaveiro.                     | `"\uDAFF\uDFC4\uE963"` |
| `lockpick-minigame-title`      | Título para a interface gráfica do minijogo de arrombamento.             | `"\uDAFF\uDFF8\uE964"` |
| `keysmithing-table-ia-furniture` | Identificador para o mobiliário da mesa de chaveiro no ItemsAdder.       | `"itemsadder:lockpick_table"` |
| `online-cops-needed-for-lockpick` | Número mínimo de policiais online para permitir arrombamento.          | `2`          |
| `container-blacklist`          | Lista de materiais de contêineres que não podem ser trancados.           | `["furnace", "blast_furnace", "smoker"]` |

---

## Permissões

O plugin utiliza um sistema baseado em permissões para controlar o acesso às suas funcionalidades. Abaixo está uma lista de permissões:

| Permissão               | Descrição                                                                 |
|-------------------------|-------------------------------------------------------------------------|
| `lockpick.override`     | Permite ignorar todos os bloqueios e restrições.                       |
| `lockpick.pick`         | Permite que jogadores ou grupos tentem arrombar fechaduras.            |
| `lockpick.craft`        | Permite que jogadores ou grupos fabriquem ferramentas de arrombamento. |
| `lockpick.crowbar`      | Permite que jogadores ou grupos fabriquem e utilizem pés de cabra.     |
| `lockpick.police`       | Marca um jogador ou grupo como policial para restrições de arrombamento.|

---

## Comandos

O plugin fornece os seguintes comandos:

| Comando                  | Descrição                                                                 |
|--------------------------|-------------------------------------------------------------------------|
| `/betterlocks password`  | Abre a GUI do chaveiro.                                                |
| `/betterlocks getitems`  | Dá ao jogador todos os itens relacionados ao plugin.                   |
| `/betterlocks reload`    | Recarrega a configuração do plugin.                                    |

---

## Instalação

1. Coloque o arquivo JAR do plugin na pasta `plugins` do seu servidor.
2. Inicie o servidor para gerar o arquivo de configuração padrão.
3. Edite o arquivo de configuração (`config.yml`) conforme necessário.
4. Recarregue ou reinicie o servidor para aplicar as alterações.

---

## Integração com móveis do ItemsAdder

Deixei anexado um pacote de exemplo do ItemsAdder.
Coloque no servidor e mude a configuração `keysmithing-table-ia-furniture` para: `magic_store:blacksmith_table_1_2x1`.

---

## Dica

Ao deletar portas trancadas utilizando `Worldedit` ou apagar a pasta `World` as trancas da porta são mantidas no banco de dados, então deve tomar cuidado com isso.
