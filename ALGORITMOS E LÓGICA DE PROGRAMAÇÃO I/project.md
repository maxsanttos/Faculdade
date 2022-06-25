# Algoritmo "cadastrodecliente"

//Engelharia de Software
// Realizado em Portugol

Var
    cliente :Vetor[1..20] de caractere
    valor:Vetor[1..20,1..10] de real
    soma,somatot,valortot:real
    opcao,opcaoc,opcaov:inteiro
    i,j,r:inteiro

Início
Repita
    Escreval("==================")
    Escreval("MERCEARIA DO JOSÉ")
    Escreval("==================")
    Escreval("Menu")
    Escreval("1-Registro")
    Escreval("2-Clientes")
    Escreval("3-Cliente Específico")
    Escreval("4-Sair")
    Escreval("Opção:")
    Leia(opcao)
    cliente[1]<-"Nagata"
    cliente[2]<-"Fred"
    cliente[3]<-"Coriga"
    cliente[4]<-"Martin"
    cliente[5]<-"Jason"
    cliente[6]<-"Henrique"
    cliente[7]<-"Pedro joao"
    cliente[8]<-"Ricardo"
    cliente[9]<-"Andre"
    cliente[10]<-"Marilia"
    cliente[11]<-"Pedro"
    cliente[12]<-"Josefa"
    cliente[13]<-"Maguinolia"
    cliente[14]<-"Marilda"
    cliente[15]<-"Antonio"
    cliente[16]<-"Mateus"
    cliente[17]<-"Manuel"
    cliente[18]<-"Marcos"
    cliente[19]<-"Zé"
    cliente[20]<-"Herinalda"
    Caso(opcao)
		Seja 1 faça
			Para i de 1 ate 20 passo 1 faca
				Escreval("-----------------------")
				Escreval("CLiente ",cliente[i])
				Para j de 1 ate 10 passo 1 faca
                    		 	valor[i,j] <- aleatório(200)
                    			Escreval("Notas",j," R$:",valor[i,j])
                    			soma <- soma+valor[i,j]
                    			somatot <- somatot + soma
                    			soma<-0
				Fim_para
			Fim_para
		Seja 2 faça
			Para i de 1 ate 20 passo 1 faça
				Escreval("---------------------------------")
				Escreval("CLiente ",cliente[i],":")
				valortot <- valortot + valor[i,1]  + valor[i,2] + valor[i,3] + valor[i,4]+ valor[i,5] + valor[i,6] + valor[i,7] + valor[i,8] + valor[i,9] + valor[i,10]
				Escreval("Tem o valor a pagar é de R$:",valortot)
				valortot <-0
			Fim_para
			Escreval("-----------------------------------------------------------")
			Escreval("Valor total de todas as notas é de R$:",somatot)
		Seja 3 faça
			Repita
				Escreval("1-Cliente Específico!")
				Escreval("0-Voltar ao menu Principal")
				Leia(opcaoc)
				Se(opcaoc = 1) então
					Escreval("Escolha um cliente 1 à 20 para ver sua informações")
					Leia(opcaov)
					Escreval("------------------------------")
					Escreval("Cliente:",cliente[opcaov])
					Escreval("A nota do cliente ",cliente[opcaov]," é: ",valor[opcaov,1],valor[opcaov,2],valor[opcaov,3],valor[opcaov,4],valor[opcaov,5],valor[opcaov,6],valor[opcaov,7],valor[opcaov,8],valor[opcaov,9],valor[opcaov,10])
					valortot <- valortot+valor[opcaov,1]+valor[opcaov,2]+valor[opcaov,3]+valor[opcaov,4]+valor[opcaov,5]+valor[opcaov,6]+valor[opcaov,7]+valor[opcaov,8]+valor[opcaov,9]+valor[opcaov,10]
					Escreval("O valor da Nota do cliente é R$:",Valortot)
					valortot <- 0
				Fim_se
			Até_que(opcaoc= 0)
			Escreval("Voltando ao Menu Pricipal")
    Fim_caso
Até_que(opcao=4)
Escreval("Fim Do Programa!!")
Fim