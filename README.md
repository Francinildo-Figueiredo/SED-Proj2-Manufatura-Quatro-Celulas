# Modelagem de um sistema de manufatura com quatro células

## Descrição geral 

Uma célula de manufatura possui um depósito de entrada, um depósito de saída, 
três máquinas e três robôs. Cada uma das máquinas possui um depósito de 
entrada e um depósito de saída. Os robôs são responsáveis por movem itens entre 
os diversos depósitos conforme a figura abaixo. 

<p align="center">
  <img src="./img/celula.png" alt="Autômato de R1"/>
</p>

Na célula existem duas rotas de produção: 𝑖𝑖 e 𝑗𝑗. O robô 1 transporta itens entre o 
depósito de entrada da célula para o depósito de entrada da máquina 1. O robô 2 
transporta itens do depósito de saída da máquina 1 para os depósitos de entrada 
das máquinas 2 e 3. Por fim, o robô 3 transporta itens dos depósitos de saída das 
máquinas 2 e 3 para o depósito de saída da célula de manufatura. 

Foi desenvolvido um modelo de Redes de Petri Coloridas usando o CPN 
Tools para um sistema de manufatura com quatro células desse tipo. 
Os depósitos de cada máquina devem armazenar no máximo 4 itens. Garanta que 
seu modelo não possui bloqueios.

### Lugares
- *De. Ent. Célula*: Depósito de entrada da célular;
- *Dep. Ent. Mx*: Depósito de entrada da máquina x;
- *Buffer Ent. Mx*: Buffer que limita a quantidade de itens armazenados na entrada máquina Mx;
- *Dep. Saida Mx*: Depósito de saída da máquina x;
- *Buffer Saida Mx*: Buffer que limita a quantidade de itens armazenados na entrada máquina Mx;
- *Dep. Saida Celula*: Depósito de saída da célula.

### Transições
- *Robo1*: Pega o produto do depósito de entrada da célula e entrega no depósito de entrada da máquina 1;
- *Robo2i*: Pega o produto no depósito de saída da máquina 1 e leva para a máquina 2 pela rota i;
- *Robo2j*: Pega o produto no depósito de saída da máquina 1 e leva para a máquina 3 pela rota j;
- *Robo3i*: Pega o produto no depósito de saída da máquina 2 e leva para o depósito de saída da céllula pela rota i;
- *Robo3j*: Pega o produto no depósito de saída da máquina 3 e leva para o depósito de saída da céllula pela rota j;
- *Prduçãox*: Pega o produto do depósito de entrada da máquina x e leva para o depósito de saída da máquina x;

<p align="center">
  <img src="./img/rede_de_petri.png" alt="Autômato de R1"/>
</p>

<p align="center">
  <img src="./img/parte1.png" alt="Autômato de R1"/>
</p>

<p align="center">
  <img src="./img/parte2.png" alt="Autômato de R1"/>
</p>
