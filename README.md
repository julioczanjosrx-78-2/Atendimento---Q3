#include <stdio.h>

int main() {
    float nota, total = 0, media;
    int i;

    for (i = 1; i <= 10; i++) {
        printf("Nota do cliente %d (0 a 10): ", i);
        scanf("%f", &nota);
        total = total + nota;
    }

    media = total / 10;
    printf("\nMedia geral: %.2f\n", media);

    if (media < 7) {
        printf("ALERTA: a media esta abaixo de 7!\n");
    }

    return 0;
}
