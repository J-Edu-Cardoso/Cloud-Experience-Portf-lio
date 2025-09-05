# CloudPortfolio | Portfólio Profissional em Cloud e DevOps

Este é o portfólio profissional de Eduardo Cardoso, destacando experiências e habilidades em tecnologias de nuvem, especialmente AWS, com foco em arquitetura de soluções escaláveis e seguras.

## 🚀 Recursos Principais

- **PWA (Progressive Web App)**: Instalável em dispositivos móveis e desktop
- **Otimizado para Performance**: Carregamento rápido mesmo em conexões lentas
- **Offline-First**: Funcionalidade offline com Service Worker
- **Design Responsivo**: Adapta-se a qualquer tamanho de tela
- **Acessibilidade**: Desenvolvido seguindo as melhores práticas de acessibilidade

## 🛠️ Tecnologias Utilizadas

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Estilização**: Tailwind CSS
- **Ícones**: Font Awesome (auto-hospedado)
- **Fontes**: Inter e JetBrains Mono (auto-hospedadas)
- **Otimização**: Service Worker, Cache API, Lazy Loading
- **Analytics**: Google Analytics

## 🚀 Como Executar Localmente

1. **Pré-requisitos**:
   - Navegador moderno (Chrome, Firefox, Edge, Safari)
   - Node.js (opcional, apenas para desenvolvimento)

2. **Método 1 - Servidor Simples**:
   - Basta abrir o arquivo `index.html` diretamente no navegador
   - Ou use o Live Server do VS Code

3. **Método 2 - Com Node.js**:
   ```bash
   # Instale o http-server globalmente (se ainda não tiver)
   npm install -g http-server
   
   # Navegue até a pasta do projeto e execute
   http-server -p 3000
   ```
   - Acesse: http://localhost:3000

## 📦 Estrutura do Projeto

```
cloudportfolio/
├── assets/
│   ├── css/
│   │   ├── styles.css
│   │   └── tailwind.min.css
│   ├── fonts/
│   │   ├── fontawesome/
│   │   ├── inter/
│   │   └── jetbrains-mono/
│   ├── img/
│   └── js/
│       ├── main.js
│       └── pwa.js
├── index.html
├── offline.html
├── manifest.json
├── sw.js
└── README.md
```

## Estrutura do Projeto

- `index.html` - Página principal do portfólio
- `src/img/` - Diretório contendo imagens utilizadas no site

## 🚀 Deploy

Este site pode ser facilmente implantado em qualquer serviço de hospedagem estática:

- **Vercel**: [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=YOUR_REPO_URL)
- **Netlify**: [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=YOUR_REPO_URL)
- **GitHub Pages**: Configuração simples via Actions
- **AWS Amplify/S3**: Ideal para integração com serviços AWS
- **Firebase Hosting**: Excelente para PWAs

### Configurações Recomendadas para Deploy

1. **Headers de Cache**:
   ```
   Cache-Control: public, max-age=31536000, immutable  # Para assets estáticos
   Cache-Control: no-cache                             # Para HTML
   ```

2. **Compressão**: Ative Gzip/Brotli
3. **Redirecionamentos**: Configure SPA fallback para `index.html`

## ⚡ Otimizações de Desempenho

- **Carregamento Otimizado de Fontes**:
  - Fontes auto-hospedadas com `font-display: swap`
  - Pré-carregamento de fontes críticas

- **Otimização de Imagens**:
  - Formato WebP com fallback
  - Lazy loading nativo
  - Tamanhos responsivos com `srcset`

- **Service Worker**:
  - Estratégia Cache First para assets estáticos
  - Estratégia Network First para navegação
  - Página offline personalizada

- **Outras Otimizações**:
  - CSS crítico inline
  - JavaScript assíncrono/defer
  - Pré-conexão com domínios de terceiros
  - Pré-carregamento de recursos críticos

## 📱 PWA (Progressive Web App)

Este site é um PWA completo com:

- **Instalação em Dispositivos**: Adicione à tela inicial
- **Funcionamento Offline**: Acesse conteúdo mesmo sem conexão
- **Atualizações Automáticas**: Notifica sobre novas versões
- **Tema de Cores**: Adapta-se às preferências do sistema

## 🔍 SEO e Metadados

- Meta tags Open Graph para compartilhamento
- Schema.org markup para rich snippets
- Sitemap.xml gerado dinamicamente
- Robots.txt configurado

## 📊 Estatísticas

O site inclui integração com Google Analytics para métricas de desempenho e uso. O código de rastreamento pode ser configurado no arquivo `index.html`.
=======
# CloudPortfolio | Exemplo de Portfólio Cloud , Desenvolvedor e DevOps

