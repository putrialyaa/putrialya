#include <stdio.h>
#include <windows.h>
int main() {
    int lebar = 10, tinggi = 5;
    int posisi = 0;

    printf("Masukkan lebar (min 10, max 100): ");
    scanf("%d", &lebar);
    printf("Masukkan tinggi (min 5, max 75): ");
    scanf("%d", &tinggi);
    while (1) {
        for (int k = 0; k < 50; k++) {
            printf("\n");
        }
        for (int i = 0; i < tinggi; i++) {
            for (int j = 0; j < posisi; j++) {
                printf(" ");
            }
            for (int j = 0; j < lebar; j++) {
                printf("* ");
            }
            printf("\n");
        }
        posisi++;
        if (posisi + lebar > 100) posisi = 0;
        Sleep(100);
    }
    return 0;
}
