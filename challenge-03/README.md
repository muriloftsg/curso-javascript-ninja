# Desafio da semana #3

```js
// Declarar uma variável qualquer, que receba um objeto vazio.
var oi = {}

/*
Declarar uma variável `pessoa`, que receba suas informações pessoais.
As propriedades e tipos de valores para cada propriedade desse objeto devem ser:
- `nome` - String
- `sobrenome` - String
- `sexo` - String
- `idade` - Number
- `altura` - Number
- `peso` - Number
- `andando` - Boolean - recebe "falso" por padrão
- `caminhouQuantosMetros` - Number - recebe "zero" por padrão
*/
pessoa = { nome: 'Murilo', sobrenome: 'Godoi', sexo: 'Masculino', idade: 17, altura: 1.81, peso: 66, andando: false, caminhouQuantosMetros: 0 }

/*
Adicione um método ao objeto `pessoa` chamado `fazerAniversario`. O método deve
alterar o valor da propriedade `idade` dessa pessoa, somando `1` a cada vez que
for chamado.
*/
pessoa.fazerAniversario = function() {
    pessoa.idade++
}

/*
Adicione um método ao objeto `pessoa` chamado `andar`, que terá as seguintes
características:
- Esse método deve receber por parâmetro um valor que representará a quantidade
de metros caminhados;
- Ele deve alterar o valor da propriedade `caminhouQuantosMetros`, somando ao
valor dessa propriedade a quantidade passada por parâmetro;
- Ele deverá modificar o valor da propriedade `andando` para o valor
booleano que representa "verdadeiro";
*/
pessoa.andar = function(metrosAndados) {
    pessoa.caminhouQuantosMetros += metrosAndados;
    pessoa.andando = true;
}

/*
Adicione um método ao objeto `pessoa` chamado `parar`, que irá modificar o valor
da propriedade `andando` para o valor booleano que representa "falso".
*/
pessoa.parar = function() {
    pessoa.andando = false;
}

/*
Crie um método chamado `nomeCompleto`, que retorne a frase:
- "Olá! Meu nome é [NOME] [SOBRENOME]!"
*/
pessoa.nomeCompleto = function() {
    return 'Ola, meu nome e ' + pessoa.nome + ' ' + pessoa.sobrenome;
}

/*
Crie um método chamado `mostrarIdade`, que retorne a frase:
- "Olá, eu tenho [IDADE] anos!"
*/
pessoa.mostrarIdade = function() {
    return 'Ola eu tenho ' + pessoa.idade + ' anos';
}

/*
Crie um método chamado `mostrarPeso`, que retorne a frase:
- "Eu peso [PESO]Kg."
*/
pessoa.mostrarPeso = function() {
    return 'Eu peso ' + pessoa.peso + 'Kg.';
}

/*
Crie um método chamado `mostrarAltura` que retorne a frase:
- "Minha altura é [ALTURA]m."
*/
pessoa.mostrarAltura = function() {
    return 'Minha altura e ' + pessoa.altura + 'm.';
}

/*
Agora vamos brincar um pouco com o objeto criado:
Qual o nome completo da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.nomeCompleto() // 'Ola, meu nome e Murilo Godoi'

/*
Qual a idade da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.mostrarIdade() // 'Ola eu tenho 18 anos'

/*
Qual o peso da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.mostrarPeso() // 'Eu peso 66Kg.'

/*
Qual a altura da pessoa? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.mostrarAltura() // 'Minha altura e 1.81m.'

/*
Faça a `pessoa` fazer 3 aniversários.
*/
pessoa.fazerAniversario()
pessoa.fazerAniversario()
pessoa.fazerAniversario()

/*
Quantos anos a `pessoa` tem agora? (Use a instrução para responder e
comentários inline ao lado da instrução para mostrar qual foi a resposta
retornada)
*/
pessoa.fazerAniversario() // 21 anos

/*
Agora, faça a `pessoa` caminhar alguns metros, invocando o método `andar` 3x,
com metragens diferentes passadas por parâmetro.
*/
pessoa.andar(12)
pessoa.andar(102)
pessoa.andar(13)

/*
A pessoa ainda está andando? (Use a instrução para responder e comentários
inline ao lado da instrução para mostrar qual foi a resposta retornada)
*/
pessoa.andar() // andando: true;

/*
Se a pessoa ainda está andando, faça-a parar.
*/
pessoa.parar()

/*
E agora: a pessoa ainda está andando? (Use uma instrução para responder e
comentários inline ao lado da instrução para mostrar a resposta retornada)
*/
pessoa.parar() // andando: false

/*
Quantos metros a pessoa andou? (Use uma instrução para responder e comentários
inline ao lado da instrução para mostrar a resposta retornada)
*/
pessoa // caminhouQuantosMetros: 137

/*
Agora vamos deixar a brincadeira um pouco mais divertida! :D
Crie um método para o objeto `pessoa` chamado `apresentacao`. Esse método deve
retornar a string:
- "Olá, eu sou o [NOME COMPLETO], tenho [IDADE] anos, [ALTURA], meu peso é [PESO] e, só hoje, eu já caminhei [CAMINHOU QUANTOS METROS] metros!"

Só que, antes de retornar a string, você vai fazer algumas validações:
- Se o `sexo` de `pessoa` for "Feminino", a frase acima, no início da
apresentação, onde diz "eu sou o", deve mostrar "a" no lugar do "o";
- Se a idade for `1`, a frase acima, na parte que fala da idade, vai mostrar a
palavra "ano" ao invés de "anos", pois é singular;
- Se a quantidade de metros caminhados for igual a `1`, então a palavra que
deve conter no retorno da frase acima é "metro" no lugar de "metros".
- Para cada validação, você irá declarar uma variável localmente (dentro do
método), que será concatenada com a frase de retorno, mostrando a resposta
correta, de acordo com os dados inseridos no objeto.
*/
?

// Agora, apresente-se ;)
var oi = {}

var pessoa = {nome: 'Murilo', sobrenome: 'Godoi', sexo:'Masculino', idade: 17, altura: 1.81, peso: 66, andando: false, caminhouQuantosMetros: 0}

pessoa.fazerAniversario = function() {
    pessoa.idade++;
}

pessoa.andar = function(caminhou) {
    pessoa.caminhouQuantosMetros += caminhou
    andando = true;
}

pessoa.parar = function() {
    pessoa.andando = false;
}

pessoa.nomeCompleto = function() {
    return 'Ola, meu nome e ' + pessoa.nome + ' ' + pessoa.sobrenome;
}

pessoa.mostrarIdade = function() {
    return 'Ola eu tenho ' + pessoa.idade + ' anos';
}

pessoa.mostrarPeso = function() {
    return 'Eu peso ' + pessoa.peso + 'Kg.';
}

pessoa.mostrarAltura = function() {
    return 'Minha altura e ' + pessoa.altura + 'm.';
}

pessoa.apresentacao = function() {
    var sexo;
    if (sexo === 'Feminino') {
        sexo = 'a'
    } else {
        sexo = 'o'
    }
    var idade;
    if (idade === 1) {
        idade = 'ano'
    } else {
        idade = 'anos'
    }
    var metragem;
    if (metragem === 1) {
        metragem = 'metro'
    } else {
        metragem = 'metros'
    }
    return 'Ola eu sou ' + sexo + ' ' + pessoa.nome + ' ' + pessoa.sobrenome + ', tenho ' + pessoa.idade + ' ' + idade + ', ' + pessoa.altura + ', meu peso e ' + pessoa.peso + ' e, so hoje eu ja caminhiei ' + pessoa.caminhouQuantosMetros + ' ' + metragem;
}
