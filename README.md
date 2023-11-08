# Grupo 9 - Laboratório de Engenharia de Software I

## Desenvolvimento Mobile com Kotlin e Android

## Integrantes

- 20213002091 - DIOGO EMANUEL ANTUNES SANTOS
- 20203005008 - FELIPE SILVA FARIA
- 20203020283 - GUILHERME DE ASSIS LIMA
- 20213004828 - PEDRO HENRIQUE ROCHA DE CASTRO


## Instalação do projeto Calculadora
Antes de tudo, a instalação do Android Studio é um requisito fundamental. Certifique-se de instalar a versão mais recente.

Para configurar o ambiente, siga as etapas detalhadas no link a seguir, de acordo com o seu sistema operacional:
https://developer.android.com/studio/install?hl=pt-br

Uma vez que o Android Studio esteja instalado, siga as instruções abaixo:

1. Realize um fork do repositório clicando no ícone Fork localizado no canto superior direito da página.

2. No terminal, efetue o clone do projeto através do comando a seguir:

```
git clone https://github.com/<SEU USUÁRIO>/roteiro-pratico.git
```

3. Inicie o Android Studio. Na tela de boas-vindas, acesse a seção Projects na barra lateral esquerda e selecione a opção Open. Procure e escolha o diretório do repositório, depois selecione a pasta App. Clique em OK para abrir o projeto.

4. Você pode optar por conectar um dispositivo físico ou usar um emulador para executar o aplicativo. Neste guia, abordaremos o uso de um emulador!
 
5. Se desejar utilizar um emulador, verifique se já possui um instalado e selecione-o na guia Device Manager. Caso não tenha um emulador instalado, acesse Device Manager na tela e clique no botão Create Device. Na janela pop-up que aparecerá, selecione o dispositivo desejado e siga as instruções para concluir a instalação. Após a instalação, selecione o dispositivo recém-criado.
        
6. Após a seleção do dispositivo desejado, clique no botão de início (representado pela cor verde) para iniciar a aplicação:
   <p align="center">
    <img width="25%" src="/prints/start.png">
 </p>

7. O resultado esperado é a criação de um aplicativo Android com a tela inicial exibida abaixo:
   
  <p align="center">
    <img width="25%" src="/prints/semBotaoLimpar.png">
 </p>

8. Explore a calculadora! Tente fazer diferentes operações.

Observe que essa calculadora não permite limpar o resultado. Vamos adicionar essa funcionalidade!


### Criando um botão para limpar o resultado
No arquivo MainActivity.kt, Adicione o código abaixo em cima da função decimalPoint (linha 34)
```
    fun onClear(view: View){
        tvInput.text= ""
        num=false
        dot=false
    }
```

  No arquivo activity_main.xml, adicione na linha 30:
```
          <Button
            android:id="@+id/btnclr"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_marginHorizontal="2dp"
            android:layout_weight="1"
            android:backgroundTint="#787878"
            android:onClick="onClear"
            android:text="C"
            android:textSize="20sp" />

```

Resultado:
  <p align="center">
    <img width="25%" src="/prints/comBotaoLimpar.png">
 </p>

 Testando multiplicação:
  <p align="center">
    <img width="25%" src="/prints/exemplo1.png">
     <img width="26%" src="/prints/exemplo2.png">
 </p>
