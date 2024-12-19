# Literalura - Challenge Back-end do Programa ONE

## Descrição do projeto

O Literalura é uma implementação de um catálogo de livros feitos com base em dados de uma API chamada Gutendex. A ideia é praticar o consumo de API em projetos Spring somado a persistência de dados em banco de dados relacional.

Focamos nos tópicos neste projeto, ou seja, na criação e consulta de livros e autores, presente no famoso CRUD (*Create, Read, Update and Delete*) que temos em projetos *backend*. 

Decidimos em não focar na parte de atualização/eliminação de dados pois este *challenge* é o primeiro contato prático usando Spring para os alunos da especialização *backend*. 

### Curso do challenge

Para mais informações sobre o Fórum Hub, acesso o [curso do challenge](https://cursos.alura.com.br/course/spring-boot-challenge-literalura), que também possui o quadro trello do challenge.

## Estrutura do projeto

Este projeto foca na implementação de entidades que compõe livros e autores, que são recebidos via requisições a API.

A API Gutendex é gratuita para consumo, não é necessário criar conta ou gerar chave da API, basta utilizar as URL das requisições disponíveis. Mais informações acesso o site oficial da Gutendex: https://gutendex.com/

Esta aplicação consome a API Gutendex e possui um banco de dados local PostgreSQL, com algumas funcionalidades que vimos na formação de Java e Spring Boot, em especial nos dois primeiros cursos da formação.

Nesta implementação, também trabalhamos a persistência de dados em um banco de dados relacional chamado PostgreSQL, aqui focamos apenas na construção de duas entidades que se relacionam: livros e autores.

## Tecnologias utilizadas

- Java - versão 17: https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html
- Maven - versão 4.0.0 
- Spring - versão 3.2.5: https://start.spring.io/
- PostgreSQL - versão 17.2: https://www.postgresql.org/download/
- Intellij Community (opcional): https://www.jetbrains.com/idea/download
- Dependências do Spring usadas:

  - Spring Data JPA
  - PostgreSQL Driver

## Como executar o projeto

Para executar este projeto localmente, basta criar o arquivo .jar do projeto Java. Para gerar um arquivo JAR (Java ARchive) de um projeto Java, você pode seguir diferentes métodos, dependendo das ferramentas e ambientes de desenvolvimento que estiver usando.

Aqui estão os passos básicos para gerar um JAR usando ferramentas comuns como a linha de comando e IDEs como Eclipse e IntelliJ IDEA.

### **Usando a Linha de Comando (javac e jar)**

- **Compile seu código:** Navegue até o diretório onde está seu código-fonte e compile os arquivos .java para .class usando o comando javac:

```bash
javac -d out src/com/seuProjeto/*.java
```

Neste exemplo, os arquivos .java estão na pasta `src/com/seuProjeto` e os arquivos .class gerados serão colocados na pasta `out`.

- **Crie o arquivo JAR:** Use o comando jar para criar o arquivo JAR a partir dos arquivos .class compilados:

```bash
jar cvf meuProjeto.jar -C out .
```

Este comando cria um arquivo JAR chamado `meuProjeto.jar`, contendo todos os arquivos .class do diretório `out`.

### **Usando o Eclipse**

1. Exportar como JAR:
   - Clique com o botão direito no projeto na aba **Project Explorer**.
   - Selecione **Export** e depois **Java > JAR file**.
   - Escolha os recursos que deseja exportar e o local para salvar o arquivo JAR.
   - Configure as opções de exportação conforme necessário e clique em **Finish**.

### **Usando o IntelliJ IDEA**

1. **Criar Artefato:**
   - Acesse **File > Project Structure**.
   - Na aba **Artifacts**, clique em **+** e selecione **JAR > From modules with dependencies**.
   - Escolha o módulo principal do seu projeto e configure as opções conforme necessário.
   - Clique em **OK** e depois em **Apply**.
2. **Construir o Artefato:**
   - Acesse **Build > Build Artifacts** e selecione o artefato criado.
   - Clique em **Build** para gerar o arquivo JAR.

Também é possível adicionar ferramentas de construção como **Maven** e **Gradle** ao projeto e criar o arquivo .jar usando essas ferramentas.

## Autores

- Instrutor Eric Monné: https://www.linkedin.com/in/ericmonnefo/
- Monitora Brenda Souza: https://www.linkedin.com/in/breudes/
