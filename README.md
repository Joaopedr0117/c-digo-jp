CPF = "01683794575"
SOMA_NOVE = (int(CPF[0]) * 10) + (int(CPF[1]) * 9) + (int(CPF[2]) * 8) + (int(CPF[3]) * 7) + (int(CPF[4]) * 6) + (int(CPF[5]) * 5) + (int(CPF[6]) *4) + ( int(CPF[7]) * 3) + (int(CPF[8]) * 2)



DIVISAO_NOVE = SOMA_NOVE % 11

if(DIVISAO_NOVE < 2):
    PRIMEIRO = 0
elif(DIVISAO_NOVE >= 2):
    PRIMEIRO = 11 - DIVISAO_NOVE

SOMA_DEZ = (int(CPF[0]) * 11) + (int(CPF[1]) * 10) + (int(CPF[2]) * 9) + (int(CPF[3]) * 8) + (int(CPF[4]) * 7) + (int(CPF[5]) * 6) + (int(CPF[6]) * 5) + (int(CPF[7]) * 4) + (int(CPF[8]) * 3) + (int(CPF[9]) * 2)

DIVISAO_DEZ = SOMA_DEZ % 11

if(DIVISAO_DEZ < 2):
    SEGUNDO = 0

elif(DIVISAO_DEZ >= 2):
    SEGUNDO = 11 - DIVISAO_DEZ

if(PRIMEIRO == int(CPF[9])) and (SEGUNDO == int(CPF[10])):
    print("CPF Válido")
else:
    print("CPF Inválido")


