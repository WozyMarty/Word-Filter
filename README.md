General Search Tools / Word Filter (mainly to ABB & FANUC)

Este projeto contém diferentes versões de ferramentas para busca e filtragem de pontos de solda em arquivos ABB (.mod / texto), com geração de saída em .csv.
As versões v5 permite acessar os arquivos de FANUC também, caso deseje filtrar os pontos de solda, recomendase a opçao FullLine do v5.

	Versões principais
	
///ABB_FullLine_csvAuto_v4///

Versão que realiza a execução automática ao carregar o arquivo PRG_MVT.mod.

	- Busca e filtra apenas pontos de solda válidos (SR_SOUDER)
	- Ignora linhas comentadas com !
	- Gera um arquivo .csv com a linha completa encontrada
	- Os dados podem ser posteriormente tratados no Excel

Exemplo de saída:
2496 | SR_SOUDER SCS1D009543_L2H2,V_rapide,1,1,Tool_Pince1,wobj_XDF;

///ABB_twoLine_csvAuto_v4///

Versão semelhante à FullLine, porém com saída reduzida.

	- Mantém apenas:
	- Tipo do ponto (SR_SOUDER)
	- Nome do ponto (SCS1D009543)
	- Ideal para visualização rápida e simplificada

Exemplo de saída:
2496 | SR_SOUDER SCS1D009543;

///ENTERSearch_v5.5 (Recomendada)///

Versão final com interface gráfica (GUI) usando wxWidgets.

	- Permite selecionar qualquer arquivo de texto
	- Campo de busca manual
	- Alternância entre:
		- Full Line
		- Two Line
	- Botão para exportar resultados em .csv
	- Terminal interno para visualização do output

///AUTOSearch_v5.4///

Versão anterior com busca automática em tempo real.

	- Pesquisa automática enquanto o usuário digita
	- Sem botão de search
	- Interface menos otimizada (pode travar durante a digitação)
	- Nao sera arrumado

///Observações
	- Todas as versões são compatíveis com arquivos de texto padrao, programas ABB, FANUC apenas v5
	- As versões mais recentes focam em usabilidade e interface gráfica
	- O formato .csv pode exigir ajuste no Excel dependendo da região/configuração