# all-technology
# Script para planejar custos de expansão de infraestrutura TI

def calcular_custos(num_funcionarios_novos, custo_por_funcionario=1500, custo_aws_mensal=500):
    custo_equipamentos = num_funcionarios_novos * custo_por_funcionario
    custo_anual_aws = custo_aws_mensal * 12
    total = custo_equipamentos + custo_anual_aws
    print(f"Custo para {num_funcionarios_novos} novos funcionários: R${custo_equipamentos}")
    print(f"Custo anual AWS: R${custo_anual_aws}")
    print(f"Total estimado: R${total}")
    return total

# Exemplo: Expansão de 9 para 30 funcionários (21 novos)
calcular_custos(21)
