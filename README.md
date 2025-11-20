# atividade_3_python - Dupla: Mateus e Yasmim

README – Sistema de RPG (Questões 1 a 30)

Projeto desenvolvido em Python
Paradigma de Linguagem de Programação – ARA0066

📘 Descrição Geral

Este projeto implementa um sistema completo de RPG em Python, seguindo rigorosamente todas as instruções das Questões 1 a 30 da atividade.
Ele inclui:

Classes de personagens (Guerreiro, Mago, Arqueiro)

Classe base Personagem (herança e encapsulamento)

Monstros, Goblin padrão e Orc

Sistema de ataque e dano

Sistema de itens (Armas e Poções)

Inventário

Habilidades (com classe abstrata)

Dado (aleatoriedade)

Sistema de batalha com turnos e vencedor

Combates individuais e em equipe

O código principal não executa nada automaticamente — ele apenas define as classes e funções necessárias para o funcionamento do RPG.
Para interagir com o sistema, utilize os testes abaixo.

🧪 Testes recomendados no Google Colab

Coloque o código principal em uma única célula.
Depois, use os testes abaixo em células separadas.

=================================================
📌 Célula 1 — Criar personagens
g = Guerreiro("Arthur", 100, 20)
m = Mago("Merlin", 80, 15, "Fogo")
a = Arqueiro("Robin", 90, 18, 95)

print(g)
print(m)
print(a)

=================================================

📌 Célula 2 — Equipar Armas
equipar_arma(g, espada_longa)
equipar_arma(m, cajado_magico)

=================================================

📌 Célula 3 — Teste de Ataque
g.atacar(m)
m.atacar(g)
a.atacar(g)

=================================================

📌 Célula 4 — Usando Poções
g.inventario.adicionar_item(pocao_vida)
g.inventario.usar_pocao(g, "Poção de Vida")

=================================================

📌 Célula 5 — Criando Monstro (Goblin padrão)
goblin = FabricaDeMonstros.goblin_padrao()
print(goblin)
g.atacar(goblin)
print("Goblin está vivo?", goblin.esta_vivo())

=================================================

📌 Célula 6 — Testando Habilidades
golpe_forte = AtaqueForte()
bola_fogo = AtaqueBolaFogo()

g.aprender_habilidade(golpe_forte)
m.aprender_habilidade(bola_fogo)

g.usar_habilidade(golpe_forte, goblin)
m.usar_habilidade(bola_fogo, goblin)

=================================================

📌 Célula 7 — Testando o Sistema de Batalha
batalha = Batalha(g, goblin)
batalha.iniciar()

📚 Resumo do que o sistema implementa
✔ Questões 1 a 3

Guerreiro, Mago e Arqueiro com atributos e métodos principais.

✔ Questão 4
Classe Monstro e Goblin padrão.

✔ Questão 5
Status com __str__().

✔ Questão 6

Ação básica de ataque.
✔ Questões 7 a 9

Armas, poções e equipar arma.

✔ Questão 10
Ataque real soma força + arma.

✔ Questões 11 a 14
Herança → classe base Personagem, proteção da vida, receber dano, ataque real.

✔ Questões 15 e 16
Inventário + integração com personagem.

✔ Questão 17
Usar poções com limite de vida.

✔ Questão 18
Ataques únicos de cada classe.

✔ Questão 19
Fábrica de Goblins.

✔ Questão 20
Método esta_vivo().

✔ Questões 21 a 23
Habilidades com classe abstrata, uso de habilidades e lista de habilidades.

✔ Questões 24 e 25
Classe Dado e dano aleatório.

✔ Questão 26
Orc com golpe crítico.

✔ Questões 27 a 29
Sistema de batalha com turnos e vencedor.

✔ Questão 30
Batalha entre equipes.

📄 Observações importantes

O código não imprime nada sozinho, isso é o funcionamento normal.
Para testar, use as células de teste acima.
Todas as classes funcionam juntas para criar um sistema de RPG completo.
