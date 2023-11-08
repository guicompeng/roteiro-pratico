# Grupo 9 - Laboratório de Engenharia de Software I

## Desenvolvimento Mobile com Kotlin e Android

## Integrantes

- 20213002091 - DIOGO EMANUEL ANTUNES SANTOS
- 20203005008 - FELIPE SILVA FARIA
- 20203020283 - GUILHERME DE ASSIS LIMA
- 20213004828 - PEDRO HENRIQUE ROCHA DE CASTRO


## Introdução ao Kotlin

No cenário em constante evolução do desenvolvimento de aplicativos móveis, a escolha da tecnologia certa desempenha um papel fundamental no sucesso de qualquer projeto. O Kotlin, uma linguagem de programação moderna e versátil, emergiu como uma escolha cada vez mais popular para desenvolvedores de aplicativos. Sua elegância, simplicidade e poder o tornam uma escolha excepcional para a criação de aplicativos de alta qualidade.

Este projeto tem como objetivo explorar o uso do Kotlin como linguagem de programação principal no desenvolvimento de um aplicativo móvel. Vamos examinar as inúmeras vantagens que o Kotlin oferece em relação a outras linguagens, bem como como essas vantagens impactam positivamente o processo de desenvolvimento e a qualidade do aplicativo final.

Vantagens do Kotlin no Desenvolvimento de Aplicativos

O Kotlin oferece uma série de vantagens significativas que o tornam uma escolha atraente para desenvolvedores de aplicativos:

Sintaxe Expressiva e Limpa: O Kotlin possui uma sintaxe intuitiva e legível, o que torna o código mais fácil de escrever e entender. Isso leva a um desenvolvimento mais eficiente e menos propenso a erros.

100% Interoperável com Java: O Kotlin é totalmente interoperável com Java, o que significa que os desenvolvedores podem aproveitar bibliotecas Java existentes e migrar gradualmente para o Kotlin, se desejarem. Isso simplifica a transição para desenvolvedores e projetos existentes.

Segurança e Redução de Erros: O Kotlin introduz recursos que reduzem a ocorrência de erros comuns, como nulos. O sistema de tipos robusto ajuda a evitar erros em tempo de compilação, resultando em um código mais seguro.

Recursos de Extensão: O Kotlin permite a criação de extensões de funções que simplificam a adição de novos recursos a bibliotecas e classes existentes, sem a necessidade de herança.

Concisão e Produtividade: A concisão da linguagem reduz a quantidade de código necessário para realizar tarefas comuns. Isso resulta em maior produtividade e menos código para manter.

Suporte à Programação Funcional: O Kotlin suporta programação funcional, o que torna mais fácil lidar com operações assíncronas e manipulação de coleções.

Comunidade Ativa e Suporte da Indústria: O Kotlin é apoiado pela JetBrains e possui uma comunidade ativa de desenvolvedores. É amplamente adotado pela indústria, incluindo grandes empresas de tecnologia, o que garante suporte contínuo e recursos em constante evolução.

Neste projeto, exploraremos a aplicação prática dessas vantagens do Kotlin no desenvolvimento de um aplicativo móvel. Examinaremos como o Kotlin simplifica o desenvolvimento, aumenta a segurança, melhora a produtividade e proporciona uma experiência de programação mais agradável para os desenvolvedores.

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


## Modificando o App para incluir um botão de limpar o resultado
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


## Estrutura do projeto calculadora
#### App/app/src/main/java/com/example/mycalculator/MainActivity.kt
O arquivo MainActivity.kt é um dos componentes-chave de um aplicativo Android. Ele representa a classe principal que atua como ponto de entrada para o aplicativo.
Como o App de calculadora é simples, toda a lógica das operações estão neste arquivo!

#### App/app/src/main/res/layout/activity_main.xml
O arquivo activity_main.xml é um arquivo de layout XML em um projeto Android que define a aparência e a estrutura da interface do usuário (UI) da atividade principal de um aplicativo Android. No nosso projeto de calculadora, esse arquivo é usado para descrever como a tela principal do aplicativo deve ser exibida, incluindo os elementos de interface do usuário (botões de operações, números, etc).


## Considerações e comentários
[A FAZER!!!]
