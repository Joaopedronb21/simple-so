# simple-so
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
- compile os arquivos `.bin` gerados pelo Nasm no fergoraw
- após gerar o arquivo `.img`, execute o Rufus para montar do SO utilizando um pendrive
- agora é só testar em uma VM (recomendado) ou no próprio computador físico
<h2>Implementações</h2>

- Janela Principal
- Interface gráfica simples
- Bibliotecas de leitura de disco; monitor; e window memory (elas estão localizadas no diretório `/Hardware`) 
