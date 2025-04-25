tags ; #coding #cpp

defs : [[Expressions]]

link : [ref](https://en.cppreference.com/w/cpp/language/template_parameters)

Pour le moment je ne bite rien 

OK ! J'ai capte ! :D 

en gros, un template c'est un truc que t'utilise pour generer du code sur d'autres trucs !
Comme un template sur wix ou keynote: 
	Tu veux faire un site ou un powerpoint. tu utilise une template et tu met tes trucs dedans 
pareille avec une template :D 

et genre le truc "typename" ou "struct" c'est le "placeholder", ce qui vas prendre la place du [[type]] que tu vas utiliser ! :D

genre :
```
template<typename T> //opla un template avec comme placeholder T

T max(T a_value, T b_value){
	if (a_value > b_value)
		return a_value;
	return b_value;
}

int main(){
	int a = 5. b = 4;
	int bigger = max(a, b);// ici Tvas prendre le type "int". Je peux faire parreil avec un char ou un long. En faite tout ce qui a deja definis "operateur<" en soit ! sinon ca sortiras une erreur... dugh
}

```

A VERIFIER

```
struct A // ici je pense que c'est une definition des condition que doit avoire la choses que l'on vas utiliser. C'est avec un typer constant ^^
{
    friend bool operator==(const A&, const A&) = default;
};
 
template<A a>//ici je supose que on dit que ca doit etre la classe "A" et l'elemment a qui doit etre un equivalent de tres loin de "this" ?
void f()
{
    &a;                       // OK
    const A& ra = a, &rb = a; // Both bound to the same template parameter object
    [assert](http://en.cppreference.com/w/cpp/error/assert)(&ra == &rb);       // passes <== logic
}
```


Tu peux avoir different parametre dans tesd templates , soit ils sont constant parametree comme juste au dessu. Soit c'est des type parametre (template \<class T>). soit des template eux meme mais laca deviens complique T^T y'as des petites precisioins sur la resolution des conflit dans les noms en bas de la page de referencde aussi, ca c'est cool.

on peu preciser un type pars defaut aussi :D Tu rajoute "= (ex : int)" devant ton "typename" vuala 