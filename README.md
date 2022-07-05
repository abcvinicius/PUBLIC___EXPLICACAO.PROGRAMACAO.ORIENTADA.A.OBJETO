# **_Programação orientada a objetos_**

## _O que é?_
 
 * Uma Aproximação entre o mundo real e o mundo virtual, através da criação e interação entre 
   objetos, atributos, códigos, métodos, entre outros. Na pratica é nada mais que a funcionalidade de uma Entidades.
   
  > Exemplo. Teoria -> Entidade Disciplina tem Matematica, Portugues...
  
  > (As Materias cadastradas que são os Objetos das Entidades, dão um funcionalidade para as entidades).



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



# _Associação e herança_

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
 
# _Graus de Relacionamentos?_

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



---



# _Criação de Objetos e Encapsulamento_
 
## _Objeto_

 _**O que é um Objeto?**_
 
* O Objeto é basicamente a Função que uma Class recebe. Um exemplo claro de Objeto seria em uma __ClassDisciplina__ tem 2 Obejtos (matematica e português) essas disciplinas(referindo à Matematica e Português) que são a função da __ClassDisciplina__, então, elas que são os Objetos, elas que dão uma "Função" para a Class.

 
 
 ## _Encapsulamento_

 _**O que é um Encapsulamento?**_

 * Posso descrever o Encapsulamento como privrar, proteger e incluir algo dentro de uma "Capsula". Ele defiine o Tipo do Atributo, no caso refere-se á um atributo Private, Protect, Public e Pakcage. Além disso o Encapsulamento está envolvido como Metodos Getters e Setters.
 
 _**Tipos de Encapsulamento?**_
 
 * _**Para entender mais sobre o Encapsulamento a gente deve compreender seus Tipos. São Eles:**_
 
 _**1° `Public`**_
 * Todas as Classes conseguem acessa-lo, não importa se está fora ou dentro da mesma pasta.
 
 _**2° `Private`**_
 * Somente a propria Class pode acessar.
 
 _**3° `Protected`**_
 * Somente a propria Class e SubClass acessa diretamente.
 
 _**4° `Package`**_
 * Pode ser acessado pelas Class de dentro do mesmo Pack(Pacote).

 _**Metodos Getters & Setters**_
 * Esses Metodos servem para que você tenha acesso aos Dados Private de uma Class mas, de forma que não seja direta(Sem Segurança).
 
 _Metodo Get_
 * Ele está relacionado a puxar/pegar algum valor.
 
 _Metodo Set_
 * Ele está relacionado a Modificar/Setar algum valor.
 
 > OBS: Toda vez que você Settar algo você deve saber que la dentro de Getters e Setter que você criou vai chegar a requisição do Objeto que você
   criou/Setou, então os atributos vão passar enviando eles mesmo e guardando eles no atributo nome "This". 
 
 _**O que é This?**_
 * Ele é uma referencia do Objeto a ele mesmo. Ele vai salvar a requisição nele mesmo.
 * Quando a gente se referir a This, ele está dizendo que ele é **Referido AO Objeto**.
