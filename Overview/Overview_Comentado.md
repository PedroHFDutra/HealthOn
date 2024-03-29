## HealthOn -> Aplicação para cadastro de pacientes 
## Features: Cadastro de Pacientes; Menu de Opções; Cadastro de Alergias Medicamentosas; Consulta de Informações; Preenchimento de Evolução Médica

    Algoritmo health_On
    Procedimento cadastrarPct( )
        Var: 
            nome_pct : Vetor [1..500] de caractere
            nome_mae : Vetor [1..500] de caractere
            data_nascimento : Vetor  [1..200] de caractere
            nome_municipio : Vetor [1..200] de caractere
            idade, respostaMenu : inteiro
            peso, altura : real

        Inicio

            Escreval("Vamos iniciar o cadastro de pacientes!")
            Escreval("Preencha as informações para prosseguirmos com o cadastro...")
            Escreval("Primeiro, informe seu nome completo:")
            Leia(nome_pct)
            Escreval("Informe sua data de nascimento:")
            Leia(data_nascimento)
            Escreval("Informe sua idade:")  
            Leia(idade)
            Escreval("Informe seu peso:")
            Leia(peso)
            Escreval("Agora, informe sua altura:")
            Leia(altura)
            Escreval("Informe o nome completo de sua mãe:")
            Leia(nome_mae)
            Escreval("Informe o nome do seu município de residência:")
            Leia(nome_municipio)
            Escreval("Cadastro Realizado!")
            //Limpar o prompt (fflush)
            Escreval("Verifique as informações adicionadas:")
            Escreval("Nome do paciente:", nome_pct)
            Escreval("Idade:", idade)
            Escreval("Nome da Mãe:", nome_mae)
            Escreval("Altura:", altura "/", "Peso:", peso)
            Escreval("Data de Nascimento:", data_nascimento "/", "Idade:", idade)
            Escreval(Município de Residência:", nome_municipio)
            Escreval("Para confirmar os dados cadastrados, digite: 1 para SIM ou 2 para NÃO")
            Leia(respostaMenu)
                Se(respostaMenu = 1) faça
                    Escreval("Os dados cadastrados foram armazenados com sucesso!")
                Senão
                    Se(respostaMenu = 2) faça 
                        Escreval("Os dados cadastrados não foram armazenados, Cadastro de Paciente não concluído.")
                Fim_Se
                    Se (respostaMenu > 2) faça  
                        Escreval("Opção Inválida!")
                    Fim_Se
        Fim_Procedimento

    Procedimento alergia_Medicamentos( )
        Var:
            nome_pct : Vetor [1..500] de caractere
            nomeDoMedicamento : [1.600] de caractere
            idade, respostaMenu : inteiro
            peso, altura : real

        Inicio

            Escreval("Iniciando o cadastro de Alergias Medicamentosas para pacientes")
            Escreval("Preencha as informações para prosseguirmos com o cadastro...")
            Escreval("Informe seu nome completo:")
            Leia("nome_pct")
            Escreval("Informe sua idade:")
            Leia(idade)
            Escreval("Informe seu peso:")
            Leia(peso)
            Escreval("Agora, informe sua altura:")
            Leia(altura)
            Escreval("Informe o medicamento que você tenha alergia:")
            Leia(nomeDoMedicamento)
            Escreval("Para confirmar o cadastro da alergia, pressione: 1 - para SIM ou 2 - para NÃO")
            Leia(respostaMenu)
                Se(respostaMenu = 1) faça
                    Escreval("Os dados cadastrados foram armazenados com sucesso!")
                Senão
                    Se(respostaMenu = 2) faça 
                        Escreval("Os dados cadastrados não foram armazenados, Cadastro de Alergias Medicamentosas não concluído.")
                Fim_Se
                    Se (respostaMenu > 2) faça  
                        Escreval("Opção Inválida!")
                    Fim_Se
        Fim_Procedimento

    Procedimento insercaoEvolucao( )
        Var:
            nome_pct : Vetor [1..500] de caractere
            evolucao_cadastro : [1.1000] de caractere
            idade, respostaMenu : inteiro
            peso, altura : real

        Inicio

            Escreval("Deseja evoluir o paciente recém cadastrado?")
            Escreval("Para prosseguir, pressione: 1 - para SIM ou 2 - para NÃO")
            Leia(respostaMenu)
            Se(respostaMenu = 1) faça
                Escreval("Vamos prosseguir com a evolução médica...")
            Senão
                Se(respostaMenu = 2) faça 
                    Escreval("A evolução médica será encerrada.")
                Fim_Se
                    Se (respostaMenu > 2) faça  
                        Escreval("Opção Inválida!")
                    Fim_Se
                Escreval("Informe o nome completo do paciente para realizar a evolução")
                Leia(nome_pct)
                Escreval("Prosseguiremos com a evolução...")
                Escreval("Informe a Evolução Médica do paciente", nome_pct)
                Leia(evolucao_cadastro)
                Escreval("Evolução Médica cadastrada!")

        Fim_Procedimento


    Var
        nome_pct : Vetor [1..500] de caractere
        respostaMenu : inteiro

    Inicio

    Escreval("Seja bem-vindo ao HealthOn!")
    Escreval("Gostaria de iniciar os procedimentos?")
    Escreval("Para prosseguir, pressione: 1 - para SIM ou 2 - para NÃO")
        Leia(respostaMenu)
            Se(respostaMenu = 1) faça
                Escreval("Vamos iniciar os procedimentos!")
            Senão
                Se(respostaMenu = 2) faça 
                    Escreval("O programa será encerrado...")
                Fim_Se
                    Se (respostaMenu > 2) faça  
                        Escreval("Opção Inválida!")
                    Fim_Se

                        Escreval("Primeiro, iniciaremos o procedimento de Cadastro de Paciente!")
                        Escreval("Iniciando o procedimento em...")
                        Escreval("...3")
                        Escreval("...2")
                        Escreval("...1")
                        Escreval("...")

                            cadastrarPct( )

                            Escreval("Vamos prosseguir com o próximo procedimento...")
                            Escreval("Iniciando o procedimento de Cadastro de Alergia Medicamentosa!")
                            Escreval("Iniciando o procedimento em...")
                            Escreval("...3")
                            Escreval("...2")
                            Escreval("...1")
                            Escreval("...")

                                 alergia_Medicamentos( )

                                 Escreval("Vamos prosseguir com o próximo procedimento...")
                                 Escreval("Iniciando o procedimento de Cadastro de Evolução Médica!")
                                 Escreval("Iniciando o procedimento em...")
                                 Escreval("...3")
                                 Escreval("...2")
                                 Escreval("...1")
                                 Escreval("...")

                                     insercaoEvolucao( )

                                     Escreval("Procedimentos finalizados!")
                                     Escreval("Muito Obrigado por utilizar nosso Software!")
                                     Escreval("Desenvolvido por: Pedro Dutra")
                                     
    Fim
