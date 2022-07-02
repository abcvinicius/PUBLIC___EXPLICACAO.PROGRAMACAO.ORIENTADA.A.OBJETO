# **_Programação orientada a objetos_**

## _Oque é?_
 
 * Uma Aproximação entre o mundo real e o mundo virtual, através da criação e interação entre 
   objetos, atributos, códigos, métodos, entre outros. Na pratica é nada mais que uma Entidade.

***

## _Como Criar um Objeto?_
 
 * Criar uma Classe(Entidade)

 * Definir seus atributos {Todo Objeto possui um 'Atributo'}
 
 * Definir sua operação(ação/comportamento -> Metodos()) {Todo Objeto possui uma ação}  
 
 > ObsDeCriação: 
 
 >Objeto(Classe/Entidade) começa com letra Maiúscula 
 
 >Atributos letras minúsculas, sem espaço, quando for dar um espaço colocar uma letra em maiúsculo para separar as letras e conseguir ler. _Ex. "dataNascimento"_.

 _`Exemplo:`_

![Classe Aluno](https://user-images.githubusercontent.com/101998147/176944110-e7788b5b-5a4e-4270-a174-b5b59259f731.png)
> Aluno(Classe) >Tem Atributos(ra, nome, dataNascimento) >Tem Operação/Metodo (realizarAvaliacao())




***



# Associação e herança

## _O que é Herança & Associação?_

_**Herança:**_
 * É a permissão que classes tem de compartilhar atributos e métodos, através de "heranças".
 * 
_**Associação:**_
 * Associação define um relacionamento entre duas classes que permite que um objeto faça com que outro objeto 
   realize uma ação em seu lugar.
  
_**Como Saber se o Relacionamento é uma Herança ou Associação?**_
 
 * Tem Um -> Associação().
 > Ex. Professor 'TEM UM' Aluno, Aluno 'TEM UMA' Turma...
`CodigoEx. `

 * É um -> Herança(extends). 
 > Ex. Aluno 'É UMA' Pessoa, Professor 'É UMA' Pessoa...
 
 > ExTeoria -> "Classe Aluno herda de Pessoa"
 
 `ExCodigo -> public class Aluno 'extends' Pessoa`

## Grau de Relacionamento?

 * Conhecido também por Cardinalidade, o Grau de Relacionamento é o 'relacionamento' entre duas Entidades/Tabelas, 
   onde ele define o "Grau do Relacionamento" entre as Entidades.

### _Os Três Graus de Relacionamento:_
 
* Relacionamento de Um para Um (1 x 1)

![Relacionamento 1 X 1](https://consultabd.files.wordpress.com/2019/09/img01_1x1.jpg)


* Relacionamento de Um para Muitos ou Muitos para Um (1 x N)

![Relacionamento 1 X N](https://user-images.githubusercontent.com/101998147/176983219-c9f34699-dc1c-4773-9664-4aaa2cf218d6.png)


* Relacionamento de Muitos para Muitos (N x N)

![Relacionamento N x N](https://consultabd.files.wordpress.com/2019/09/img01_nxn.jpg?w=616)

### _Tipos de Cardinalidades:_
 
* Cardinalidade Máxima: Número máximo de vezes que uma entidade A pode ocorrer em B. Pode assumir o valor de 1 ou N 
  (inúmeras vezes).

* Cardinalidade Mínima: Número mínimo de vezes que uma entidade A pode ocorrer em B. Pode assumir o valor de 0 ou 1
