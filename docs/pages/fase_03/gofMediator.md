# GoF Mediator

 ## Versionamento

 | Versão |    Data    |     Modificação      | Autor | Revisor |
 | ------ | :--------: | :------------------: | :---: | :-----: |
 | 1.0    | 07/03/2022 | Criação do Documento |  Guilherme Fernandes     |         |

 <!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

 ## Introdução
 Os padrões de projeto descrevem uma solução geral para um problema que acontece recorrentemente dentro de um projeto de software. Este documento tem como objetivo explicar sobre o padrão GoF comportamental Mediator e suas aplicações. 

 ## Metodologia
 O Mediator é um GoF comportamental que permite que haja uma redução das dependências caóticas entre classes. Ele consiste na restrição de comunicação direta entre objetos e exige que eles interajam entre si apenas por meio de um objeto mediador. Abaixo, um exemplo de Mediator em C#:
 ```
  public interface IMediator
    {
        void Notify(object sender, string ev);
    }

    // Concrete Mediators implement cooperative behavior by coordinating several
    // components.
    class ConcreteMediator : IMediator
    {
        private Component1 _component1;

        private Component2 _component2;

        public ConcreteMediator(Component1 component1, Component2 component2)
        {
            this._component1 = component1;
            this._component1.SetMediator(this);
            this._component2 = component2;
            this._component2.SetMediator(this);
        } 

        public void Notify(object sender, string ev)
        {
            if (ev == "A")
            {
                Console.WriteLine("Mediator reacts on A and triggers folowing operations:");
                this._component2.DoC();
            }
            if (ev == "D")
            {
                Console.WriteLine("Mediator reacts on D and triggers following operations:");
                this._component1.DoB();
                this._component2.DoC();
            }
        }
    }

    // The Base Component provides the basic functionality of storing a
    // mediator's instance inside component objects.
    class BaseComponent
    {
        protected IMediator _mediator;

        public BaseComponent(IMediator mediator = null)
        {
            this._mediator = mediator;
        }

        public void SetMediator(IMediator mediator)
        {
            this._mediator = mediator;
        }
    }

    // Concrete Components implement various functionality. They don't depend on
    // other components. They also don't depend on any concrete mediator
    // classes.
    class Component1 : BaseComponent
    {
        public void DoA()
        {
            Console.WriteLine("Component 1 does A.");

            this._mediator.Notify(this, "A");
        }

        public void DoB()
        {
            Console.WriteLine("Component 1 does B.");

            this._mediator.Notify(this, "B");
        }
    }

    class Component2 : BaseComponent
    {
        public void DoC()
        {
            Console.WriteLine("Component 2 does C.");

            this._mediator.Notify(this, "C");
        }

        public void DoD()
        {
            Console.WriteLine("Component 2 does D.");

            this._mediator.Notify(this, "D");
        }
    }
    
    class Program
    {
        static void Main(string[] args)
        {
            // The client code.
            Component1 component1 = new Component1();
            Component2 component2 = new Component2();
            new ConcreteMediator(component1, component2);

            Console.WriteLine("Client triggets operation A.");
            component1.DoA();

            Console.WriteLine();

            Console.WriteLine("Client triggers operation D.");
            component2.DoD();
        }
    }
 ```
 ## Aplicabilidade

 É possível utilizar o GoF comportamental Mediator é aplicado em diversos contextos, sendo principalmente utilizado em soluções onde é necessário que classes se comuniquem sem que seja necessário um alto acoplamento entre elas. Por utilizar uma interface como mediador, é interessante para implementações que utilizam classes que contém as mesmas funções, mas com implementação diferente. Um exemplo é classes que realizam autenticação de serviços, pois é possível definir um protocolo chamado Autenticação e passar para o mediador qual serviço será utilizado (ex: Firebase, Facebook, Google Sign In, etc). Dessa forma, é possível reduzir o acoplamento entre classes, aumentar a testabilidade e a manutenibilidade da solução, além de permitir que o código seja reutilizado em outras partes da aplicação. 

 ## Vantagens e desvantagens

 | Vantagens | Desvantagens |
 | :-------: | :----------: |
 | Respeita o princípio da responsabilidade única. | Pode evoluir para um Objeto Deus com o tempo. 
 | Respeita o princípio aberto/fechado |
 | Reduz o acoplamento entre os componentes do programa. |  |
 | Permite a reutilização de código mais facilmente. |  |

 ## Conclusão

O padrão Mediator é amplamente utilizado por reduzir o acoplamento entre classes. Dessa forma, seu uso é extremamente interessante para que haja um aumento da qualidade da aplicação. Todavia, esse padrão deve ser arquitetado cautelosamente na solução para que não haja a criação de um Objeto Deus. Além disso, é um padrão recomendado em soluções que apresentem classes com comportamentos parecidos, mas que fazem implementações distintas. Sendo assim, no contexto do nosso projeto, não há aplicações aparentes para a utilização do Mediator pois ele adiciona uma camada de abstração desnecessária no escopo do projeto, visto que é um projeto menos robusto e complexo. 

 ## Bibliografia

 - Mediator. Disponível em: <https://refactoring.guru/pt-br/design-patterns/mediator>. (último acesso em 07/03/2022)
 - Mediator em C#. Disponível em: <https://refactoring.guru/pt-br/design-patterns/mediator/csharp/example>. (último acesso em 07/03/2022)

