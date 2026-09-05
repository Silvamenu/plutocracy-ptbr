# plutocracy-pt

Brazilian Portuguese (pt-BR) translation of Plutocracy.

Tradução para português brasileiro do jogo Plutocracy.

---

## Status

| | |
|---|---|
| Strings translated | **6,080 / 6,103** unique |
| Files | 22 XML |
| Source | `translations/en`, Steam build `24362355` |
| Encoding | UTF-8, no BOM |

### Intentionally left in English

| Count | What | Why |
|---|---|---|
| 23 | `image://rip/.../en_*.png` | Image asset paths. No pt-BR assets exist — translating these would break the icons. |
| 7 | `%`, `%1`, `-`, `---`, `1890`, `1900`, `1949` | Pure placeholders and literals. |

## Method

Translated from `translations/en` rather than from another localisation, so no
meaning is lost through a second-hand language.

Preserved verbatim in every string:

- positional placeholders — `%1`, `%2`, `%3`
- named placeholders — `{person}`, `{company_name}`, `{date}`, `{reputation_icon}`, …
- escaped markup — `&lt;br&gt;`, `&lt;font face='…'&gt;`, `&quot;`, `&amp;`
- literal escapes — `\n`, `\r\n`
- plural forms separated by `;` (e.g. `%1 empresa;%1 empresas;%1 empresas`)

Terminology was kept consistent across all files: agent names, company types,
skills, political offices, and the economic vocabulary (*truste*, *cartel*,
*participação de controle*, *paraquedas dourado*, and so on).

US state names use the established Brazilian Portuguese forms
(*Carolina do Norte*, *Pensilvânia*, *Luisiana*, …). Latin, French and Hawaiian
state mottos are left in the original, as in the English source; English-language
mottos and state nicknames are translated.

## QA

Every check below was run against the whole set of files and passes:

- `value="…"` attribute count is identical between `en/` and `pt/` in all 22 files
- every `{token}` placeholder appears the same number of times per file in both languages
- no unescaped `&`, `<`, `>` or `"` inside any attribute value
- all files valid UTF-8, no BOM, XML declaration intact

## Install (manual) / Instalação manual

**EN** — Copy the `pt` folder into `.../steamapps/common/Plutocracy/translations/`,
then pick **Português (Brasil)** in the game's language options.

**PT** — Copie a pasta `pt` para `.../steamapps/common/Plutocracy/translations/`
e selecione **Português (Brasil)** nas opções de idioma do jogo.

> A Steam pode sobrescrever a pasta ao atualizar o jogo. Guarde uma cópia fora do
> diretório de instalação, ou reinstale a tradução depois de cada atualização.

## Contributing / Como contribuir

Encontrou um texto cortado na interface, um termo inconsistente ou um erro de
digitação? Abra uma *issue* dizendo em que tela apareceu — de preferência com
print. Correções por *pull request* são bem-vindas: edite apenas o atributo
`value` do XML correspondente e mantenha placeholders e markup intactos.

## Credits

Translation by the community. *Plutocracy* is developed by
[Redwood Games](https://redwood-games.com). All original game text is
copyright Redwood Games; this repository contains only the translated strings
and exists to support the game's built-in localisation system.
