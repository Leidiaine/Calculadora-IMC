# Calculadora-IMC
Codigo em c #include <stdio.h>

int main() {
    float peso, altura, imc;
    float somaIMC = 0;
    int qtdUsuarios = 0;
    int opcao;

    printf("=====================================\n");
    printf("     SISTEMA DE CALCULO DE IMC\n");
    printf("=====================================\n\n");

    do {
        printf("MENU PRINCIPAL\n");
        printf("1 - Calcular IMC de um usuario\n");
        printf("2 - Mostrar media geral dos IMCs\n");
        printf("3 - Sair\n");
        printf("Escolha uma opcao: ");
        scanf("%d", &opcao);

        if (opcao == 1) {
            printf("\nDigite o peso (kg): ");
            scanf("%f", &peso);
            printf("Digite a altura (m): ");
            scanf("%f", &altura);

            imc = peso / (altura * altura);
            printf("\nIMC calculado: %.2f\n", imc);

            if (imc < 18.5) {
                printf("Classificacao: Abaixo do peso\n");
            } else if (imc < 24.9) {
                printf("Classificacao: Peso normal\n");
            } else if (imc < 29.9) {
                printf("Classificacao: Sobrepeso\n");
            } else if (imc < 34.9) {
                printf("Classificacao: Obesidade Grau I\n");
            } else if (imc < 39.9) {
                printf("Classificacao: Obesidade Grau II\n");
            } else {
                printf("Classificacao: Obesidade Grau III (morbida)\n");
            }

            somaIMC += imc;
            qtdUsuarios++;
            printf("-------------------------------------\n\n");

        } else if (opcao == 2) {
            if (qtdUsuarios > 0) {
                printf("\nMedia geral dos IMCs: %.2f\n", somaIMC / qtdUsuarios);
            } else {
                printf("\nNenhum IMC foi calculado ainda.\n");
            }
            printf("-------------------------------------\n\n");

        } else if (opcao == 3) {
            printf("\nEncerrando o programa...\n");
            printf("Obrigado por utilizar o sistema de IMC!\n");

        } else {
            printf("\nOpcao invalida! Tente novamente.\n\n");
        }

    } while (opcao != 3);

    return 0;
}
