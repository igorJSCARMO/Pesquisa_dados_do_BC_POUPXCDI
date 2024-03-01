# Pesquisando_dados_financeiros_do_Banco_Central
Este é um código Python de referência para pesquisa de dados financeiros públicos no sistema do Banco central brasileiro.

import numpy as np
import pandas as pd
import investpy as inv
from matplotlib import pyplot as plt
from bcb import sgs

#https://www3.bcb.gov.br/sgspub/localizarseries/localizarSeries.do?method=prepararTelaLocalizarSeries

ComparativoBCB = sgs.get({"Poupança" : 196,"CDI" : 4391,}, start = "2023-01-01", end = "2023-12-31")

ComparativoBCB