## Sobre o Projeto
CloudPortfolio é um portfólio educacional criado como exemplo para desenvolvedores iniciantes em Cloud e DevOps. Ele demonstra a importância de ter um portfólio para o mercado de tecnologia, mostrando habilidades práticas em AWS, infraestrutura como código, e desenvolvimento web moderno.

Ter um portfólio ajuda você a:

- Demonstrar habilidades práticas para recrutadores e clientes.
- Destacar projetos reais e desafios resolvidos.
- Diferenciar-se no mercado competitivo de Cloud e DevOps.

---

## Objetivo Educacional
Este projeto tem caráter **100% educacional** e visa:

- Consolidar conhecimentos em AWS e serviços cloud.
- Criar uma aplicação web funcional e profissional para exibir projetos pessoais.

---

## Tecnologias Utilizadas

![HTML](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) 
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?logo=tailwind-css&logoColor=white)
![S3](https://img.shields.io/badge/AWS-S3-blue?logo=amazon-aws&logoColor=white) 
---

## Estrutura do Projeto
O CloudPortfolio contém:

- **Seção Hero**: Apresentação do desenvolvedor e habilidades.  
- **Seção Skills**: Ícones e descrições das habilidades técnicas.  
- **Seção Projetos**: Lista de projetos com links e imagens.  
- **Seção Contato**: Formulário e links de redes sociais.  

💡 **Dica:** Organize seus projetos em cards visuais, mostrando tecnologias usadas, desafios resolvidos e resultados obtidos.

---

## Hospedagem do Portfólio

Você pode hospedar seu portfólio de duas formas principais:

### 1️⃣ Vercel
1. Crie uma conta em [Vercel](https://vercel.com/).  
2. Conecte seu repositório GitHub.  
3. Configure o projeto e clique em **Deploy**.  
4. O Vercel gera uma URL pública automaticamente.

### 2️⃣ Amazon S3
1. Crie um **bucket S3** público.  
2. Faça upload do seu site estático (HTML, CSS, JS).  
3. Habilite **Static Website Hosting** no bucket.  
4. Configure permissões de leitura pública.  
5. Seu site estará disponível via URL do S3.

## 🪣 Passo a Passo: Hospedagem no Amazon S3

1. **Criar um Bucket**
   - Acesse o console da AWS > S3 > **Create bucket**.
   - Dê um nome único e selecione a região.
   - Desmarque a opção **Block all public access** para permitir acesso público.
   - Clique em **Create bucket**.

2. **Upload dos Arquivos**
   - Clique no bucket criado > **Upload** > **Add files**.
   - Selecione todos os arquivos do portfólio (`index.html`, `css`, `js`, `imagens`).
   - Clique em **Upload**.

3. **Configurar como Website Estático**
   - No bucket, vá em **Properties** > **Static website hosting**.
   - Selecione **Enable**.
   - Defina o **Index document** como `index.html`.
   - Salve as alterações.

4. **Permissões de Leitura Pública**
   - Vá em **Permissions** > **Bucket Policy**.
   - Adicione a seguinte política, substituindo `NOME_DO_BUCKET` pelo seu bucket:

   ```json
   {
       "Version": "2012-10-17",
       "Statement": [
           {
               "Sid": "PublicReadGetObject",
               "Effect": "Allow",
               "Principal": "*",
               "Action": "s3:GetObject",
               "Resource": "arn:aws:s3:::NOME_DO_BUCKET/*"
           }
       ]
   }
   
   ```
   - **Salve a política.**

5. **Acessar o Portfólio**

   - Vá em Properties > Static website hosting.

   - Copie a URL pública fornecida pelo S3.

   - Abra no navegador para verificar seu portfólio online.
   - Acesse diretamente: 🪣  [CloudPortfolio no S3](http://cloudportfolio1.s3-website-us-east-1.amazonaws.com)
---

## Dicas para Alunos
- Mantenha o portfólio **atualizado com projetos recentes**.  
- Documente cada projeto com **README, imagens e tecnologias utilizadas**.  
- Use **GitHub Pages, Vercel ou S3** para criar visibilidade online.  

---

## Licença
Este projeto é **livre para fins educacionais**.  
Não utilize para fins comerciais sem autorização.

---

## Autor
🧑‍🏫 **Heberton Geovane**  
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/heberton-geovane/)

---

## Conclusão
Um portfólio bem estruturado mostra suas habilidades práticas e ajuda você a se destacar no mercado de Cloud , Desensenvolvedor e DevOps. Comece pequeno, documente cada projeto e evolua com novas tecnologias! 🚀
>>>>>>> 9e7ca30ff5c33c6e17b19f3deaf2dbfaebcda7d9
