## Entendendo o Hello World em Java

> Não é só rodar o código. É entender o que ele é, onde ele roda e o que acontece por trás de cada linha.

Material didático em formato de carrossel (5 slides) que explica o primeiro programa em Java além do `System.out.println`.

Feito por **gisa.dev** — feito para explicar, não só mostrar.

---

## Sobre o material

Esse material responde 3 perguntas que todo iniciante tem e quase nenhum tutorial responde direito:

**1. O que é o Hello World, de verdade?**
Não é só um programa qualquer, é um ritual desde os anos 1970 (Kernighan e Ritchie, livro de C). Ele testa com o mínimo de código se o ambiente inteiro está funcionando: editor, compilador e execução. É o menor programa "completo" em Java — já tem classe, método principal e instrução de saída.

**2. Onde isso roda?**
- **O editor de código:** Onde você escreve. VS Code, IntelliJ, Eclipse. Aqui é só texto.
- **O arquivo .java:** Salvo com o mesmo nome da classe pública (`HelloWorld.java` para `class HelloWorld`). Java exige isso.
- **O JDK:** O Java Development Kit traz o compilador (`javac`) e a JVM. Sem ele, não compila nem roda.

> **JDK = ferramentas para desenvolver. JRE = ambiente para rodar. JVM = a máquina virtual que executa. O JDK inclui os outros dois.**

**3. O que acontece nos bastidores?**

📝 http://HelloWorld.java (texto para humanos)
    ↓ javac compila
⚙️ http://HelloWorld.class (bytecode - código intermediário)
    ↓ java inicia a JVM
💻 JVM lê e executa o bytecode
    ↓
🖥️ Console: Hello, World!

O bytecode não é de nenhum sistema operacional específico. Cada JVM (Windows, Linux, Mac) traduz ele para o processador da máquina. Daí o lema: "escreva uma vez, rode em qualquer lugar".

## O código

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello, World!");
  }
}
`System.out` é o canal de saída padrão. O `println` manda o texto pra esse canal e o terminal exibe.

Como rodar
1. Compile
javac HelloWorld.java

2. Execute
java HelloWorld
Pré-requisito: ter o JDK instalado. Verifique com `java -version` e `javac -version`.

Tecnologias do material visual

O carrossel foi feito em HTML/CSS puro com estilo editorial:
- Fontes: Press Start 2P, JetBrains Mono, Inter
- Estética: pixel art cat em canvas, design minimalista com borda preta

📂 Estrutura
/01-capa - ENTENDENDO O HELLO WORLD
/02-conceito - O QUE É O HELLO WORLD DE VERDADE
/03-ambiente - ONDE ISSO RODA
/04-bastidores - O QUE ACONTECE NOS BASTIDORES
/05-fechamento - AGORA VOCÊ ENTENDE, NÃO SÓ RODOU
---

gisa.dev | java
