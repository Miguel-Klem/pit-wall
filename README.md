# 🏁 Pit Wall — GP de São Paulo

Página do GP de São Paulo de Fórmula 1 (Autódromo José Carlos Pace, Interlagos), feita só com **HTML e CSS**.

Projeto de estudo da disciplina de Linguagem de Marcação (LIMA) — Desafio Pit Wall.

**Autor:** Miguel Bompadre Klem

---

## 📁 Estrutura

```text
pit-wall
├── index.html
├── styles.css
├── README.md
└── img
    └── piloto.jpg
```

> A foto `img/piloto.jpg` é a imagem de fundo do hero. Se o arquivo não estiver na pasta, o fundo fica só com o degradê e o resto da página funciona normalmente.

## 🧱 O que tem na página

| Bloco | Tag / classe | O que faz |
| :--- | :--- | :--- |
| Topo | `header.topo` | Logo, menu e botão em `flex` |
| Destaque (hero) | `section.destaque` | Título gigante, 3 números e foto de fundo |
| Zebra | `div.zebra` | Faixa roxa e branca da pista |
| Pilotos | `section#pilotos` | 22 cards em `grid` com `auto-fit` (`.grade-pilotos`) |
| Classificação | `section#classificacao` | Filtros em `flex` e tabela de 2026 com `thead` e `tbody` (25 pilotos) |
| Ingressos | `section#ingressos` | Texto + formulário com a grade de 2 colunas (`.grade-formulario`) |
| Rodapé | `footer` | Créditos com o nome do autor |

## 🎨 Conceitos usados

- **`:root` e `var()`**: paleta (preto, roxo, lilás, branco e cinza), a fonte e as cores das 11 equipes.
- **Classes de equipe** (`.equipe-ferrari`, `.equipe-mclaren`...): cada uma troca só a variável `--equipe`, usada nos cards e na tabela.
- **Nomes em português**: classes, variáveis e ids foram escritos em português (`.numero-carro`, `--preto`, `.grade-formulario`...).
- **Flexbox**: topo, hero, botões, filtros e linhas de preço.
- **Grid**: cards dos pilotos com `repeat(auto-fit, minmax(220px, 1fr))`, seção de ingressos (`1fr 1.6fr`) e `.grade-formulario` com a classe `.inteiro`.
- **Tabela**: `thead`, `tbody`, linha do líder destacada e `hover` nas linhas.
- **Formulário**: `label for`, `required`, `placeholder` e os tipos `text`, `email`, `date`, `number`, `url`, `file`, além de `select` e `textarea`.
- **Novidades do desafio**: fonte do Google Fonts (Roboto), foto de fundo com `url()` (`contain`, para a foto aparecer inteira), degradê com corte seco e zebra com `repeating-linear-gradient`.
- **Responsivo**: `@media (max-width: 768px)` para o celular.

## ▶️ Como abrir

1. Baixe ou clone o repositório.
2. Coloque a foto `piloto.jpg` dentro da pasta `img`.
3. Abra o `index.html` no navegador (a fonte precisa de internet).

Para testar no celular: `F12` e o ícone de celular no navegador.

## ⚠️ Observações

- Os botões e o formulário não enviam nada (é só front-end).
- A tabela de classificação usa os dados de 2026 (pontos, vitórias e pódios) conferidos pelo autor.
- Os preços dos ingressos são **ilustrativos**.
- Foto: Jonathan Borba, no Pexels (uso gratuito).
