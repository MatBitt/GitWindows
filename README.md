# GitWindows
Para começarmos a usar o GitHub é necessário tê-lo baixado e instalado em seu computador. Para isso, usaremos esse link:

https://gitforwindows.org/

Agora que você já tem o Git instalado em seu computador, vamos vinculá-lo a sua conta no site.
Abra o aplicativo do Git e digite esse códigos de comando:

git config --global user.name "SeuNome"
git config --global user.email "SeuEmail@OQue.com"
git config --global credential.helper cache

Obs.: digite as aspas.

-------

Para editar nossos arquivos, é necessário um bom editor de texto e ferramentas as quais são muito úteis. Porque a maioria das pessoas da Droid-UnB conhece o Sublime, nós o usaremos. Desta maneira, iremos mostrar como instalar o Sublime. Se você está usando outro editor de texto como Notepad++, TextMate 2, Kate ou Gedit, talvez eles sejam muito bons e úteis, contudo não é garantido que esses editores de texto funcionem bem com o git.

Você pode instalar o sumblime em seu site oficial: 

https://www.sublimetext.com/

Agora para torná-lo seu editor de texto do Git primeiro devemos torná-lo um comando existente no seu bash. Para isso, basta seguir esse passo a passo:

Passo 1:
	Abra as propriedades do seu computador (Vá em meu computador, clique com o botão direito e clique em propriedades), clique em configurações avançadas do sistema e clique em Variáveis 
de ambiente. 

Passo 2:
	Ache o diretório onde seu sublime está (o caminho que leva até ele) e copie esse diretório.
	Ex.: C:\Program Files\Sublime Text 3

Passo 3:
	Volte na aba das variáveis de ambiente e clique em Novo na caixa das Variáveis do Sistema.

Passo 4:
	No nome da variável escreva SUBLIME e em seu valor cole o diretório
	Ex.: Nome da Variável: SUBLIME
		 Valor da Variável: C:\Program Files\Sublime Text 3

	Clique em OK.

Passo 5:
	Ainda na caixa das Variáveis do Sistema, ache a variável Path e clique em editar.
	Dentro da nova caixa, clique em novo e escreva: %SUBLIME%
	Clique em OK em todas as caixas abertas.

Passo 6:
	Abra o Git e digite: subl.exe
	Caso dê erro, feche tudo e tente novamente.

Ao final de tudo, para torná-lo seu editor de texto, abra o git e digite: subl ~/.gitconfig

Fazendo isso, o sublime text irá aparecer. Dentro desse arquivo você tem as configurações do git. Então, por fim, acrescente ao final do arquivo as linhas: 

[core]
	editor = subl -w

Salve e feche.
