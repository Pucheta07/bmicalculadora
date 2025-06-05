# bmicalculadora
Legajo:417062 Estudiante: Pucheta Benjamin

#include <stdio.h>

int main(void) {
    float p, a, A, imc;

    printf("Ingrese su peso: ");
    scanf("%f", &p);
    printf("Ingrese su altura en cm: ");
    scanf("%f", &a);
    A = a/100;
    imc = p / (A * A);

    printf("Su índice de masa corporal es: %.2f\n", imc);

    if (imc < 18.5) {
        printf("Condición: Bajo peso\n");
    } else if (imc >= 18.5 && imc <= 24.9) {
        printf("Condición: Normal\n");
    } else if (imc >= 25.0 && imc <= 29.9) {
        printf("Condición: Sobrepeso\n");
    } else if (imc >= 30.0) {
        printf("Condición: Obesidad\n");
    }
    printf("\n%-10s| %-15s\n", "Índice", "Condición");
    printf("-----------------------------\n");
    printf("<18.5     | Bajo peso\n");
    printf("18.5-24.9 | Normal\n");
    printf("25.0-29.9 | Sobrepeso\n");
    printf(">=30      | Obesidad\n");
    return 0;
//Al parecer ya lo habia hecho al codigo diculpa profe
}
