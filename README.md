
# atv-iago


1:

            #include <stdio.h>

            int main() {
                int matriz[2][2] = {
                    {3, 4},
                    {5, 6}
                };

                printf("Matriz 2x2 com os números 3, 4, 5, 6:\n");
                for (int i = 0; i < 2; i++) {
                    for (int j = 0; j < 2; j++)
                        printf("%d ", matriz[i][j]);
                    printf("\n");
                }

                return 0;
            }


2:

#include <stdio.h>

int main() {
    int matriz[3][3] = {
        {3, 4, 5},
        {7, 8, 3},
        {4, 5, 7}
    };

    printf("Matriz 3x3:\n");
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++)
            printf("%d ", matriz[i][j]);
        printf("\n");
    }

    printf("\nDiagonal principal:\n");
    for (int i = 0; i < 3; i++)
        printf("%d ", matriz[i][i]);

    printf("\n");
    return 0;
}

3:


#include <stdio.h>

int main() {
    int matriz[2][3] = {
        {4, 7, 2},
        {1, 5, 6}
    };
    int soma = 0;

    printf("Matriz 2x3:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++) {
            printf("%d ", matriz[i][j]);
            soma += matriz[i][j];
        }
        printf("\n");
    }

    printf("Soma dos elementos: %d\n", soma);
    return 0;
}


4:

#include <stdio.h>

int main() {
    int matriz[3][3] = {
        {12, 7, 5},
        {9, 18, 3},
        {4, 6, 15}
    };
    int maior = matriz[0][0];

    for (int i = 0; i < 3; i++)
        for (int j = 0; j < 3; j++)
            if (matriz[i][j] > maior)
                maior = matriz[i][j];

    printf("Maior valor da matriz: %d\n", maior);
    return 0;
}


5:

#include <stdio.h>

int main() {
    int matriz[3][2] = {
        {2, 5},
        {8, 3},
        {4, 7}
    };
    int pares = 0;

    for (int i = 0; i < 3; i++)
        for (int j = 0; j < 2; j++)
            if (matriz[i][j] % 2 == 0)
                pares++;

    printf("Quantidade de números pares: %d\n", pares);
    return 0;
}


6:

#include <stdio.h>

int main() {
    int matriz[2][2] = {
        {1, 2},
        {3, 4}
    };
    int temp;

    // Troca as linhas
    for (int j = 0; j < 2; j++) {
        temp = matriz[0][j];
        matriz[0][j] = matriz[1][j];
        matriz[1][j] = temp;
    }

    printf("Matriz após troca de linhas:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++)
            printf("%d ", matriz[i][j]);
        printf("\n");
    }

    return 0;
}

7:

#include <stdio.h>

int main() {
    int matriz[2][3] = {
        {10, 20, 30},
        {40, 50, 60}
    };

    printf("Matriz 2x3 formatada:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++)
            printf("%d\t", matriz[i][j]);
        printf("\n");
    }

    return 0;
}

8:
#include <stdio.h>

int main() {
    int matriz[3][3] = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9}
    };
    int soma;

    for (int i = 0; i < 3; i++) {
        soma = 0;
        for (int j = 0; j < 3; j++)
            soma += matriz[i][j];
        printf("Soma da linha %d: %d\n", i, soma);
    }

    return 0;
}

9:

#include <stdio.h>

int main() {
    int matriz[2][3] = {
        {1, 2, 3},
        {4, 5, 6}
    };
    int transposta[3][2];

    // Gera a transposta
    for (int i = 0; i < 2; i++)
        for (int j = 0; j < 3; j++)
            transposta[j][i] = matriz[i][j];

    // Exibe a transposta
    printf("Matriz transposta (3x2):\n");
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 2; j++)
            printf("%d\t", transposta[i][j]);
        printf("\n");
    }

    return 0;
}

