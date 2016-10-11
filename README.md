#Gerador de Funções Minipa MFG-4221

A automação é essencial para um laboratório de pesquisa e ensino. O objetivo deste trabalho é facilitar a o uso de geradores de sinais em experimentos de eletrônica, física e afins.
O gerador é fabricado pela Minipa, modelo MFG-4221, todo por comando digital e com a possibilidade de comunicação através da porta RS-232.

![Foto Gerador](https://github.com/andretec/Gerador-MFG-4221/blob/master/Photo-MFG-4221.JPG)
*Manual : 
http://www.minipa.com.br/Content/Manuais/X7Q4J1S7-MFG-4221-1103-BR.pdf*

---

Para a automação e controle de processos, uma linguagem muito utilizada em universidades, é a linguagem de programação visual [LabView](http://www.ni.com/labview/pt/).
Na figura abaixo temos as telas do painel frontal do programa teste e a foto do bloco de diagrama.
![Front Panel](https://github.com/andretec/Gerador-MFG-4221/blob/master/Front-Panel.png)
![Block Diagram](https://github.com/andretec/Gerador-MFG-4221/blob/master/Block-Diagram.png)

O programa teste é bem simples e intuitivo, possui um sub-vi de configuração da porta de comunicação (MFG-4221-Open.vi) e em seguida um sub-vi de envio dos comandos para a porta RS-232. (MFG-4221-Send-Commands.vi)

Inicialmente este sub-vi proporciona as seguintes funcionalidades :

* Canal A ou B
* Frequência da Onda
* Tipo da Onda (Senoidal, Quadrada, Triangular)
* Amplitude da Onda
* Ajuste de Offset

**detalhe do meu gerador é que só consigo ajustar o offset corretamente quando a amplitude da Onda é maior ou igual a 2.2 volts. (penso ser algum tipo de defeito)**


Para mudanças e melhorias no programa, estou disponibilizando o arquivo DDSGenerator.chm, que contém todos os comandos de configuração e controle do gerador.


