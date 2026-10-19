# reservat-rio
Python 3.14.7 (tags/v3.14.7:823f032, Aug  5 2026, 10:51:32) [MSC v.1944 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
...   for item in niveis_reservatorio:
...     if item["nivel"] == nivel_dado:
...       item_encontrado = item
...       break
...
...   if item_encontrado:
...     # Exibe a mensagem formatada com a cor específica
...     print(
...         f"{item_encontrado['cor']}[Nível {item_encontrado['nivel']}]"
...         f" Reservatório em estado: {item_encontrado['situacao']}{Style.RESET_ALL}"
...     )
...   else:
...     print(f"{Fore.MAGENTA}Nível inválido informado.{Style.RESET_ALL}")
...
...
... def simular_monitoramento():
...   """Simula o monitoramento do reservatório passando por diferentes níveis."""
...   print("=== SISTEMA DE MONITORAMENTO DE RESERVATÓRIO ===")
...   print("Iniciando simulação dos níveis de água...\n")
...
...   # Simulando a variação dos níveis de 1 a 5
...   leituras_simuladas = [1, 2, 3, 4, 5, 3, 1]
...
...   for leitura in leituras_simuladas:
...     exibir_alerta(leitura)
...
...
... if __name__ == "__main__":
...   simular_monitoramento()
...
=== SISTEMA DE MONITORAMENTO DE RESERVATÓRIO ===
Iniciando simulação dos níveis de água...

[Nível 1] Reservatório em estado: Muito baixo (crítico)
[Nível 2] Reservatório em estado: Baixo
[Nível 3] Reservatório em estado: Médio
[Nível 4] Reservatório em estado: Alto
[Nível 5] Reservatório em estado: Muito alto (alerta)
[Nível 3] Reservatório em estado: Médio
[reservatorio.py](https://github.com/user-attachments/files/33644363/reservatorio.py)
