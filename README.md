# soundness cli PROOF

# OBSERVAÇÕES: 

1- ESSE TUTORIAL É PRA TODOS QUE ESTAO COM DIFICUDADES DE FAZER O PROOF VIA CLI.

2- ESSE TUTORIAL É PRA TODOS QUE TEM EM MÃOS A FRASE SECRETA DA KEY (Mnemonic)

2.1 - A FRASE SECRETA (Mnemonic) FOI GERADO QUANDO VOCê CRIOU A KEY E POSSUI 12,16,18 OU 24 DIGITOS.

3- PRA QUEM NÃO POSSUI O Mnemonic É PRECISO GERAR UMA NOVA KEY, SENDO ASSIM ATUALIZAREI O TUTORIAL POSTERIORMENTE CONFORME DEMANDA.

#CONFIGURAÇÃO DO CLI:

1- CRIE O REPOSITORIO NO SEU GITHUB CLICANDO EM NEW

<img width="318" height="50" alt="image" src="https://github.com/user-attachments/assets/c421acf0-12fb-4eb1-b705-beaec5f96219" />

1.1 - CONFIGURE O REPOSITORIO DA SEGUINTE FORMA E CLIQUE EM "CREATE REPOSITORY"

<img width="764" height="816" alt="image" src="https://github.com/user-attachments/assets/f0315376-310d-4a0c-ad89-14ed07370fb4" />

2- VA ATE OS 4 PONTOS NA PARTE SUPERIOR E CLIQUE EM "CODESPACES"

<img width="322" height="315" alt="image" src="https://github.com/user-attachments/assets/2c652e75-e380-49e3-9193-b47d394d3672" />


2-1 CLIQUE EM "NEW CODE ESPACES" E CONFIGURE O CODESPACES ASSIM:

<img width="954" height="552" alt="image" src="https://github.com/user-attachments/assets/d7f86174-0bf6-4690-8072-e6e5da64af3e" />

2.2-DEPOIS CLIQUE EM "CREATE CODESPACES"

3- APÓS O CODSPACES CARREGAR VOCE VAI VER ESSA TELA:

<img width="1919" height="922" alt="image" src="https://github.com/user-attachments/assets/887fdccf-48be-44d4-ab1a-cdf3ccc42d6a" />


# CONFIGURAÇÃO DO SOUNDNESS LAYER:

OBS: COLE CODIGO POR CODIGO - SEMPRE QUE UM ACABAR DE INSTALAR/EXECUTAR COLE OUTRO

VISUALIZE O TERMINAL:

<img width="1444" height="301" alt="image" src="https://github.com/user-attachments/assets/6b07b29b-bf96-4c61-bc42-6702b5059706" />

DIGITE OS SEGUINTES COMANDOS:

1-
```bash
sudo apt update && sudo apt upgrade -y
```

2-

```bash
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```

3-

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
```

4-

```bash
source ~/.bashrc
```

5-

```bash
soundnessup install
```

6-

```bash
soundnessup update
```

# CARREGAR A FRASE SECRETA (Mnemonic)


```bash
soundness-cli import-key --name my-key --mnemonic "SUA FRASE SECRETA AQUI"
```

OBS: 

1- EM --name my-key utilize o nome da sua key que vc salvou, caso nao tenha salvado o nome utilize my-key
2 - se ocorrer tudo certo ao fazer o upload da key, vai pedir a senha é so por a mesma senha 2x
3- vale lembrar que sua frase secreta tem entre 12/16/18/24 palavras e voce vai colar entre as aspas onde esta escrito "SUA FRASE SECRETA AQUI"


# RODANDO O PROOF

OBS:
***** PRA QUEM FEZ O GAME, FEZ O PROOF DO GAME E RECEBEU A MENSAGEM DO BOT TIPO ESSA:

<img width="541" height="710" alt="image" src="https://github.com/user-attachments/assets/6aa2e2c7-e0f3-44fb-9994-158754de5422" />

1 - É SÓ COPIAR O CODIGO E ALTERAR ONDE ESTA ESCRITO <your-key-name> POR my-key FICANDO ASSIM:

<img width="1449" height="231" alt="image" src="https://github.com/user-attachments/assets/399c7cd8-56b4-4d36-9a6b-23fb12827597" />

2- APOS ALTERAR O NOME DA KEY, COLE O CODIGO NO TERMINAL E DE ENTER, VAI CARREGAR A API DA WALRUS E DA SUI E VAI PEDIR A SENHA QUE VOCE COLOCOU NOS PASSOS ANTERIORES
COLOQUE A SENHA E DE ENTER, SE TUDO OCORRER CERTO VAI APRESENTAR O SEGUINTE RETORNO:

<img width="750" height="264" alt="image" src="https://github.com/user-attachments/assets/455aea47-9ede-4393-8240-637ae557a93e" />

3- APOS APRESENTAR ESSE RETORNO SEU PROOF JA ESTA FEITO.








