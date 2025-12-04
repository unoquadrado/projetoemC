#include <stdio.h>
#include <string.h>
#include <math.h>

int main() {
    // dados da primeira carta
    char estado[3], cidade[20], codigo[5];
    int carta, ponto_turistico;
    unsigned int populacao;
    float area, pib, densidadepopulacional, pibpercapita;

    // dados da segunda carta  
    char estado2[3], cidade2[20], codigo2[5];
    int carta2, ponto_turistico2;
    unsigned int populacao2;
    float area2, pib2, densidadepopulacional2, pibpercapita2;

    // Cadastro da primeira carta
    printf("=== CADASTRO PRIMEIRA CARTA ===\n");
    printf("Digite o numero da carta: \n");
    scanf("%d", &carta);
    
    printf("Digite o estado (sigla): \n");
    scanf("%s", estado);
    
    printf("Digite o código: \n");
    scanf("%s", codigo);
    
    printf("Digite a cidade: \n");
    scanf("%s", cidade);
    
    printf("Digite a população: \n");
    scanf("%u", &populacao);
    
    printf("Digite a área (km²): \n");
    scanf("%f", &area);
    
    printf("Digite o PIB (bilhões): \n");
    scanf("%f", &pib);
    
    printf("Digite o numero de pontos turísticos: \n");
    scanf("%d", &ponto_turistico);
    
    // Cálculos primeira carta
    densidadepopulacional = populacao / area;
    pibpercapita = (pib * 1000) / populacao;

    // Cadastro da segunda carta
    printf("\n=== CADASTRO SEGUNDA CARTA ===\n");
    printf("Digite o numero da carta: \n");
    scanf("%d", &carta2);

    if (carta2 == carta ? printf("Os Valores nao podem ser iguais!\n"), 1 : 0) return 1;
    
    printf("Digite o estado (sigla): \n");
    scanf("%s", estado2);

    if(strcmp(estado2, estado) == 0 ? printf("Os Valores nao podem ser iguais!\n"), 1 : 0) return 1;if(strcmp(estado2, estado) == 0 ? printf("Os Estados nao podem ser iguais!\n"), 1 : 0) return 1;
    
    printf("Digite o código: \n");
    scanf("%s", codigo2);

    if(strcmp(codigo2, codigo) == 0 ? printf("Os Valores nao podem ser iguais!\n"), 1 : 0) return 1;if(strcmp(estado2, estado) == 0 ? printf("Os Estados nao podem ser iguais!\n"), 1 : 0) return 1;
    
    printf("Digite a cidade: \n");
    scanf("%s", cidade2);

    if(strcmp(cidade2, cidade) == 0 ? printf("Os Valores nao podem ser iguais!\n"), 1 : 0) return 1;if(strcmp(estado2, estado) == 0 ? printf("Os Estados nao podem ser iguais!\n"), 1 : 0) return 1;
    
    printf("Digite a população: \n");
    scanf("%u", &populacao2);

    if (populacao2 == populacao ? printf("Os Valores nao podem ser iguais!\n"), 1 : 0) return 1;

    
    printf("Digite a área (km²): \n");
    scanf("%f", &area2);

    if(fabs(area2 - area) < 0.0001f ? printf("Os Valoes nao podem ser iguais!\n"), 1 : 0) return 1;
    
    printf("Digite o PIB (bilhões): \n");
    scanf("%f", &pib2);

    if(fabs(pib2 - pib) < 0.0001f ? printf("Os Valoes nao podem ser iguais!\n"), 1 : 0) return 1;
    
    printf("Digite o numero de pontos turísticos: \n");
    scanf("%d", &ponto_turistico2);

    if (ponto_turistico2 == ponto_turistico ? printf("As Cartas nao podem ser iguais!\n"), 1 : 0) return 1;
    
    // Cálculos segunda carta
    densidadepopulacional2 = populacao2 / area2;
    pibpercapita2 = (pib2 * 1000) / populacao2;

    // MENU INTERATIVO - switch
    printf("\n=== SUPER TRUNFO - COMPARAÇÃO DE CARTAS ===\n");
    printf("Cartas cadastradas:\n");
    printf("1. %s, %s (Carta %d)\n", cidade, estado, carta);
    printf("2. %s, %s (Carta %d)\n", cidade2, estado2, carta2);
    printf("\nEscolha o atributo para comparar:\n");
    printf("1 - População\n");
    printf("2 - Área\n");
    printf("3 - PIB\n");
    printf("4 - Pontos Turísticos\n");
    printf("5 - Densidade Populacional\n");
    printf("Opção: ");
    
    int opcao;
    scanf("%d", &opcao);

    switch(opcao) {
        case 1: // População
            printf("\n=== COMPARAÇÃO: POPULAÇÃO ===\n");
            printf("%s: %u habitantes\n", cidade, populacao);
            printf("%s: %u habitantes\n", cidade2, populacao2);
            
            if(populacao > populacao2) {
                printf("VENCEDOR: %s!\n", cidade);
            } else if(populacao2 > populacao) {
                printf("VENCEDOR: %s!\n", cidade2);
            } else {
                printf("EMPATE!\n");
            }
            break;
            
        case 2: // Área
            printf("\n=== COMPARAÇÃO: ÁREA ===\n");
            printf("%s: %.2f km²\n", cidade, area);
            printf("%s: %.2f km²\n", cidade2, area2);
            
            if(area > area2) {
                printf("VENCEDOR: %s!\n", cidade);
            } else if(area2 > area) {
                printf("VENCEDOR: %s!\n", cidade2);
            } else {
                printf("EMPATE!\n");
            }
            break;
            
        case 3: // PIB
            printf("\n=== COMPARAÇÃO: PIB ===\n");
            printf("%s: %.2f bilhões\n", cidade, pib);
            printf("%s: %.2f bilhões\n", cidade2, pib2);
            
            if(pib > pib2) {
                printf("VENCEDOR: %s!\n", cidade);
            } else if(pib2 > pib) {
                printf("VENCEDOR: %s!\n", cidade2);
            } else {
                printf("EMPATE!\n");
            }
            break;
            
        case 4: // Pontos Turísticos
            printf("\n=== COMPARAÇÃO: PONTOS TURÍSTICOS ===\n");
            printf("%s: %d pontos\n", cidade, ponto_turistico);
            printf("%s: %d pontos\n", cidade2, ponto_turistico2);
            
            if(ponto_turistico > ponto_turistico2) {
                printf("VENCEDOR: %s!\n", cidade);
            } else if(ponto_turistico2 > ponto_turistico) {
                printf("VENCEDOR: %s!\n", cidade2);
            } else {
                printf("EMPATE!\n");
            }
            break;
            
        case 5: // Densidade Populacional (regra invertida)
            printf("\n=== COMPARAÇÃO: DENSIDADE POPULACIONAL ===\n");
            printf("%s: %.2f hab/km²\n", cidade, densidadepopulacional);
            printf("%s: %.2f hab/km²\n", cidade2, densidadepopulacional2);
            printf("(Menor densidade vence!)\n");
            
            if(densidadepopulacional < densidadepopulacional2) {
                printf("VENCEDOR: %s!\n", cidade);
            } else if(densidadepopulacional2 < densidadepopulacional) {
                printf("VENCEDOR: %s!\n", cidade2);
            } else {
                printf("EMPATE!\n");
            }
            break;
            
        default:
            printf("Opção inválida!\n");
            break;
    }

    return 0;
}