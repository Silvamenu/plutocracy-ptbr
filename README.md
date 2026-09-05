# 🇧🇷 Plutocracy PT-BR

Tradução comunitária de **Plutocracy** para **Português do Brasil (pt-BR)**.

> Projeto não oficial criado para disponibilizar a tradução brasileira usando o próprio sistema de localização do jogo.

## 📊 Status da tradução

| Item | Status |
|---|---|
| Strings traduzidas | **6.080 / 6.103** strings únicas |
| Arquivos de tradução | **22 XML** |
| Idioma | **Português (Brasil)** |
| Codificação | **UTF-8, sem BOM** |
| Base utilizada | `translations/en` — Steam build `24362355` |

Algumas entradas permanecem propositalmente sem tradução porque são caminhos de imagens, placeholders ou valores literais usados internamente pelo jogo. Alterá-los poderia quebrar ícones ou elementos da interface.

## 📥 Como instalar

### 1. Baixe a tradução

No GitHub, clique em:

**Code → Download ZIP**

Extraia o arquivo baixado.

### 2. Abra a pasta do Plutocracy

Na Steam:

**Biblioteca → Plutocracy → botão direito → Gerenciar → Explorar arquivos locais**

Normalmente o jogo estará em algo parecido com:

```text
C:\Program Files (x86)\Steam\steamapps\common\Plutocracy
```

### 3. Abra a pasta `translations`

Dentro da instalação do jogo, localize:

```text
Plutocracy\translations\
```

### 4. Copie a pasta `pt`

Copie **somente a pasta `pt` deste repositório** para a pasta `translations` do jogo.

O resultado deve ficar assim:

```text
Plutocracy\
└── translations\
    ├── en\
    ├── ...
    └── pt\
        ├── lang.xml
        ├── gui.xml
        ├── story.xml
        ├── wiki.xml
        └── demais arquivos XML
```

> ⚠️ Não coloque a pasta do repositório inteiro dentro de `translations`. A pasta que precisa estar ali é diretamente a **`pt`**.

### 5. Selecione o idioma no jogo

Abra o **Plutocracy**, acesse as opções de idioma e selecione:

**Português (Brasil)**

O arquivo `pt/lang.xml` registra esse idioma para o sistema de localização do jogo.

## 🔄 Atualizações do jogo

A Steam pode substituir ou alterar arquivos durante atualizações do Plutocracy.

Se a tradução deixar de funcionar depois de uma atualização:

1. baixe novamente a versão mais recente deste repositório;
2. copie novamente a pasta `pt` para `Plutocracy\translations\`;
3. substitua os arquivos quando solicitado.

Também recomendamos manter uma cópia da pasta `pt` fora do diretório do jogo.

## ♻️ Como remover a tradução

Feche o jogo e remova:

```text
Plutocracy\translations\pt
```

Se houver qualquer problema com os arquivos do jogo, use na Steam:

**Plutocracy → Propriedades → Arquivos instalados → Verificar integridade dos arquivos**

## 🧪 Qualidade da tradução

A tradução foi criada diretamente a partir de `translations/en`, evitando tradução indireta por outro idioma.

Foram preservados elementos técnicos importantes, incluindo:

- placeholders posicionais como `%1`, `%2` e `%3`;
- placeholders nomeados como `{person}`, `{company_name}` e `{date}`;
- markup escapado em XML;
- sequências como `\n` e `\r\n`;
- formas plurais separadas por `;`;
- caminhos internos de imagens que não devem ser traduzidos.

As verificações realizadas incluem correspondência da quantidade de atributos `value`, preservação de tokens e placeholders, validação de caracteres escapados e arquivos XML em UTF-8.

## 🛠️ Como contribuir

Encontrou:

- texto cortado na interface;
- erro de digitação;
- tradução estranha;
- termo inconsistente;
- frase ainda em inglês?

Abra uma **Issue** informando onde o texto aparece. Se possível, inclua uma captura de tela.

Pull Requests também são bem-vindos. Ao editar os XMLs, altere apenas o conteúdo traduzível e **não modifique placeholders, tags ou referências internas do jogo**.

## 📁 Estrutura

```text
plutocracy-ptbr/
├── README.md
└── pt/
    ├── lang.xml
    ├── agents.xml
    ├── authority_settings.xml
    ├── citations.xml
    ├── company_settings.xml
    ├── company_technologies.xml
    ├── crimes.xml
    ├── discussion_dialog.xml
    ├── game_events.xml
    ├── google_breakpad.xml
    ├── gui.xml
    ├── hints.xml
    ├── images.xml
    ├── laws.xml
    ├── persons_characters.xml
    ├── player_achievements_description.xml
    ├── random_events.xml
    ├── sandbox_settings.xml
    ├── story.xml
    ├── usa_desc.xml
    ├── wiki.xml
    └── demais arquivos da localização
```

## ⚖️ Aviso

Este é um projeto comunitário e **não oficial**.

**Plutocracy** e todo o conteúdo original do jogo pertencem aos seus respectivos desenvolvedores e detentores de direitos. Este repositório contém apenas arquivos relacionados à tradução e exige uma cópia legítima do jogo para utilização.

## ❤️ Créditos

Tradução para Português do Brasil mantida pela comunidade.

**Plutocracy** é desenvolvido pela **Redwood Games**.