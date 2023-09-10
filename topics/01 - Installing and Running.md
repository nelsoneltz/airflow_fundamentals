# 01 - Installing and Running

Para instalação eu usei o método "winget" do Windows. Os demais métodos de instalação estão [aqui](https://docs.astronomer.io/astro/cli/install-cli?tab=windows#install-the-astro-cli)

1. Com um Windows PowerShell aberto com modo admnistrador, execute o comando:

```
winget install -e --id Astronomer.Astro
```

2. Acesse a pasta com caminho "C:\Users\myname\AppData\Local\Microsoft\WinGet\Packages\"
3. Troque o nome do arquivo para "astro.exe"
4. Para teste, execute o comando abaixo no terminal:

```
astro version
```

Caso seja necessário adicionar uma variável ao Path do seu sistema, use esse [GUIA](https://www.java.com/en/download/help/path.html).

Com Astronomer CLI instalado, para criar um projeto de Airflow:

```
astro dev init
```

Para executar o projeto:

```
astro dev start
```

Caso não consiga executar o projeto devido à portas que já estão sendo utilizadas, pode-se trocar a porta com o comando:

```
astro config set webserver.port 8081
astro config set postgres.port 5435
```
