Translator App

Um site moderno de tradução de inglês para português que traduz automaticamente enquanto você digita.

🎯 Descrição

Translator App é uma aplicação web que oferece tradução instantânea de textos do inglês para português brasileiro. Diferente dos tradutores convencionais, este projeto não requer cliques adicionais - a tradução aparece automaticamente conforme você digita.

O projeto demonstra conhecimento avançado em desenvolvimento frontend com React, TypeScript e Tailwind CSS, implementando boas práticas de desenvolvimento web moderno.

✨ Funcionalidades

•
✅ Tradução Automática - Traduz enquanto você digita, sem cliques

•
✅ Interface Responsiva - Funciona perfeitamente em desktop, tablet e celular

•
✅ Modo Escuro/Claro - Alternância automática entre temas

•
✅ Copiar Tradução - Um clique para copiar para a área de transferência

•
✅ Inverter Idiomas - Troca entrada e saída para traduzir de volta

•
✅ Limpar Texto - Remove todo o texto digitado

•
✅ Contador de Caracteres - Mostra número de caracteres em tempo real

•
✅ Salvamento Automático - Salva o último texto digitado no localStorage

🚀 Como Usar

Online (Mais Fácil)

Acesse diretamente: https://translatapp-5argmbbj.manus.space

Localmente

1.
Clonar o repositório

Bash


git clone https://github.com/Thuur7/Translator_App.git
cd Translator_App





2.
Instalar dependências

Bash


pnpm install
# ou
npm install





3.
Iniciar servidor de desenvolvimento

Bash


pnpm run dev
# ou
npm run dev





4.
Abrir no navegador

Plain Text


http://localhost:3000





🛠️ Tecnologias Utilizadas

Tecnologia
Versão
Propósito
React
19
Framework para interface
TypeScript
5.6
Linguagem tipada
Tailwind CSS
4
Framework CSS
Vite
7.1
Build tool
shadcn/ui
-
Componentes UI
Radix UI
-
Primitivos de UI
Lucide React
-
Ícones SVG
Sonner
-
Notificações
MyMemory API
-
Serviço de tradução




📁 Estrutura do Projeto

Plain Text


translator-app/
├── client/
│ ├── src/
│ │ ├── pages/
│ │ │ ├── Home.tsx # Página principal
│ │ │ └── NotFound.tsx # Página 404
│ │ ├── components/
│ │ │ └── ui/ # Componentes shadcn/ui
│ │ ├── hooks/
│ │ │ └── useTranslator.ts # Hook de tradução (PRINCIPAL )
│ │ ├── contexts/
│ │ │ └── ThemeContext.tsx # Contexto de tema
│ │ ├── App.tsx # Componente raiz
│ │ ├── main.tsx # Ponto de entrada
│ │ └── index.css # Estilos globais
│ ├── index.html # HTML principal
│ └── public/ # Arquivos estáticos
├── package.json # Dependências
├── vite.config.ts # Configuração Vite
├── tsconfig.json # Configuração TypeScript
└── README.md # Este arquivo



🔑 Arquivos Principais

client/src/pages/Home.tsx

Componente principal que renderiza a interface. Contém:

•
Header com título e botão de tema

•
Painel de entrada (inglês)

•
Painel de saída (português)

•
Botões de ação (copiar, limpar, inverter)

•
Footer

client/src/hooks/useTranslator.ts ⭐

Hook customizado que gerencia toda a lógica de tradução:

•
Estado do texto de entrada e saída

•
Debounce de 300ms para otimizar requisições

•
Requisições à API de tradução

•
Salvamento em localStorage

•
Funções para copiar, limpar e inverter idiomas

client/src/contexts/ThemeContext.tsx

Contexto que fornece:

•
Estado do tema (claro/escuro)

•
Função para alternar tema

•
Sincronização com preferência do sistema

client/src/index.css

Arquivo de estilos que define:

•
Variáveis de cores em OKLCH

•
Tipografia (Geist e Inter)

•
Classes customizadas

•
Animações suaves

💡 Como Funciona

Plain Text


1. Usuário digita "Hello"
        ↓
2. onChange dispara em Home.tsx
        ↓
3. setSourceText atualiza o estado
        ↓
4. useEffect detecta mudança
        ↓
5. Timer de 300ms começa (debounce)
        ↓
6. Se usuário continuar digitando, timer reseta
        ↓
7. Se usuário parar, após 300ms:
        ↓
8. Requisição HTTP para MyMemory API
        ↓
9. API retorna "Olá"
        ↓
10. setTranslatedText atualiza estado
        ↓
11. React renderiza novamente
        ↓
12. Usuário vê "Olá" na tela



⚖️ Limitações

•
❌ Qualidade Básica: API MyMemory traduz literalmente, sem contexto

•
❌ Requer Internet: Sem conexão, não funciona

•
❌ Apenas 2 Idiomas: Suporta apenas inglês ↔ português

✅ Vantagens

•
✅ Tradução Automática: Sem necessidade de cliques

•
✅ Interface Moderna: Design profissional e responsivo

•
✅ Modo Escuro: Integrado e com transições suaves

•
✅ Funcionalidades Úteis: Copiar, inverter, limpar, contador

📊 Comparação com Concorrentes

Recurso
Google Translate
DeepL
Translator App
Tradução
✅
✅
✅
Automática
❌
❌
✅
Modo Escuro
✅
❌
✅
Responsivo
✅
✅
✅
Offline
❌
❌
❌




🔮 Melhorias Futuras




Adicionar suporte a mais idiomas




Implementar histórico de traduções




Integrar com API melhor (Google Translate, DeepL)




Adicionar tradução offline (Transformers.js)




Criar versão mobile nativa




Adicionar atalhos de teclado

📚 Documentação Adicional

•
CODIGO.md - Código principal do projeto

•
IMAGENS.md - Informações sobre as imagens

💻 Requisitos

•
Node.js 18+

•
npm ou pnpm

•
Navegador moderno (Chrome, Firefox, Safari, Edge)

📝 Licença

Este projeto é fornecido para uso pessoal e educacional.

🎓 Aprendizados Demonstrados

Este projeto demonstra:

•
✅ React Hooks (useState, useEffect, useCallback, useRef)

•
✅ TypeScript e tipagem

•
✅ CSS moderno (Tailwind CSS)

•
✅ Integração com APIs externas

•
✅ Debounce e otimização de performance

•
✅ Design responsivo

•
✅ UX/UI profissional

•
✅ Boas práticas de desenvolvimento

🔗 Links Úteis

•
Site Online: https://translatapp-5argmbbj.manus.space

•
GitHub: https://github.com/Thuur7/Translator_App

•
Autor: Thuur7

🤝 Contribuições

Contribuições são bem-vindas! Sinta-se livre para:

•
Reportar bugs

•
Sugerir melhorias

•
Fazer pull requests

📞 Suporte

Se tiver dúvidas ou problemas:

1.
Verifique a documentação

2.
Abra uma issue no GitHub

3.
Consulte o arquivo CODIGO.md para entender a implementação
