
> What precisely do we mean by software engineering? What distinguishes “software engineering” from “programming” or “computer science”? And why would Google have a unique perspective to add to the corpus of previous software engineering literature written over the past 50 years?
 
> The terms “programming” and “software engineering” have been used interchangeably for quite some time in our industry, although each term has a different emphasis and different implications. University students tend to study computer science and get jobs writing code as “programmers.”

> “Software engineering,” however, sounds more serious, as if it implies the application of some theoretical knowledge to build something real and precise. Mechanical engineers, civil engineers, aeronautical engineers, and those in other engineering disciplines all practice engineering. They all work in the real world and use the application of their theoretical knowledge to create something real. Software engineers also create “something real,” though it is less tangible than the things other engineers create.
 
> Unlike those more established engineering professions, current software engineering theory or practice is not nearly as rigorous. Aeronautical engineers must follow rigid guidelines and practices, because errors in their calculations can cause real damage; programming, on the whole, has traditionally not followed such rigorous practices. But, as software becomes more integrated into our lives, we must adopt and rely on more rigorous engineering methods. We hope this book helps others see a path toward more reliable software practices.


A engenharia, segundo o conhecimento popular, é conhecida pela construção de algo concreto, como um objeto palpável. Podemos observar isso em prédios ou carros, que envolvem respectivamente a Engenharia Civil e a Engenharia Mecânica.

Já a Engenharia de Software desenvolve aplicações que se aproximam mais do intangível. Essa característica faz com que seja aparentemente mais simples de desenvolver, exigindo menos recursos como tempo, dinheiro e conhecimento. No entanto, mantém a essência da engenharia: o planejamento, desenvolvimento e manutenção.

> # Programming Over Time
> We propose that “software engineering” encompasses not just the act of writing code, but all of the tools and processes an organization uses to build and maintain that code over time. What practices can a software organization introduce that will best keep its code valuable over the long term? How can engineers make a codebase more sustainable and the software engineering discipline itself more rigorous? We don’t have fundamental answers to these questions, but we hope that Google’s collective experience over the past two decades illuminates possible paths toward finding those answers.
 
> One key insight we share in this book is that software engineering can be thought of as “programming integrated over time.” What practices can we introduce to our code to make it sustainable—able to react to necessary change—over its life cycle, from conception to introduction to maintenance to deprecation?
 
> The book emphasizes three fundamental principles that we feel software organizations should keep in mind when designing, architecting, and writing their code:
 
> ### Time and Change
> How code will need to adapt over the length of its life
 
> ### Scale and Growth
> How an organization will need to adapt as it evolves
 
> ### Trade-offs and Costs
> How an organization makes decisions, based on the lessons of Time and Change and Scale and Growth

A engenharia de software está além da simples escrita de código, abrangendo todas as ferramentas e processos usados por uma organização para criar e manter o código ao longo do tempo. Ele sugere que as práticas que a organização adote devem assegurar que o código se mantenha lapidado ao longo do ciclo de vida do software, indo da concepção até a descontinuação. A ideia central é que a engenharia de software é como uma "programação integrada ao longo do tempo", com o objetivo de criar um código sustentável, capaz de se adaptar às mudanças necessárias.

Existem três princípios fundamentais para a criação de código sustentável: 
* O tempo e a mudança, que aborda como o código precisa evoluir durante sua vida útil; 
* A escala e o crescimento, que reflete como a organização deve se adaptar à medida que cresce; 
* E os trade-offs e custos, que enfatizam a importância de tomar decisões informadas, equilibrando as lições dos dois primeiros princípios. 

Esses princípios visam tornar a engenharia de software mais rigorosa e eficiente, garantindo que o código e a organização possam se ajustar e prosperar ao longo do tempo.

> # Exemplos de Trade-offs

#### 1. Portabilidade X Acessibilidade
O Java é uma linguagem altamente portátil, capaz de ser executada em múltiplos sistemas, enquanto o Python é uma linguagem acessível, com uma curva de aprendizado suave e ampla usabilidade para diferentes usuários.

#### 2. Usabilidade X Segurança
O Windows é conhecido por suas interface gráfica e recursos que facilitam a vida de usuários, principalmente iniciantes. Em contrapartida o Linux é conhecido por sua segurança, controle e maior personalização de suas configurações, o que torna seu sistema livre de ataques e vulnerabilidades.
#### 3. Simplicidade X Escalabilidade
Suponha que você está criando um aplicativo de tarefas para gerenciar a lista de afazeres de um usuário. Para simplificar, você decide armazenar todas as tarefas de todos os usuários em um único arquivo de texto. Isso torna o código muito **simples e fácil** de implementar.

À medida que o número de usuários cresce esse arquivo de texto se torna maior e mais difícil de gerenciar. A busca por uma tarefa específica ou o carregamento de todas as tarefas pode ficar muito lento. Para **escalabilidade**, você precisaria migrar para um banco de dados, o que daria uma complexidade ao sistema. Trocando o simples por algo que possa se expandir e permitir melhorias no futuro.

> ### [Engenharia de Software - MVP](https://docs.google.com/presentation/d/1GMds68vXowb3h_GFtI3fwKeXJQQJjm7L-wL0BJhIfLI/edit#slide=id.g1100bb71266_1_7)
> ![image](https://github.com/user-attachments/assets/a89365ab-8947-4177-b04a-21e0c887b0f6)

Na imagem acima é demonstrado o beneficio de, ao longo de uma entrega de um produto, realizar entregas com valor ao invés de partes não funcionais do todo. Como no exemplo, se alguém precisa de um carro, é melhor oferecer aos poucos outros meios para transporte mais simples como um skate, uma bicicleta, uma moto e então um carro, ao invés de entregar as rodas ou um chassi, onde o cleinte não conseguirá utilizar.

