### 1. INTRODUÇÃO
A ATECH é uma empresa de desenvolvimento de software localizada no bairro Vila Olímpia – São Paulo – SP e possuí uma filial no Parque Tecnológico de São José dos Campos que abrange vários segmentos de mercado, como aeronáutico, defesa e segurança, negócios corporativos, entre outros. Dentro do segmento de negócios corporativos, ela possui a plataforma OKTO, que é um conjunto de soluções para excelência operacional, conexões inteligentes, gestão de ativos e logística que segue o conceito de #IndustryNXT, que une a eficiência da indústria 4.0 aos processos inovadores da digitalização para criar um ciclo contínuo de desenvolvimento que vai desde a produção até a entrega do produto final.
	A plataforma OKTO possuí quatro linhas de segmento: excelência operacional, conexões inteligentes, gestão logística, gestão de ativos. O modulo que vai ser desenvolvido neste trabalho irá fazer parte no segmento de gestão de ativos.
	A ferramenta de gestão de ativos é responsável por conectar o mundo financeiro e o chão de fábrica, auxiliando nas tomadas de decisões em cima de um ativo, como momento de fazer manutenção, revisão etc. Um sistema de gestão de ativos também é responsável por coletar dados, assim conseguindo balancear os três pilares principais para o uso do ativo, que são performance, custo e risco. Performance é possível visualizar a disponibilidade do ativo, a confiabilidade, manutenibilidade e o quanto ele está produzindo. Risco é o quanto um ativo pode impactar financeiramente na empresa, confiabilidade e disponibilidade. Custo é o valor que se gasta para produzir com aquele ativo. Com isso a intenção é de diminuir os custos de manutenção, minimizar defeitos de equipamentos, reduzir paradas não programadas, diagnosticar problemas de forma proativa, saber o custo do inventario, aumentar a disponibilidade e produtividade de um ativo, entre outros.
Hoje no sistema de gestão de ativos da Atech não possui um controle de versionamento quando é gerado uma movimentação, sem o versionamento não existe um mapeamento de como sistema estava antes da movimentação, e para fazer uma movimentação de equipamento, é necessário excluir o ativo e recadastrá-lo em outro local ou planta, gerando um desgaste e esforço grande, para o usuário do sistema.
O trabalho irá auxiliar no problema, permitindo que o usuário mova um ativo para outro local ou planta, sendo validado pelo backend, após permitido o modulo mostrará como estava a estrutura e como ficou para ser confirmado pelo usuário. Outro ponto relevante será o versionamento da estrutura, o usuário poderá fazer um “rollback”, para uma estrutura anterior, caso seja permitido conforme as regras que serão estabelecidas pelo administrador do sistema.
Este trabalho utilizará de levantamentos de requisitos, assim será feita uma entrevista com o cliente para coletar informações, conforme o necessário para o desenvolvimento do mesmo.
#### 1.1. Objetivos do Trabalho 
O objetivo geral deste trabalho é desenvolver um modulo que irá fazer uma solução simplificada para manutenção de estruturas de localização em gestão de ativos no sistema OKTO da ATECH.
#### 1.2. Conteúdo do Trabalho
O presente trabalho está estruturado em seis Capítulos, cujo conteúdo é sucintamente apresentado a seguir:
No Capítulo 2 será apresentado os levantamentos de requisitos e as tecnologias que serão utilizadas na implementação do projeto.
No Capítulo 3 apresenta a arquitetura da aplicação, desenvolvimento da solução.
No Capítulo 4 ....
No Capítulo 5 ....


### 2. FUNDAMENTAÇÃO TÉCNICA
Neste capítulo será visto o levantamento de requisitos e uma previa sobre as tecnologias que vamos utilizar para o desenvolvimento do sistema. 
#### 2.1. Levantamento de Requisitos
Levantamento de requisitos é a técnica de investigar, procurar as necessidades e/ou exigências do sistema. Através de uma entrevista o engenheiro de sistemas, coletas as informações junto ao cliente.
Este módulo disponibilizará uma interface em o usuário irá controlar os seus ativos. Será exibido uma arvore, onde terá os seus “nós” ou “filhos”. Terá como “raiz” No sistema o usuário pode cadastrará um “nó”, o sistema terá um controlar a quantidades de “nós”, pois terá uma quantidade máxima configurada. 
 ![](/img/Imagem1.png)
 ![](/img/Imagem2.png)
 ![](/img/Imagem3.png)
 
#### 2.1.1. Requisitos Funcionais
Os requisitos funcionais definem as funcionalidades que um sistema deve fazer, sempre descritos os comportamentos de entrada e saída. São funcionalidades que o sistema deve fazer.
![](/img/Imagem4.png)
 
#### 2.1.2. Requisitos não funcionais
Os requisitos não funcionais definem os atributos do sistema, como segurança, confiabilidade, desempenho, capacidade de manutenção, escalabilidade e usabilidade. Não dizem respeito diretamente as funções específicas do sistema. São qualidades que o sistema de ter.

#### 2.2. Tecnologias Arquitetura Web
Neste projeto vamos utilizar a Arquitetura Web e será implementada separadamente com as Arquiteturas Backend e Frontend, que irão ser apresentadas no próximo capítulo. Para a implementação desta serão utilizadas algumas tecnologias que veremos a seguir:

### 3. DESENVOLVIMENTO

#### 3.1. Arquitetura do Sistema
Uma aplicação web é um software executado em um servidor disponível na rede (internet). Para acessar uma aplicação web, é necessário o uso de um navegador com conexão à internet.
Dois termos muitos usados na arquitetura web são o back-end e front-end, os quais serão utilizados na implementação deste trabalho.

#### 3.1.1. Front-end
Front-end é a parte visual do sistema que o usuário interage diretamente, vezes chamado “lado do cliente”, para que o usuário tenha uma boa experiência é muito importante ser bem modelado, para que o usuário tenha uma boa experiência. 

#### 3.1.2. Back-end
Back-end é a parte do sistema que o usuário não “vê”, onde fica toda regra de negócio, processamento, domínio, conexão com o banco de dados, segurança etc.

