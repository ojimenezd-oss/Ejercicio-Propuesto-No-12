# Ejercicio-Propuesto-No-12
class Nomina:
    @staticmethod
    def calcular_salario_bruto(horas_trabajadas, valor_hora):
        return horas_trabajadas * valor_hora

    @staticmethod
    def calcular_valor_retefuente(porcentaje_retefuente, salario_bruto):
        return porcentaje_retefuente * salario_bruto

    @staticmethod
    def calcular_salario_neto(salario_bruto, valor_retefuente):
        return salario_bruto - valor_retefuente


horas_trabajadas = 48.0
valor_hora = 5000.0
retencion = 12.5
porcentaje_retefuente = retencion / 100

salario_bruto = Nomina.calcular_salario_bruto(horas_trabajadas, valor_hora)
valor_retefuente = Nomina.calcular_valor_retefuente(porcentaje_retefuente, salario_bruto)
salario_neto = Nomina.calcular_salario_neto(salario_bruto, valor_retefuente)

print("Salario Bruto:" , salario_bruto)
print("Retención en la Fuente: ", valor_retefuente)
print("Salario Neto:", salario_neto)
