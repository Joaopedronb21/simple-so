# simple-so
![image](https://github.com/Joaopedronb21/simple-so/assets/105052730/0fd9a970-e1ba-40b4-84af-52ca68429a2c)

<h2>Objetivos</h2>
Um projeto de faculdade no qual o objetivo é criar um SO simples utilizando Assembly para a matéria de Sistemas Operacionais utilizando a playlist a seguir:
https://www.youtube.com/watch?v=Jws7BHrts6g&list=PLsoiO2Be-2z8BfsSkspJfDiuKeC9-LSca&index=1
    <div align="left">
    <h2>Problemas</h2>
    *Sofri com problemas iniciais como:
       MSCOMCTL.OCX Error 
    [solucionando o problema](https://www.youtube.com/watch?v=ZSJnJULnrng)
    usar este comando como administrador no cmd (64BITS):
        <div align="left">
        cd C:\Windows\SysWOW64
        <div align="left">
    depois:
    <div align="left">
        regsvr32 mscomctl.ocx
    <div align="left">
        COMDLG32.OCX Error
    [solucionando o problema](https://www.youtube.com/watch?v=_Fpp6lYpS-U)
    <div align="left">
    regsvr32 C:\Windows\SysWOW64\comdlg32.ocx 
    se for 64 coloca esse comando no cmd e n no do cara (executar como adm)
        
<div align="left">
Recomendo utilizar VM
<div align="left">
Ferramentas utilizadas: VirtualBox; NASM; etc...
<div align="left">
Seguindo o vídeo é necessario um pendrive para rodar o SO na VM e configura-la também  
<div align="left">
<h2>Passo a Passo</h2>
após fazer os passos descritos acima siga esses passos a seguir
<h2>Passo 1</h2>
    
- use o Nasm para converter arquivos `.asm` em `.bin`
- execute o arquivo Assembler para gerar os arquivos
<h2>Passo 2</h2>

- compile os arquivos `.bin` gerados pelo Nasm no fergoraw
- após gerar o arquivo `.img`, execute o Rufus para montar do SO utilizando um pendrive
<h2>Pronto</h2>

- agora é só testar em uma VM (recomendado) ou no próprio computador físico
<h2>Implementações</h2>

- Janela Principal
- Interface gráfica simples
- Bibliotecas de leitura de disco; monitor; e window memory (elas estão localizadas no diretório `/Hardware`)
<h2>Confirando FergoRaw</h2>

- Percebe-se que todos os componentes estão no cabeçote 0, cilindro 0, o `bootloader` sempre deve estar no primeiro setor, seguido pelo arquivo `kernel` nos setores 2 e 3, e finalmente pelo `window` nos setores 4 e 5.

- "File to add to the raw image" significa os arquivos que serão adicionados no disco, `bootloader.bin`, `kernel.bin` e `window.bin`.

- Output file significa o local onde a imagem gerada será salva.
![FergoRaw](https://i.imgur.com/nPyMDgr.png)
<h2>Finalizando</h2>

![image](https://github.com/Joaopedronb21/simple-so/assets/105052730/17d7b24e-2845-436f-9c23-420c9f740087)


<h1>OBRIGADO KLEBER & KIDDEOS</h1>


