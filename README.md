# una-ihcux-lista04
# Try-Catch e Prevenção de Erros

## O que é Try-Catch

O bloco `try-catch` é uma estrutura de controle utilizada em diversas linguagens de programação para tratar exceções (erros) que podem ocorrer durante a execução do código.

* `try`: contém o código que pode gerar um erro.
* `catch`: captura e trata o erro caso ele ocorra.

### Exemplo (JavaScript)

```javascript
try {
  let resultado = 10 / 0;
  console.log(resultado);
} catch (erro) {
  console.error("Ocorreu um erro:", erro.message);
}
```

## O que são Exceções

Exceções são eventos inesperados que interrompem o fluxo normal do programa, como:

* Divisão por zero
* Acesso a propriedades inexistentes
* Falhas de conexão
* Entrada de dados inválida

## Conexão com a Prevenção de Erros

O `try-catch` não evita que erros aconteçam, mas é essencial para **prevenção de falhas críticas** e **controle do comportamento da aplicação**.

### Como ele contribui:

1. **Evita que o programa quebre**

   * Sem tratamento, erros podem encerrar a execução da aplicação.

2. **Permite respostas controladas**

   * É possível exibir mensagens amigáveis ou executar ações alternativas.

3. **Facilita o diagnóstico**

   * O erro pode ser registrado (log) para análise futura.

4. **Melhora a experiência do usuário**

   * O sistema continua funcional mesmo diante de falhas.

## Boas Práticas

* Use `try-catch` apenas onde erros são esperados.
* Não utilize como substituto de validações.
* Sempre trate ou registre o erro capturado.
* Evite blocos `catch` vazios.

## Conclusão

O `try-catch` é uma ferramenta fundamental para tornar aplicações mais robustas e resilientes. Ele não impede erros, mas permite que sejam tratados de forma segura, contribuindo diretamente para a prevenção de falhas graves no sistema.
