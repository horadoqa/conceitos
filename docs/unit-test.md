# Testes de Unidade (Unit Tests)

Na base da pirâmide, temos os testes de unidade. 

Esses testes se concentram na validação das unidades individuais de código, como funções ou métodos. Eles são altamente específicos, cobrindo pequenas partes do código, e são geralmente escritos pelos desenvolvedores. Testes de unidade são executados rapidamente e frequentemente, permitindo a detecção precoce de erros e a manutenção da qualidade do código.

Como funciona um teste unitário?

Os testes unitários são escritos pelos próprios desenvolvedores e são executados sempre que o código é modificado. Se algum erro for encontrado, o teste identificará uma falha e o desenvolvedor poderá corrigir o problema antes que ele se torne um erro maior. Isso é extremamente importante, pois permite que os erros sejam corrigidos de forma mais eficiente e ágil, evitando problemas mais sérios no futuro.

É possível realizar testes unitários de forma eficiente e garantir a qualidade do código, ao seguir os passos básicos abaixo:

- Defina o objetivo:

    Antes de escrever um teste unitário, é importante entender o que se deseja testar e o que se espera que aconteça.

- Escreva o código:

    Redija o código que será testado, garantindo que ele esteja claro, conciso e facilmente testável.

- Escreva o teste:

    Redija o teste unitário que verificará o comportamento do código. O teste deve ser escrito para garantir que o resultado esperado seja claramente definido.

- Execute o teste:

    Execute o teste unitário e verifique se o resultado corresponde ao esperado.

- Analise dos resultados:

    Se o resultado não for o esperado, corrija o código e execute o teste novamente. Se o resultado for o esperado, o teste unitário pode ser considerado concluído.

Ferramentas:
- JUnit (Java)
- NUnit (C#)
- pytest (Python)
- Jasmine (JavaScript)
- GO

É importante lembrar que a escolha da ferramenta ou framework adequado para os testes unitários depende das necessidades específicas do projeto e da linguagem de programação utilizada. Além das mencionadas, há uma variedade de outras opções disponíveis, cada uma com suas vantagens e características únicas.

Exemplo com testes unitários com Python

O método de desenvolvimento orientado a testes — ou Test-Driven Development (TDD)

Tem a premissa de que a fase de testes deve ser escrita antes do próprio código. Essa é uma prática de repetição de pequenos ciclos, que são divididos em três fases que acontecem de forma contínua: escrita dos testes, aprovação do teste, refatoração e assim por diante.

fruit.py




test_fruit.py

Para que você consiga gerar os relatórios de cobertura, realize o comando “python -m pytest — cov” dentro do diretório de testes, ou informe o caminho do diretório logo após “ — cov”, resultando no relatório exemplificado abaixo:

```bash
python -m pytest — cov
```
Outro caminho que você pode seguir é gerar um arquivo HTML contendo o relatório de testes. Para isso, basta executar 

```bash
python -m pytest — cov=./ — cov-report html
```

Será gerado um diretório contendo um relatório com diversos detalhes da cobertura dos testes.