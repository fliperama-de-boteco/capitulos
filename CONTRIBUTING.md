# Como contribuir

Você pode contribuir fazendo uma bifurcação (_fork_) desse repositório e enviando um _Pull Request_ (PR) com novos capítulos para os nossos episódios.

Caso você não tenha experiência com GitHub e Pull Requests, você pode aprender com [esse guia](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

Se por algum motivo você não quiser usar Pull Requests, você pode propor a criação de capítulos usando _issues_ no GitHub. Clique [aqui](https://github.com/fliperama-de-boteco/capitulos/issues/new/choose) para criar uma issue.

## Como adicionar capítulos

Você pode editar os capítulos já existentes na pasta [capitulos](./capitulos), ou criar novos arquivos de capítulos para os episódios que ainda não possuem capítulos.

Se criar novos arquivos, use a seguinte convenção de nomenclatura:

```
ep-<número do episódio>-<título>.json
```

Exemplos:
- `ep-299-gex.json`
- `ep-300-entrevista-stefano-arnhold.json`

Ainda à definir: Nomenclatura para as séries (Rádio, Bora pro Fliper, etc...)

### Formato dos arquivos

Os arquivos são no formato JSON e seguem a definição `podcast:chapters` (veja as referências).

Veja o exemplo (`startTime` em segundos):

```json
{
	"version": "1.2.0",
	"chapters": [
		{
			"startTime": 0,
			"title": "Abertura"
		},
		{
			"startTime": 1117,
			"title": "Vinheta"
		},
		{
			"startTime": 1156,
			"title": "Vamos pra pauta!"
		},
		{
			"startTime": 6938,
			"title": "Disclaimers"
		}
	]
}
```

### Capítulos padrão

- Abertura
- Vinheta (Recardos do Guilherme)
- Assunto Principal (exemplos: _Gex_, _Dossiê Master System_)
- Disclaimers

### Referências

- [Especificação de `podcast:chapters` no _podcast_ namespace RSS](https://github.com/Podcastindex-org/podcast-namespace/blob/main/chapters/jsonChapters.md)
