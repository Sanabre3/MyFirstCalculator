# 🧮 First Calculator

Uma calculadora moderna e elegante desenvolvida com HTML, CSS e JavaScript vanilla, apresentando um design glassmorphism atraente e funcionalidade completa para operações matemáticas básicas.

## ✨ Características

- **Design Moderno**: Interface glassmorphism com efeitos de blur e transparência
- **Responsivo**: Layout adaptável para diferentes tamanhos de tela
- **Operações Básicas**: Adição, subtração, multiplicação e divisão
- **Funcionalidades Extras**: 
  - Botão Clear (C) para limpar tudo
  - Backspace (←) para apagar o último dígito
  - Visual feedback nos botões com hover e active states

## �� Design

- **Background**: Gradiente colorido (rosa, amarelo, verde-azulado)
- **Glassmorphism**: Efeitos de blur e transparência nos elementos
- **Cores**: Paleta harmoniosa com destaque para o botão de igual
- **Typography**: Fonte Dosis para uma aparência moderna

## 🚀 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e acessível
- **CSS3**: 
  - Flexbox para layout
  - Backdrop-filter para efeitos glassmorphism
  - Box-shadow para profundidade
  - Gradientes lineares
- **JavaScript ES6**: Lógica da calculadora com funções modulares

## 📁 Estrutura do Projeto

```
calculator/
│
├── index.html          # Estrutura HTML principal
├── style.css           # Estilos e design
└── script.js           # Lógica JavaScript
```

## 🛠️ Funcionalidades Implementadas

### Operações Matemáticas
- ➕ **Adição**: Soma de números
- ➖ **Subtração**: Subtração de números  
- ✖️ **Multiplicação**: Multiplicação de números
- ➗ **Divisão**: Divisão de números

### Controles
- 🔄 **Clear (C)**: Reseta todos os valores
- ⬅️ **Backspace**: Remove o último dígito inserido
- 🟰 **Igual**: Executa a operação atual

## 💻 Como Usar

1. **Clone ou baixe o projeto**
2. **Abra o arquivo `index.html`** em seu navegador
3. **Use a calculadora**:
   - Clique nos números para inserir valores
   - Clique nos operadores (+, -, ×, ÷) para selecionar operações
   - Clique em "=" para obter o resultado
   - Use "C" para limpar ou "←" para apagar

## 🔧 Código Principal

### Variáveis de Estado
```javascript
let runningTotal = 0;        // Total acumulado
let buffer = "0";            // Valor atual na tela
let previousOperator;        // Operador anterior
```

### Função Principal
```javascript
function buttonClick(value) {
    if(isNaN(value)) {
        handleSymbol(value);     // Trata símbolos
    } else {
        handleNumber(value);     // Trata números
    }
    screen.innerText = buffer;   // Atualiza display
}
```

## 🎯 Recursos Técnicos

- **Event Delegation**: Um único listener para todos os botões
- **Parsing Inteligente**: Diferenciação automática entre números e símbolos
- **Estado Persistente**: Mantém operações em cadeia
- **Validação**: Previne operações inválidas

## 🌐 Compatibilidade

- ✅ **Navegadores Modernos**: Chrome, Firefox, Safari, Edge
- ✅ **Dispositivos Móveis**: Layout responsivo
- ✅ **Performance**: JavaScript vanilla para máxima velocidade

## 📱 Layout Responsivo

O design se adapta automaticamente a diferentes tamanhos de tela mantendo a usabilidade e estética em todos os dispositivos.

## 🎨 Personalização

Para customizar cores ou layout, edite as variáveis CSS:

```css
/* Gradiente do background */
background: linear-gradient(320deg, #eb92be, #ffef78, #63c9b4);

/* Cor do botão igual */
.calc-button:last-child {
    background: #d72880;
}
```

## 🚀 Melhorias Futuras

- [ ] Suporte a números decimais
- [ ] Histórico de operações
- [ ] Temas alternativos
- [ ] Operações avançadas (raiz, potência)
- [ ] Suporte a teclado

---

**Desenvolvido com 💖 por Beto** | *Projeto de estudo em desenvolvimento front-end*
