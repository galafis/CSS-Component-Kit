# CSS Component Kit

![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

Kit completo de componentes UI reutilizáveis implementados com CSS3 puro, incluindo botões, cards, modais, navegação e outros elementos essenciais para desenvolvimento web moderno.

## 🎯 Demonstração

Este projeto oferece uma biblioteca de componentes prontos para uso, facilitando o desenvolvimento de interfaces web consistentes e profissionais. Abra o `index.html` em seu navegador para ver todos os componentes em ação!

## ✨ Características

- **Componentes Modulares**: Elementos reutilizáveis e independentes
- **Design System**: Consistência visual em todos os componentes
- **CSS Puro**: Sem dependências JavaScript
- **Customizável**: Fácil personalização via CSS Variables
- **Responsivo**: Todos os componentes adaptáveis
- **Extensões**: Componentes avançados na pasta `extensions/`

## 🛠️ Tecnologias

- **HTML5**: Estrutura semântica
- **CSS3**: Flexbox, Grid, Custom Properties
- **CSS Variables**: Sistema de design tokens

## 📁 Estrutura do Projeto

```
CSS-Component-Kit/
├── index.html              # Showcase dos componentes principais
├── styles.css              # Biblioteca completa de componentes
├── extensions/             # Componentes avançados (tabs, accordions, tooltips, dark mode)
│   ├── README-EXTENSIONS.md
│   ├── accordion.html
│   ├── dark-mode.html
│   ├── tabs.html
│   └── tooltip.html
├── README.md               # Documentação principal
├── LICENSE                 # Licença MIT
└── .gitignore              # Arquivos ignorados pelo Git
```

## 🚀 Como Usar

### Instalação

**1.** Clone o repositório:

```bash
git clone https://github.com/galafis/CSS-Component-Kit.git
cd CSS-Component-Kit
```

**2.** Abra o arquivo index.html no navegador:

```bash
# Usando Python
python -m http.server 8000

# Usando Node.js
npx serve .
```

### Uso dos Componentes

#### Botões

```html
<button class="btn btn-primary">Primary Button</button>
<button class="btn btn-secondary">Secondary Button</button>
<button class="btn btn-outline">Outline Button</button>
```

#### Cards

```html
<div class="card">
  <div class="card-header">
    <h3>Card Title</h3>
  </div>
  <div class="card-body">
    <p>Card content goes here...</p>
  </div>
  <div class="card-footer">
    <button class="btn btn-primary">Action</button>
  </div>
</div>
```

#### Navigation

```html
<nav class="navbar">
  <div class="navbar-brand">Brand</div>
  <ul class="navbar-nav">
    <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
    <li class="nav-item"><a href="#" class="nav-link">About</a></li>
    <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
  </ul>
</nav>
```

## 🧩 Componentes Disponíveis

### Layout
- **Container**: Sistema de grid responsivo
- **Flexbox Utilities**: Classes utilitárias para layout
- **Grid System**: `.grid`, `.grid-2`, `.grid-3`, `.grid-4` com responsividade
- **Spacing**: Margins e paddings padronizados (`.mt-*`, `.mb-*`, `.p-*`)

### Navegação
- **Navbar**: Barra de navegação responsiva com gradiente
- **Breadcrumb**: Navegação hierárquica
- **Pagination**: Paginação de conteúdo com estados ativos

### Conteúdo
- **Cards**: Containers de conteúdo flexíveis com header, body e footer
- **Modals**: Janelas modais overlay (CSS-only com `:target`)
- **Alerts**: Mensagens de feedback (success, warning, danger, info)
- **Badges**: Indicadores e labels coloridos

### Formulários
- **Form Controls**: Inputs, selects e textareas estilizados
- **Form Groups**: Agrupamento de campos
- **Validation**: Estados de validação (`.is-valid`, `.is-invalid`)

### Utilitários
- **Typography**: Classes para texto (`.h1`, `.h2`, `.h3`, `.text-muted`)
- **Colors**: Paleta de cores completa via CSS Variables
- **Shadows**: Efeitos de sombra (`.shadow-sm`, `.shadow-md`, `.shadow-lg`)
- **Borders**: Bordas e cantos arredondados (`.rounded`, `.rounded-full`)

## 🎨 Sistema de Design

### Cores

```css
:root {
    --primary: #667eea;
    --secondary: #764ba2;
    --success: #28a745;
    --warning: #ffc107;
    --danger: #dc3545;
    --info: #17a2b8;
    --light: #f8f9fa;
    --dark: #343a40;
}
```

### Espaçamentos

```css
:root {
    --spacing-xs: 4px;
    --spacing-sm: 8px;
    --spacing-md: 16px;
    --spacing-lg: 24px;
    --spacing-xl: 32px;
}
```

### Tipografia

```css
:root {
    --font-size-sm: 14px;
    --font-size-base: 16px;
    --font-size-lg: 18px;
    --font-size-xl: 24px;
    --font-size-xxl: 32px;
}
```

## 📱 Responsividade

Todos os componentes incluem breakpoints responsivos:

```css
/* Mobile: 320px - 767px */
/* Tablet: 768px - 1023px */
/* Desktop: 1024px+ */
```

O sistema de grid se adapta automaticamente:
- **Mobile**: Todas as colunas empilham (1 coluna)
- **Tablet**: Grid-3 e Grid-4 se tornam 2 colunas
- **Desktop**: Todas as grids mantêm suas colunas originais

## 🔧 Personalização

Customize facilmente modificando as variáveis CSS:

```css
:root {
    --primary-color: #your-color;
    --border-radius: 12px;
    --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}
```

## 🎁 Extensões Disponíveis

Na pasta `extensions/` você encontra componentes avançados:

### ✅ Tabs (Abas)
Sistema de abas puro CSS usando radio buttons e `:checked`
- Ver: `extensions/tabs.html`

### ✅ Accordion (Acordeão)
Acordeão expansível usando checkboxes
- Ver: `extensions/accordion.html`

### ✅ Tooltips
Tooltips com múltiplas posições (top, right, bottom, left)
- Ver: `extensions/tooltip.html`

### ✅ Dark Mode (Modo Escuro)
Modo escuro 100% CSS puro com toggle switch interativo
- Ver: `extensions/dark-mode.html`
- Toggle visual com ícones lua/sol
- Adaptação automática de todos os componentes
- Implementação educativa usando CSS Variables e `:checked`

Para mais detalhes, consulte `extensions/README-EXTENSIONS.md`

## 🔧 Extensões Futuras

- [ ] Animações e transições avançadas
- [ ] Componentes de data/calendar
- [ ] Charts e gráficos CSS
- [ ] Integração com frameworks JavaScript
- [ ] Sistema de temas customizáveis
- [ ] Mais variações de dark mode

## 🤝 Contribuindo

Contribuições são bem-vindas! Para adicionar novos componentes:

1. Fork o projeto
2. Crie uma branch para seu componente (`git checkout -b feature/NovoComponente`)
3. Commit suas mudanças (`git commit -m 'Adiciona novo componente'`)
4. Push para a branch (`git push origin feature/NovoComponente`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 👨‍💻 Autor

**Gabriel Demetrios Lafis**

- GitHub: [@galafis](https://github.com/galafis)
- Email: gabrieldemetrios@gmail.com

---

⭐ Se este projeto foi útil, considere deixar uma estrela!

*Desenvolvido com 💜 e CSS3 puro por Gabriel Demetrios Lafis*
