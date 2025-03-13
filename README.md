

---

# DesafioControleFluxo

Este projeto implementa um exercício prático sobre Controle de Fluxo em Java, com foco em validações de parâmetros e exceções personalizadas. O sistema recebe dois números inteiros via terminal, realiza verificações de validade e, com base nesses números, imprime uma sequência de mensagens. Caso o primeiro número seja maior que o segundo, uma exceção personalizada é lançada.

## Funcionalidade

O sistema recebe dois números inteiros como parâmetros do terminal. Com base nesses valores, o programa:

1. Valida se o primeiro número é maior que o segundo.
2. Se o primeiro número for maior, uma exceção personalizada `ParametrosInvalidosException` é lançada.
3. Se a validação for bem-sucedida, o programa executa um loop `for` que imprime a quantidade de mensagens correspondente à diferença entre o segundo número e o primeiro. Cada mensagem indica a impressão de um número incrementado.

### Exemplo de Execução

#### Entrada:
```
Digite o primeiro parâmetro
12
Digite o segundo parâmetro
30
```

#### Saída:
```
Imprimindo o número 1
Imprimindo o número 2
Imprimindo o número 3
...
Imprimindo o número 18
```

Se o primeiro número for maior que o segundo, será lançada a seguinte exceção:

#### Exceção:
```
O segundo parâmetro deve ser maior que o primeiro
```

## Estrutura do Projeto

O projeto é composto pelas seguintes classes:

### `Contador.java`

Esta classe contém o método `main` que é responsável por receber os parâmetros via terminal e chamar o método de contagem. Ela também trata a exceção personalizada quando o primeiro número é maior que o segundo.

### `ParametrosInvalidosException.java`

Exceção personalizada que é lançada quando o primeiro número fornecido é maior que o segundo.

### Método `contar`

Dentro da classe `Contador`, o método `contar` executa a validação e o loop para imprimir as mensagens no console.

## Como Executar o Projeto

### 1. Clonar o Repositório
Clone este repositório para sua máquina local usando o comando:

```bash
git clone https://github.com/usarnamevictor/DesafioControleFluxo.git
```

### 2. Compilar e Executar

Você pode compilar e executar o código da seguinte forma:

1. **Compilar**:

   Abra o terminal no diretório do projeto e execute:

   ```bash
   javac Contador.java ParametrosInvalidosException.java
   ```

2. **Executar**:

   Após a compilação, execute o programa com:

   ```bash
   java Contador
   ```

3. **Entrada de Dados**:

   O programa solicitará dois números inteiros. Digite o primeiro e o segundo parâmetro para que o programa realize a contagem.

### Exemplo de Execução:

Se o primeiro parâmetro for `12` e o segundo `30`, a saída será:

```
Imprimindo o número 1
Imprimindo o número 2
Imprimindo o número 3
...
Imprimindo o número 18
```

Se o primeiro parâmetro for maior que o segundo, o programa lançará a exceção:

```
O segundo parâmetro deve ser maior que o primeiro
```

## Exceção Personalizada

Caso o primeiro parâmetro seja maior que o segundo, será lançada a exceção `ParametrosInvalidosException`, com a seguinte mensagem:

```
O segundo parâmetro deve ser maior que o primeiro
```

## Tecnologias Utilizadas

- **Java**: A linguagem de programação utilizada para desenvolver este sistema.
- **Controle de Fluxo**: Exercício de loops, condicionais e exceções em Java.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

