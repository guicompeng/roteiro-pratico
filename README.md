# Grupo 9 - Laboratório de Engenharia de Software I

## Desenvolvimento Mobile com Kotlin e Android

## Integrantes

- 20213002091 - DIOGO EMANUEL ANTUNES SANTOS
- 20203005008 - FELIPE SILVA FARIA
- 20203020283 - GUILHERME DE ASSIS LIMA
- 20213004828 - PEDRO HENRIQUE ROCHA DE CASTRO

Clique em start
 <p align="center">
    <img width="25%" src="/prints/start.png">
 </p>

 Apos iniciar o projeto, deverá ser mostrado nossa calculadora:
  <p align="center">
    <img width="25%" src="/prints/semBotaoLimpar.png">
 </p>

 Essa calculadora não permite limpar o resultado. Vamos adicionar essa funcionalidade!


Criando um botão para limpar:
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
