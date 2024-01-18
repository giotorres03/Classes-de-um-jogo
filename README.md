Classes de um jogo

class Heroi {
  constructor(nome, idade, tipo) {
    this.nome = nome;
    this.idade = idade;
    this.tipo = tipo;
  }

  atacar() {
    let ataque;
    switch (this.tipo) {
      case 'mago':
        ataque = ' magia';
        break;
      case 'guerreiro':
        ataque = ' espada';
        break;
      case 'monge':
        ataque = ' artes marciais';
        break;
      case 'ninja':
        ataque = ' shuriken';
        break;
      default:
        ataque = ' um ataque desconhecido';
    }
    console.log(`O ${this.tipo} atacou usando ${ataque}`);
  }
}

// Exemplo de uso
const heroi1 = new Heroi('Gandalf', 1000, 'mago');
heroi1.atacar(); // O mago atacou usando usou magia
