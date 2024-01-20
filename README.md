# JS-DIO_Potencia_TechI_IFood-Calculadora_Partidas_Rankeadas

// Definição da classe Heroi
class Heroi {
    // Construtor da classe com as propriedades nome, idade e tipo
    constructor(nome, idade, tipo) {
      this.nome = nome;
      this.idade = idade;
      this.tipo = tipo;
    }
  
    // Método de ataque que exibe a mensagem apropriada conforme o tipo do herói
    atacar() {
      let ataque = "";
  
      // Determinar o tipo de ataque com base no tipo do herói
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
  
      // Exibir a mensagem de ataque
      console.log(`O ${this.tipo} ${this.nome}` `atacou usando ${ataque}`);
    }
  }
  
  // Exemplo de uso da classe Heroi
  const meuHeroi = new Heroi("Aragorn", 30, "guerreiro");
  meuHeroi.atacar(); // Exemplo de saída: O guerreiro Aragorn atacou usando espada
