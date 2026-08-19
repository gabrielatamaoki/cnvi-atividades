# Atividade Avaliativa 1, Técnicas de Virtualização em Infraestrutura de TI

**Instruções:** cada questão vale 5,0 pontos. Marque a alternativa correta com um `x` dentro do checkbox (`- [x]`) e escreva sua justificativa no campo indicado.

---

**1.** Uma empresa tem 10 servidores físicos, cada um rodando uma única aplicação e usando, em média, 15% da capacidade de CPU. A empresa quer reduzir o número de servidores físicos, os custos de energia e climatização, sem perder o isolamento entre as aplicações. Qual técnica resolve esse problema?

- [ ] a) Comprar mais servidores físicos, um para cada nova aplicação
- [X] b) Consolidar as aplicações em múltiplas VMs, rodando em um número menor de hosts físicos, usando um hipervisor
- [ ] c) Desligar permanentemente as aplicações menos usadas
- [ ] d) Substituir os servidores físicos por notebooks comuns
- [ ] e) Virtualização não permite reduzir o número de servidores físicos

**Justificativa:** A virtualização permite executar diversas máquinas virtuais em um único servidor físico, mantendo um nível de isolamento semelhante ao de servidores separados. Como os servidores utilizam, em média, apenas 15% de sua capacidade, é possível consolidá-los em uma quantidade menor de hosts. Dessa forma, a organização pode reduzir o consumo de energia, os gastos com climatização e os custos relacionados à infraestrutura, sem comprometer o isolamento necessário para o funcionamento das aplicações.

**2.** Um data center de produção precisa do máximo desempenho possível para as VMs, com isolamento forte entre elas e sem depender de um sistema operacional hospedeiro rodando por baixo do hipervisor. Qual tipo de hipervisor é o mais adequado?

- [ ] a) Tipo 2 (hosted), pois é mais simples de instalar
- [X] b) Tipo 1 (bare-metal), pois roda diretamente sobre o hardware, sem SO hospedeiro intermediário
- [ ] c) Nenhum hipervisor é necessário, pois apenas containers resolvem isso
- [ ] d) Tipo 2, porque tem sempre melhor desempenho que o Tipo 1
- [ ] e) É indiferente: os dois tipos entregam o mesmo desempenho em produção

**Justificativa:** O hipervisor Tipo 1 funciona diretamente sobre o hardware físico, não necessitando de um sistema operacional hospedeiro para sua execução. Essa característica diminui a sobrecarga do sistema e possibilita um uso mais eficiente dos recursos disponíveis, além de proporcionar um maior nível de isolamento entre as máquinas virtuais. Por isso, é amplamente indicado para ambientes de produção e data centers que necessitam de desempenho elevado, alta disponibilidade e segurança.
