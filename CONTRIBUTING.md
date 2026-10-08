# Como contribuir

Convenções válidas para todos os repositórios da Metrol Tecnologia. O README de cada repositório pode complementar estas regras.

## Branches

Use `tipo/descricao-curta`, em kebab-case. Tipos aceitos:

| Tipo | Uso |
|---|---|
| `feat` | funcionalidade nova |
| `fix` | correção de bug |
| `docs` | documentação |
| `test` | testes |
| `refactor` | reestruturação sem mudar comportamento |
| `chore` | manutenção, dependências, configuração |
| `ci` | pipelines e automações |
| `experiment` | prova de conceito que pode ser descartada |

Exemplo: `fix/calculo-ferias-proporcionais`.

## Commits

[Conventional Commits](https://www.conventionalcommits.org/pt-br/) em português: `tipo: descrição no imperativo`.

```text
feat: adiciona exportação de holerite em PDF
fix: corrige arredondamento do banco de horas
```

Repositórios com prefixos próprios devem documentá-los no README. Exemplo: o firmware usa `master:`, `slave:` e `docs:`.

## Pull requests

- Abra um PR para mudanças que afetam produção ou que outra pessoa deveria revisar.
- Espere o CI ficar verde antes do merge. Ainda não é obrigatório, mas passará a ser quando a org migrar para o GitHub Team.
- Prefira squash merge, para que cada PR vire um commit na `main`.

## Segredos

- Nunca commite `.env`, chaves, senhas ou tokens.
- Segredos usados no CI ficam em **Settings → Secrets and variables → Actions** do repositório.
- Se um segredo vazar num commit, avise o time e troque o segredo. Apagar o commit não basta.

## Repositórios novos

- Nome `metrol-<nome>` em kebab-case.
- Visibilidade privada, salvo decisão explícita.
- Um topic de área (`area-web`, `area-embarcados`, `area-pesquisa-ia`, `area-plataforma`) e um de status (`status-prototipo`, `status-desenvolvimento`, `status-pesquisa`, `status-producao`).
