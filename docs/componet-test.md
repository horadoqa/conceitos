# Teste de Componentes ()

Acima dos Testes Unitários (Unit Tests), temos o Teste de Componentes, que foca em testar unidades individuais de código, como métodos ou classes.
Geralmente é realizado por desenvolvedores para garantir que cada parte do código funcione como esperado.
Usa mocks e stubs para isolar o componente em teste.

- Objetivo: 
    
    O objetivo principal é verificar se componentes maiores, geralmente APIs, Banco de Dados, funcionam corretamente quando interagem entre si.

- Escopo: 
    
    Ao contrário dos testes unitários, os testes de componente envolvem a interação entre diferentes unidades de código ou módulos. O teste pode incluir a verificação da integração, comunicação e cooperação entre esses componentes.

- Foco: 

    Os testes de componente visam garantir que os diferentes elementos do sistema, quando combinados, produzam o comportamento desejado. Chamei a função que salva um dado no banco de dados e ela não salvou nada, o banco não aceita x tipagem de váriavel, coisas assim.