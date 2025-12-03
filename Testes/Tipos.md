# Tipos de testes

Se você já trabalhou em algum projeto desenvolvendo código, já deve ter separado com uma parede de erros interrompendo a execução do seu programa, agora imagine a interrupção dessa execução em prod (runtime).

**Porque erros acontecem?**

- Seres humanos desenvolvem o código e como seres humanos temos tendencia a falhar ou cometer erros;
- E como os testes nos ajudam com isso?
- Os testes não são parfeitos, mas são uma camada de proteção a mais

**Pirâmide de Testes**

**E2E** - O teste da aplicação de ponta a ponta;
**INTEGRAÇÃO** - Onde são testadas integrações entre as partes do projeto e algumad dependências externas;
**UNITÁRIOS** - Menores componentes da nossa base de código, que serão testados individualmente.

**Testes Unitários**

- Testes curtos e isolados;
- Análise de funções ou métodos;
- Não garante uma integração de módulos.

**Testes de Integração**

- Testes de rotas e requisições;
- Comunicação dos módulos;
- Não análisa todo o fluxo da aplicação.

**Testes E2E (end to end)**

- Ponta a ponta, alto nível;
- testes longos e completos;
- Análise de todos os módulos e stacks. Ex.: front-end/banco de dados / micro serviços.
- Tempo longo e custo alto;
- Complexa estrutura de testes.
