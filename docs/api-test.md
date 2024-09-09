# Teste de APIs (APIs Test):

O teste de API é o processo de verificar se APIs estão funcionando e apresentando o desempenho esperado. Desenvolvedores e engenheiros de controle de qualidade testam APIs enviando solicitações para vários endpoints de API e validando as respostas em relação aos resultados esperados. O objetivo é determinar se as APIs atendem aos padrões definidos de funcionalidade, desempenho, escalabilidade e segurança. Este processo inclui testar os cenários do “caminho feliz” e os casos negativos para garantir que as verificações de segurança adequadas estejam em vigor. Você pode automatizar esses testes usando uma ferramenta de teste de API.

É essencial testar a API como um todo, simulando as jornadas esperadas do usuário e as cargas do servidor para garantir que ela possa lidar com o uso no mundo real. Por exemplo, para uma jornada de usuário típica em que um usuário faz login, procura um produto e o adiciona a um carrinho, o teste de API ideal seria imitar essas etapas enviando solicitações que replicam essas ações. Como os aplicativos do mundo real costumam sofrer flutuações no tráfego de usuários, o teste também deve simular esses picos e cargas de servidor para ajudar a identificar possíveis gargalos ou lentidão.

Uma estratégia típica de teste de API especifica o número e a combinação de endpoints, os resultados esperados, o tempo de resposta ideal e os critérios para uma resposta malsucedida. Idealmente, deveria haver vários casos de teste para analisar APIs em todos os cenários possíveis. Nos últimos anos, houve uma mudança no sentido de executar esses testes mais cedo no Ciclo de vida da API para identificar e resolver problemas antes que se transformem em problemas maiores.

Tipos de Testes de APIs

- Teste funcional
    
    Os testes funcionais confirmam que uma API faz o que deveria, verificando se os endpoints processam solicitações corretamente e retornam respostas apropriadas. Inclui testar a entrada e a saída de uma API, bem como verificar seu comportamento sob diferentes condições. Também inclui a verificação de validações de parâmetros quanto à exatidão dos tipos e valores de dados, categorização de solicitações válidas ou inválidas e verificação de que mensagens de erro apropriadas são enviadas.

    Existem diferentes categorias de testes funcionais de API, incluindo:

- Teste de unidade: 
    
    Envolve o teste de um componente de uma API, como um método ou função específica.

    - Teste de integração: 
        
        Ele verifica como uma API funciona com outros componentes ou sistemas.
    
    - Teste de sistema: 
        
        Ele testa toda a API para garantir que está funcionando conforme o esperado.
    
    - Teste de tratamento de erros: 
    
        Ele garante que uma API seja capaz de lidar com todos os erros. Isso inclui testar cenários como valores de entrada ausentes ou inválidos e condições inesperadas.
    
    - Teste de performance:
    
        Como o nome sugere, o teste de desempenho avalia o desempenho de uma API em diversos fatores, como: tempo de resposta, capacidade e escalabilidade. É uma etapa fundamental para garantir que sua API possa lidar com cargas elevadas em condições exigentes.

- O teste de desempenho pode incluir:

    - Teste de carga: 
    
        Testa o desempenho de uma API sob cargas esperadas, como o número de usuários ou solicitações simultâneas.
    
    - Teste de estresse: 
        
        Testa o desempenho de uma API aumentando gradualmente a carga para identificar a capacidade máxima da API.
    
    - Teste de resistência: 
    
        Rastreia o desempenho de uma API por um longo período de tempo, como várias horas ou dias, para garantir que ela possa lidar com a carga de trabalho esperada por um período prolongado.
    
    - Teste de pico: 
        
        Garante a capacidade da API de lidar com picos repentinos na carga de trabalho.
    
    - Teste de tempo de resposta: 
    
        Mede o tempo de resposta de uma API às solicitações e verifica se ela atende às metas de desempenho esperadas.
    
- Testes de segurança:
    
    Segurança API os testes ajudam a verificar se sua API pode proteger dados e sistemas confidenciais contra acesso não autorizado. Os testes de segurança da API incluem a avaliação dos mecanismos de autenticação e autorização da API e testes de vulnerabilidades.

Os testes de API para segurança também podem incluir:

- Teste de autenticidade: 

    Testa os mecanismos de autenticação da API para garantir que sejam seguros e impedir acesso não autorizado. Por exemplo, proteção contra hackers que tentam se passar por outro usuário para obter acesso aos seus dados confidenciais.

- Teste de autorização: 

    Testa os mecanismos de autorização da API para garantir que estejam funcionando conforme esperado e impedir o acesso não autorizado a recursos protegidos. Isso significa que cada usuário deve acessar apenas os dados de sua propriedade (segurança granular em nível de linha).

- Teste de penetração: 

    Simula um ataque cibernético para identificar vulnerabilidades da API que um invasor em potencial poderia explorar. Esse teste é feito usando algoritmos especializados que procuram injeções de código e interrompem essas solicitações antes que possam causar qualquer dano ao servidor.

Ferramentas:
- [Postman](https://www.postman.com/)
- [JMeter](https://jmeter.apache.org/)
- [K6](https://k6.io/)
- [Locust](https://locust.io/)
