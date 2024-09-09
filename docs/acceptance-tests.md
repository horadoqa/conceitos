# Testes de Aceitação (Acceptance Tests):

Na ponta da pirâmide, temos os testes de aceitação, também conhecidos como testes funcionais ou de aceitação do usuário. Esses testes validam o comportamento do sistema como um todo, muitas vezes simulando a interação do usuário com a aplicação. Eles se concentram em casos de uso e fluxos de trabalho completos e são executados em um nível mais alto de abstração. Os testes de aceitação ajudam a garantir que o software atenda aos requisitos e expectativas dos usuários finais.

Os testes de ponta a ponta (E2E) têm como principal objetivo simular o comportamento de um usuário final em nossa aplicação.

No entanto, assim como os testes de integração, os testes E2E são mais complexos e consomem mais tempo para execução. Portanto, é importante fazer uma seleção criteriosa dos cenários que serão cobertos por esses testes, priorizando os casos mais relevantes e estratégicos dentro do produto.

Já para os testes E2E, que ocupam o topo da pirâmide, é necessário uma seleção cuidadosa e limitada, devido ao seu alto custo de implementação e execução, embora proporcionem uma validação mais completa dos fluxos dentro do aplicativo.

Às vezes há uma confusão entre testes de integração e testes funcionais, uma vez que ambos exigem vários componentes para interagirem entre si. A diferença é que um teste de integração pode simplesmente verificar que você pode consultar o banco de dados, enquanto um teste funcional esperaria obter um valor específico do banco de dados conforme definido pelos requisitos do produto.

Podem ser realizados de duas formas:

- Manuais

O teste manual é um tipo de teste de software que é realizado por um profissional sem a assistência de todas as ferramentas automatizadas, através de casos de testes ou documentações de requisitos e negócios, que possui o passo a passo com as funcionalidades do sistema para obter o resultado esperado.

- Automatizados

Os testes automatizados são realizados utilizando algumas opções de linguagens de programação, frameworks e bibliotecas, dependendo do tipo e condições de testes a serem realizados, para a construção de scripts de testes.

Benefícios da automação em seu projeto:

- Economia de tempo x custo;
- Redução de erros;
- 70% mais ágil do que os testes manuais;
- Reaproveitamento de testículos;
- Aumento da produtividade;
- Aumento da qualidade.

Ferramentas:
- Selenium
- Cypress
- Robot Framework
- Cucumber