# 🚗 Carro - Análise de Preços por Ano

Projeto Java simples que modela um carro e realiza análise de preços ao longo de 3 anos, identificando o maior e o menor valor registrado.

---

## 📋 Descrição

Este projeto contém duas classes:

- **`Carro`** — Representa um modelo de carro com preços registrados em 3 anos distintos, além de métodos para calcular o menor e o maior preço do período.
- **`ModeloCarro`** — Classe principal que instancia um objeto `Carro`, define seus dados e exibe os resultados no console.

---

## 🗂️ Estrutura do Projeto

```
📦 projeto
 ┣ 📄 Carro.java
 ┗ 📄 ModeloCarro.java
```

---

## 🧩 Classe `Carro`

### Atributos

| Atributo       | Tipo     | Descrição                        |
|----------------|----------|----------------------------------|
| `nomeModelo`   | `String` | Nome do modelo do carro          |
| `precoAno1`    | `double` | Preço registrado no 1º ano       |
| `precoAno2`    | `double` | Preço registrado no 2º ano       |
| `precoAno3`    | `double` | Preço registrado no 3º ano       |

### Métodos

| Método                  | Retorno  | Descrição                                        |
|-------------------------|----------|--------------------------------------------------|
| `getNomeModelo()`       | `String` | Retorna o nome do modelo                         |
| `setNomeModelo(String)` | `void`   | Define o nome do modelo                          |
| `getPrecoAno1()`        | `double` | Retorna o preço do 1º ano                        |
| `setPrecoAno1(double)`  | `void`   | Define o preço do 1º ano                         |
| `getPrecoAno2()`        | `double` | Retorna o preço do 2º ano                        |
| `setPrecoAno2(double)`  | `void`   | Define o preço do 2º ano                         |
| `getPrecoAno3()`        | `double` | Retorna o preço do 3º ano                        |
| `setPrecoAno3(double)`  | `void`   | Define o preço do 3º ano                         |
| `calcularMenorPreco()`  | `double` | Retorna o menor preço entre os 3 anos            |
| `calcularMaiorPreco()`  | `double` | Retorna o maior preço entre os 3 anos            |

---

## ▶️ Exemplo de Uso

```java
Carro volvo = new Carro();
volvo.setNomeModelo("Volvo");
volvo.setPrecoAno1(250);
volvo.setPrecoAno2(220);
volvo.setPrecoAno3(280);

System.out.println("Preço ano 1: " + volvo.getPrecoAno1());
System.out.println("Preço ano 2: " + volvo.getPrecoAno2());
System.out.println("Preço ano 3: " + volvo.getPrecoAno3());
System.out.println("Menor valor dos últimos 3 anos: " + volvo.calcularMenorPreco());
System.out.println("Maior valor dos últimos 3 anos: " + volvo.calcularMaiorPreco());
```

### Saída esperada

```
Preço ano 1: 250.0
Preço ano 2: 220.0
Preço ano 3: 280.0
Menor valor dos últimos 3 anos: 220.0
Maior valor dos últimos 3 anos: 280.0
```

---

## 🛠️ Como Executar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. **Compile os arquivos:**
   ```bash
   javac Carro.java ModeloCarro.java
   ```

3. **Execute a classe principal:**
   ```bash
   java ModeloCarro
   ```

---

## 📌 Requisitos

- Java JDK 8 ou superior

