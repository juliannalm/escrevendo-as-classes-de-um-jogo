# escrevendo-as-classes-de-um-jogo
// Definição da classe Heroi
class Heroi {
  // Construtor da classe
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo;
  }

  // Método para atacar
  atacar() {
    let ataque;

    // Definindo o ataque com base no tipo do herói
    switch (this.tipo) {
      case "mago":
        ataque = "usou magia";
        break;
      case "guerreiro":
        ataque = "usou espada";
        break;
      case "monge":
        ataque = "usou artes marciais";
        break;
      case "ninja":
        ataque = "usou shuriken";
        break;
      default:
        ataque = "usou um ataque indefinido";
    }

    // Exibindo a mensagem
    console.log(`O ${this.tipo} atacou usando ${ataque}`);
  }
}

// Exemplo de uso das classes
const heroi1 = new Heroi("Aragorn", 35, "guerreiro");
heroi1.atacar(); // Saída esperada: "O guerreiro atacou usando espada"

const heroi2 = new Heroi("Gandalf", 200, "mago");
heroi2.atacar(); // Saída esperada: "O mago atacou usando magia"
