# 04-07-2024
def verificar_idade():
    nome = input("Digite seu nome: ")
    ano_nascimento = int(input("Digite seu ano de nascimento: "))
    
    # Calculando a idade com base no ano atual
    import datetime
    ano_atual = datetime.datetime.now().year
    idade = ano_atual - ano_nascimento
    
    if idade < 18:
        print("Desculpe, você é menor de idade e não pode continuar.")
    else:
        escolaridade = input("Digite sua escolaridade (Ensino Médio completo ou Ensino Superior completo): ")
        
        if escolaridade.lower() == "ensino médio completo":
            print("Ótimo! Aqui estão algumas opções de cursos superiores para você considerar:")
            print("- Engenharia Civil")
            print("- Administração de Empresas")
            print("- Ciência da Computação")
        elif escolaridade.lower() == "ensino superior completo":
            print("Ótimo! Aqui estão algumas opções de pós-graduação para você considerar:")
            print("- MBA em Gestão de Projetos")
            print("- Mestrado em Ciência de Dados")
            print("- Especialização em Direito Tributário")
        else:
            print("Escolaridade não reconhecida. Por favor, digite 'Ensino Médio completo' ou 'Ensino Superior completo'.")
