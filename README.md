# prueba_01
#include <stdio.h>
#include <string.h>

int main() {
    char password[10];
    printf("Ingrese la contraseña: ");
    gets(password); // Error de buffer overflow
    
    if (strcmp(password, "secreto123") == 0) {
        printf("Contraseña correcta. Acceso concedido.\n");
    } else {
        printf("Contraseña incorrecta. Acceso denegado.\n");
    }
    
    return 0;
}
