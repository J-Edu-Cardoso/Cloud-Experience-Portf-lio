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
