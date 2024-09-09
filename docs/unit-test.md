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

## Exemplo com testes unitários com Python

O método de desenvolvimento orientado a testes — ou Test-Driven Development (TDD)

Tem a premissa de que a fase de testes deve ser escrita antes do próprio código. Essa é uma prática de repetição de pequenos ciclos, que são divididos em três fases que acontecem de forma contínua: escrita dos testes, aprovação do teste, refatoração e assim por diante.

Na fase de escrita dos testes , uma pessoa desenvolvedora cria o teste com a premissa de que ele irá falhar de qualquer forma, já que não existe um código para ser validado. Na primeira fase de aprovação do teste , o código é desenvolvido de forma que ele será validado pela etapa. Já na fase de refatoração , será apresentado se o código possui alguma melhoria possível.

A ideia de criar o teste antes do próprio código pode parecer algo difícil de entender, né? No entanto, esse é um raciocínio que faz sentido se nos atentarmos a alguns pontos. Quando criamos um teste falho antes do código que será validado, garantimos que não estamos desenvolvendo um teste falso que, na prática, não esteja testando nada. Isso porque quando não temos nenhum código para ser validado, ele sempre apresentará falhas.

## Utilizando o PyTest

O PyTest é um framework de testes para Python que oferece soluções para a execução de testes, validações e produção de relatórios, além de muitas outras possibilidades. O framework é bastante utilizado por possuir uma flexibilidade razoável e funcionalidades intuitivas.

Conforme falamos anteriormente, é importante nos atentarmos ao padrão utilizado para os arquivos e métodos de testes. A partir dele, o PyTest consegue identificar quais são os arquivos que devem ser testados: quando ele é executado, é realizada uma varredura no diretório do seu projeto, em busca de arquivos e métodos de testes seguindo o padrão de nomenclatura “test_*”.

Uma das grandes funcionalidades do PyTest são as fixtures , que representam tudo o que o teste precisa para fazer o seu trabalho. Ou seja, são funções que você define para moldar uma configuração de testes personalizada. Em um nível bem simples, as funções de teste solicitam fixtures declarando como argumentos, o que torna possível utilizar diversos modelos de entrada de dados em uma função de teste, por exemplo.

test_arquivo.py

<div align="center">
    ![Funções]()
<div>

conftest.py

<div align="center">
    ![]()
<div>

arquivo.py

<div align="center">
    ![]()
<div>

Para que você consiga gerar os relatórios de cobertura, realize o comando “python -m pytest --cov” dentro do diretório de testes, ou informe o caminho do diretório logo após “ — cov”, resultando no relatório exemplificado abaixo:

```bash
python -m pytest
```



Outro caminho que você pode seguir é gerar um arquivo HTML contendo o relatório de testes. Para isso, basta executar 

```bash
python -m pytest — cov=./ — cov-report html
```

Será gerado um diretório contendo um relatório com diversos detalhes da cobertura dos testes.