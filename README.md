# ExercioAvaliativo4AED1
## Nome: João Pedro da Silva Netto
## LeetCode 18: 4sum
### (https://leetcode.com/problems/4sum/)
Esse leetcode fornecia um vetor de inteiros e um valor alvo. Deveriamos verificar quais conjuntos de 4 numeros do vetor, somados, resultavam no valor alvo, não podendo repetir e a ordem não importava dentro da matriz de resposta.

### Casos testados:
#### Teste 1: exemplo 1 do enunciado<br>
	int		t1[] = { 1, 0, -1, 0, -2, 2 };<br>
	int		e1[][4] = { { -2, -1, 1, 2 }, { -2, 0, 0, 2 }, { -1, 0, 0, 1 } };<br>
#### Teste 2: exemplo 2 do enunciado - duplicatas extremas <br>
	int		t2[] = { 2, 2, 2, 2, 2 };<br>
	int		e2[][4] = { { 2, 2, 2, 2 } };<br>
#### Teste 3: menos de 4 elementos - resposta vazia<br>
	int		t3[] = { 1, 2, 3 };<br>
#### Teste 4: overflow - 4 * 10^9 com int estoura para -294967296, uma solucao sem long long ENCONTRARIA esta quadrupla e falharia<br>
	int		t4[] = { 1000000000, 1000000000, 1000000000, 1000000000 };<br>
#### Teste 5: negativos e simetrias - 8 quadruplas <br>
	int		t5[] = { -3, -2, -1, 0, 0, 1, 2, 3 };<br>
	int		e5[][4] = { { -3, -2, 2, 3 }, { -3, -1, 1, 3 }, { -3, 0, 0, 3 },
						{ -3, 0, 1, 2 }, { -2, -1, 0, 3 }, { -2, -1, 1, 2 },
						{ -2, 0, 0, 2 }, { -1, 0, 0, 1 } };<br>
#### Teste 6: exatamente 4 elementos que somam o alvo <br>
	int		t6[] = { 1, 2, 3, 4 };<br>
	int		e6[][4] = { { 1, 2, 3, 4 } };<br>
#### Teste 7: exatamente 4 elementos que NAO somam o alvo <br>
	int		t7[] = { 1, 2, 3, 4 };<br>
#### Teste 8: todos iguais a zero - deve sair UMA quadrupla, nao varias <br>
	int		t8[] = { 0, 0, 0, 0, 0, 0 };<br>
	int		e8[][4] = { { 0, 0, 0, 0 } };<br>
#### Teste 9: todos negativos com alvo negativo <br>
	int		t9[] = { -5, -4, -3, -2, -1 };<br>
	int		e9[][4] = { { -4, -3, -2, -1 } };<br>
#### Teste 10: duplicatas espalhadas e desordenadas <br>
	int		t10[] = { 4, 3, 3, 4, 4, 2, 1, 2, 1, 1 };<br>
	int		e10[][4] = { { 1, 1, 3, 4 }, { 1, 2, 2, 4 }, { 1, 2, 3, 3 } }; <br>

