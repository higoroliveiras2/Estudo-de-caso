# Estudo-de-caso
Jogos
soma = 0
jogos = []
participantes = []
qtd_jogos = int(input('quantos jogos terão no campeonato? '))
for i in range(qtd_jogos):
    nomeJogo = input(f"Digite o nome do {i+1}º jogo: ")

    jogos.append(nomeJogo)
    qtd_participantes = int(input(f"Quantos jogadores se inscreveram no jogo {nomeJogo}? "))
    participantes.append(qtd_participantes)
print("\n Programação de Jogos ")

for jogo in jogos:
   print(f"Jogo inscrito: {jogo}")
   

for i in range(qtd_jogos):
    print('🎮' * participantes[i])
    print(f"{jogos[i]}: {participantes[i]} jogadores inscritos")

for participante in participantes:
    soma= participante + soma
    print('total de participantes:', soma)
