import pyautogui

import time
 
import pandas as pd

pyautogui.press("win")

pyautogui.sleep(2)


pyautogui.write("chrome")

pyautogui.sleep(5)

pyautogui.press("enter")

pyautogui.sleep(5)

pyautogui.write("https://dlp.hashtagtreinamentos.com/python/intensivao/login")

pyautogui.sleep(5)

pyautogui.press("enter")
pyautogui.sleep(5)
pyautogui.click(x=433, y=365)
pyautogui.sleep(10)
pyautogui.write("isaacvieira2")   
pyautogui.click(x=445, y=474)
pyautogui.write("isaacrei")
pyautogui.sleep(3)
pyautogui.press("enter")
pyautogui.sleep(5)

#escrever a tabela no terminal


import pandas as pd

# Carregar a tabela de produtos
tabela = pd.read_csv("produtos.csv")

print(tabela)

for linha in tabela.index:
    # clicar no campo de código
    pyautogui.click(x=397, y=264)
    # pegar da tabela o valor do campo que a gente quer preencher
    codigo = tabela.loc[linha, "codigo"]
    pyautogui.sleep(2)
    # preencher o campo
    pyautogui.write(str(codigo))
    # passar para o proximo campo
    pyautogui.press("tab")
    # preencher o campo
    pyautogui.sleep(2)
    pyautogui.write(str(tabela.loc[linha, "marca"]))
    pyautogui.press("tab")
    pyautogui.sleep(2)
    pyautogui.write(str(tabela.loc[linha, "tipo"]))
    pyautogui.press("tab")
    pyautogui.sleep(2)
    pyautogui.write(str(tabela.loc[linha, "categoria"]))
    pyautogui.press("tab")
    pyautogui.sleep(2)
    pyautogui.write(str(tabela.loc[linha, "preco_unitario"]))
    pyautogui.press("tab")
    pyautogui.sleep(2)
    pyautogui.write(str(tabela.loc[linha, "custo"]))
    pyautogui.press("tab")
    pyautogui.sleep(2)
    obs = tabela.loc[linha, "obs"]
    if not pd.isna(obs):
        pyautogui.write(str(tabela.loc[linha, "obs"]))
    pyautogui.press("tab")
    pyautogui.press("enter") # cadastra o produto (botao enviar)
    # dar scroll de tudo pra cima
    pyautogui.scroll(5000)
    # Passo 5: Repetir o processo de cadastro até o fim
