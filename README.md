# Trilha HTML - Dio.me

## Módulo 02 - HTML I - Conceitos Básicos

Desafio de Projeto do Módulo II da trilha de HTML da [DIO](https://www.dio.me/).

O objetivo é criar um site "quase" completo de uma **clínica médica**, aplicando
todos os assuntos vistos no módulo: **formulários**, **estruturação e formatação
de texto**, **mídias** e **tabelas**.

### A clínica escolhida

**Clínica Bem Viver** &mdash; clínica multiespecializada em São Paulo, com
atendimento em Clínica Geral, Psicologia, Pediatria e Oftalmologia.

### Estrutura do projeto

```
trilha-html-modulo-2/
├── index.html        Página Principal
├── sobre.html        Sobre a clínica
├── horario.html      Horário de Atendimento
├── contato.html      Contato
├── template.html     Modelo base (referência do desafio)
├── base.css          Estilo compartilhado por todas as páginas
├── images/
│   ├── principal.svg
│   ├── sobre.svg
│   ├── horario.svg
│   └── contato.svg
└── README.md
```

### Padrão de todas as páginas

Todas as quatro páginas seguem o mesmo esqueleto do `template.html`:

```
.wrapper
├── .menu      → menu de navegação (igual em todas as páginas)
└── .main
    ├── .header   → imagem diferente em cada página
    ├── .content  → conteúdo específico da página
    └── .footer   → informações de contato (igual em todas as páginas)
```

### Conteúdo de cada página

| Página | Header | Content |
| --- | --- | --- |
| `index.html` | `images/principal.svg` | Descrição da clínica, especialidades, diferenciais e áudio |
| `sobre.html` | `images/sobre.svg` | História, missão/visão/valores, tabela do corpo clínico |
| `horario.html` | `images/horario.svg` | Tabelas de horários, preços e convênios |
| `contato.html` | `images/contato.svg` | Telefones, endereço, iframe do Google Maps e formulário |

### Assuntos abordados nas aulas

#### Formulários

O formulário em `contato.html` utiliza:

- `type="text"` &mdash; Nome e Assunto
- `type="email"` &mdash; E-mail
- `type="tel"` &mdash; Telefone (com `pattern`)
- `type="date"` &mdash; Data de preferência
- `textarea` &mdash; Mensagem
- `select` / `option` &mdash; Especialidade e período
- `type="radio"` &mdash; Via de contato preferida
- `type="checkbox"` &mdash; Autorizações
- `button type="submit"` e `button type="reset"` &mdash; Enviar e limpar
- `fieldset` / `legend` / `label` &mdash; Agrupamento e acessibilidade
- `required`, `placeholder`, `maxlength`, `pattern` &mdash; Validação

#### Estruturação e formatação de texto

`h1` a `h6`, `p`, `strong`, `i`, `u`, `mark`, `small`, `del`, `sub`, `sup`,
`blockquote`, `abbr`, `address`, `dl` / `dt` / `dd`, `ul` / `ol` / `li`.

#### Mídias

- `img` &mdash; imagens de header em cada página
- `iframe` &mdash; mapa do Google Maps na página de contato
- `audio` &mdash; player de podcast na página principal
- `figure` / `figcaption` &mdash; legendas para mídias

#### Tabelas

Quatro tabelas com `caption`, `thead`, `tbody`, `tfoot`, `th` com `scope`,
`colspan` e `rowspan`:

1. Horário de funcionamento por serviço
2. Tabela de preços por consulta
3. Cobertura por operadora de convênio
4. Corpo clínico (página Sobre)

### Como visualizar

Abra o arquivo `index.html` no navegador:

```bash
xdg-open index.html   # Linux
```

> Não é necessário servidor local. As imagens são arquivos `.svg` versionados
> junto ao projeto, então tudo funciona offline.

### Referências

- [DIO](https://www.dio.me/)
- [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
- [MDN - Formulários HTML](https://developer.mozilla.org/pt-BR/docs/Learn/Forms)
- [Repositório original do desafio](https://github.com/digitalinnovationone/trilha-html-modulo-2)

---

Feito durante a trilha de HTML da DIO - Módulo II.
