def atualizatela(linha0,linha1,linha2):
	print(""" a %s | b %s | c %s
---------------------------------""" % (linha0[0],linha0[1],linha0[2]) )
	print(""" d %s | e %s | f %s
--------------------------------- """ % (linha1[0],linha1[1],linha1[2]) )
	print(""" g  %s| h %s | i %s """%(linha2[0], linha2[1], linha2[2]))
	return;
	
print("bem vindo ao jogo da velha")
usuario = input("voce gostaria de jogar com X ou O?\n")
usuario = usuario.upper()
if (usuario == 'X'):
                oponente = 'O'
else:
                oponente = 'X'
print("certo,voce vai jogar com: ",usuario)
print("e o seu oponente vai jogar com:  ",oponente)
print("\n")
linha0 = ['X', 'O', 'O']
linha1 = ['O', 'X', 'O']
linha2=  [' ', 'O', 'X']
atualizatela(linha0,linha1,linha2)
def ganhou():
        for i in('X','O'):
        if ((linha0[0] == linha0[1])and(linha0[2] == i)): return i
        if ((linha1[0] == linha1[1])and(linha1[2] == i)): return i
        if ((linha2[0] == linha2[1])and(linha2[2] == i)): return i
        if ((linha0[0] == linha1[1])and(linha2[2] == i)): return i
        if ((linha1[2] == linha1[1])and(linha2[0] == i)): return i
        if ((linha0[0] == linha1[0])and(linha2[0] == i)): return i
        if ((linha0[1] == linha1[1])and(linha2[1] == i)): return i
        if ((linha0[2] == linha1[2])and(linha2[2] == i)): return i
        print(i)
        print("Ganhou")
        return;
def velha();
        if ((linha0[0] =! linha0[1]) and (linha0[2] =! i)): return i
        if ((linha1[0] =! linha1[1]) and (linha1[2] =! i)): return i
        if ((linha2[0] =! linha2[1]) and (linha2[2] =! i)): return i
        if ((linha0[0] =! linha1[1]) and (linha2[2] =! i)): return i
        print("Deu velha")

