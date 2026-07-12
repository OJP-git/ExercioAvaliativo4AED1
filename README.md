# ExercioAvaliativo4AED1
## Nome: João Pedro da Silva Netto
## LeetCode 18: 4sum
### [https://leetcode.com/problems/global-and-local-inversions/](https://leetcode.com/problems/4sum/)
Esse leetcode fornecia um vetor de inteiros e um valor alvo. Deveriamos verificar quais conjuntos de 4 numeros do vetor, somados, resultavam no valor alvo, não podendo repetir e a ordem não importava dentro da matriz de resposta.

### Casos testados:
####Teste 1: exemplo 1 do enunciado
	int		t1[] = { 1, 0, -1, 0, -2, 2 };
	int		e1[][4] = { { -2, -1, 1, 2 }, { -2, 0, 0, 2 }, { -1, 0, 0, 1 } };
####Teste 2: exemplo 2 do enunciado - duplicatas extremas 
	int		t2[] = { 2, 2, 2, 2, 2 };
	int		e2[][4] = { { 2, 2, 2, 2 } };
####Teste 3: menos de 4 elementos - resposta vazia
	int		t3[] = { 1, 2, 3 };
####Teste 4: overflow - 4 * 10^9 com int estoura para -294967296, uma solucao sem long long ENCONTRARIA esta quadrupla e falharia 
	int		t4[] = { 1000000000, 1000000000, 1000000000, 1000000000 };
####Teste 5: negativos e simetrias - 8 quadruplas 
	int		t5[] = { -3, -2, -1, 0, 0, 1, 2, 3 };
	int		e5[][4] = { { -3, -2, 2, 3 }, { -3, -1, 1, 3 }, { -3, 0, 0, 3 },
						{ -3, 0, 1, 2 }, { -2, -1, 0, 3 }, { -2, -1, 1, 2 },
						{ -2, 0, 0, 2 }, { -1, 0, 0, 1 } };
####Teste 6: exatamente 4 elementos que somam o alvo 
	int		t6[] = { 1, 2, 3, 4 };
	int		e6[][4] = { { 1, 2, 3, 4 } };
####Teste 7: exatamente 4 elementos que NAO somam o alvo 
	int		t7[] = { 1, 2, 3, 4 };
####Teste 8: todos iguais a zero - deve sair UMA quadrupla, nao varias 
	int		t8[] = { 0, 0, 0, 0, 0, 0 };
	int		e8[][4] = { { 0, 0, 0, 0 } };
####Teste 9: todos negativos com alvo negativo 
	int		t9[] = { -5, -4, -3, -2, -1 };
	int		e9[][4] = { { -4, -3, -2, -1 } };
####Teste 10: duplicatas espalhadas e desordenadas 
	int		t10[] = { 4, 3, 3, 4, 4, 2, 1, 2, 1, 1 };
	int		e10[][4] = { { 1, 1, 3, 4 }, { 1, 2, 2, 4 }, { 1, 2, 3, 3 } }; 

