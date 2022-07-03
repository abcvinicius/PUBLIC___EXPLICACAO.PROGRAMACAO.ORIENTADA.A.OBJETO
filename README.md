# **_Programação orientada a objetos_**




***



## _Como Criar um Objeto?_
 
 * Criar uma Classe(Entidade)

 * Definir seus atributos {Todo Objeto possui um 'Atributo'}
 
 * Definir sua operação(ação/comportamento -> Metodos()) {Todo Objeto possui uma ação}  
 
 > ObsDeCriação: 
 
 >Objeto(Classe/Entidade) começa com letra Maiúscula 
 
 >Atributos letras minúsculas, sem espaço, quando for dar um espaço colocar uma letra em maiúsculo para separar as letras e conseguir ler. _Ex. "dataNascimento"_.

 _`Ex. ou Exemplo:`_

![Classe Aluno](https://user-images.githubusercontent.com/101998147/176944110-e7788b5b-5a4e-4270-a174-b5b59259f731.png)
> Aluno(Classe) >Tem Atributos(ra, nome, dataNascimento) >Tem Operação/Metodo (realizarAvaliacao())




***



# Associação e herança

## _O que é Herança & Associação?_

_**Herança:**_
 * É a permissão que classes tem de compartilhar atributos e métodos, através de "heranças".
 
_**Associação:**_
 * Associação define um relacionamento entre duas classes que permite que um objeto faça com que outro objeto 
   realize uma ação em seu lugar.
  
_**Como Saber se o Relacionamento é uma Herança ou Associação?**_
 
 * _**TEM Um**_ -> Associação('nome do Objeto').
 > Ex. ->  Aluno 'TEM Uma' Turma, Turma 'TEM Varios' Aluno...

> 1°Ex. -> Teoria(usando a class de Aluno para Turma) -> Dentro da Class de Aluno se cria uma 'Variavel(objeto da class de Turma)  
> 1.1Ex. -> Class Turma Cria um Objeto dentro da class de Aluno.  
> 1.2°Ex. -> Objeto da Class turma esta em Aluno. Até porque todo Aluno TEM que ter uma Turma, por isso Cria um ObjetoTurma dentro de Aluno.

`Ex. Codigo -> Turma turma;`   Turma -> Class Turma / turma -> Objeto ou turma.

> 2°Ex. -> Teoria(Usando a class de Turma para Aluno) -> Dentro da Class de Turma se cria um _ArryList_ de Alunos
> 2.1Ex. -> Toda turma tem Varios aluno ent se cria um 'Lista + Nome do Objeto' da ClassAluno dentro da Class de Turma

`Ex. Codigo -> ArryList<Aluno> alunos;` ArryList<Aluno> -> Class Aluno / alunos -> Objeto.


 * _**É um**_ -> Herança(extends). 
 > Ex. -> Aluno 'É UMA' Pessoa, Professor 'É UMA' Pessoa...
 > Ex. Teoria -> "Classe Aluno herda de Pessoa"
 
 `Ex. Codigo -> public class Aluno 'extends' Pessoa`

 ---
 
# Graus de Relacionamentos?

 * Conhecido também por Cardinalidade, o Grau de Relacionamento é o 'relacionamento' entre duas Entidades/Tabelas, 
   onde ele define o "Grau do Relacionamento" entre as Entidades.

## _Os Três Graus de Relacionamento:_
 
* Relacionamento de Um para Um (1 x 1)

![Relacionamento 1 X 1](https://consultabd.files.wordpress.com/2019/09/img01_1x1.jpg)


* Relacionamento de Um para Muitos ou Muitos para Um (1 x N)

![Relacionamento 1 X N](https://user-images.githubusercontent.com/101998147/176983219-c9f34699-dc1c-4773-9664-4aaa2cf218d6.png)


* Relacionamento de Muitos para Muitos (N x N)

![Relacionamento N x N](https://consultabd.files.wordpress.com/2019/09/img01_nxn.jpg?w=616)

## _Tipos de Cardinalidades:_
 
* Cardinalidade Máxima: Número máximo de vezes que uma entidade A pode ocorrer em B. Pode assumir o valor de 1 ou N 
  (inúmeras vezes).

* Cardinalidade Mínima: Número mínimo de vezes que uma entidade A pode ocorrer em B. Pode assumir o valor de 0 ou 1
