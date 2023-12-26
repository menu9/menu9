#include <stdio.h>

void displayMenu() {
    printf("1. Вибрати опцію 1\n");
    printf("2. Вибрати опцію 2\n");
    printf("3. Вибрати опцію 3\n");
    printf("4. Вийти з програми\n");
}

int main() {
    int choice;

    do {
        displayMenu();
        printf("Виберіть опцію: ");
        scanf("%d", &choice);

        switch (choice) {
            case 1:
                printf("Ви обрали опцію 1\n");
                break;
            case 2:
                printf("Ви обрали опцію 2\n");
                break;
            case 3:
                printf("Ви обрали опцію 3\n");
                break;
            case 4:
                printf("Дякую за використання програми. До побачення!\n");
                break;
            default:
                printf("Невірний вибір. Будь ласка, оберіть знову.\n");
        }
    } while (choice != 4);

    return 0;
}
