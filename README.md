# Camada Física

### Nessa instrução, você verá conceitos e boas práticas da CAMADA 1 - FÍSICA.


## (1) Topologias de Rede

Topologia de Rede é a maneira como os elementos de uma rede estão organizados e interligados. Ela pode ser classificada em duas categorias: **topologia física** e **topologia lógica**. 

### (1.1) Topologia Física

A **topologia física** se refere à disposição real e física dos cabos, dispositivos e outros componentes da rede. É a maneira como os cabos e equipamentos, como switches e roteadores, estão fisicamente conectados uns aos outros. Os hosts podem ser organizados em algum tipo de topologia a seguir:

<picture>
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/agodoi/SubRedes/blob/main/imgs/network-topology.png">
   <img alt="Topologias de Redes" src="[YOUR-DEFAULT-IMAGE](https://github.com/agodoi/SubRedes/blob/main/imgs/network-topology.png)">
</picture>

Para o padrão Ethernet, adota-se **Estrela** que também pode ser estendido para **Estrela Estendida** quando uma estrela dá origem para outra estrela.

<picture>
   <source media="(prefers-color-scheme: light)" srcset="https://github.com/agodoi/SubRedes/blob/main/imgs/estrela_extendida.png">
   <img alt="Estrela Estendida" src="[YOUR-DEFAULT-IMAGE](https://github.com/agodoi/SubRedes/blob/main/imgs/estrela_extendida.png)">
</picture>

### (1.2) Topologia Lógica

A **topologia lógica** descreve como os dados se movem dentro da rede, ou seja, o caminho que as informações seguem independentemente da disposição física dos cabos e dispositivos. O fluxo de dados entre os dispositivos, que nem sempre segue a topologia física. Por exemplo, em uma rede fisicamente em estrela, os dados podem se comportar como se estivessem em uma topologia em barramento, dependendo de como os pacotes de dados são transmitidos entre os dispositivos.

---

## (2) Tipos de Meios de Transmissão

   Os meios de transmissão são os canais pelos quais os dados se movem de um dispositivo para outro em uma rede. Eles podem ser classificados em três grandes categorias: par metálico, óptico e eletromagnético. Cada um desses meios tem características próprias que influenciam sua velocidade, capacidade e alcance.

### (2.1) Par metálico

   O **par metálico** é um dos meios mais comuns e tradicionais usados para transmissão de dados, especialmente em redes locais e de telefonia. Ele utiliza cabos de cobre ou outro material metálico condutor para transmitir sinais elétricos. Existem dois tipos principais:

* Cabo coaxial: um condutor central de cobre cercado por uma malha metálica, usado principalmente em TV a cabo e redes antigas de dados.
* Cabo de par trançado (UTP/STP): 8 fios de cobre trançados entre si, que ajudam a reduzir interferências eletromagnéticas. Esse é o tipo mais comum em redes de computadores, especialmente em conexões Ethernet.
* Vantagens: baixo custo, facilidade de instalação e flexibilidade.
* Desvantagens: menor alcance e susceptibilidade a interferências em comparação com outros meios.

### (2.4) Óptico

   O meio óptico utiliza fibras ópticas feitas de vidro ou plástico para transmitir dados por meio de pulsos de luz, em vez de sinais elétricos. A fibra óptica é capaz de transportar grandes quantidades de dados a altas velocidades por longas distâncias com mínima perda de sinal.

* Fibra monomodo: Ideal para transmissões de longa distância, geralmente em WANs, devido à baixa atenuação e alta capacidade.
* Fibra multimodo: Usada em curtas distâncias, como dentro de prédios ou campus, oferecendo também alta capacidade, mas com mais perda de sinal.
* Vantagens: Alta velocidade, grande capacidade de dados e imunidade a interferências eletromagnéticas.
* Desvantagens: custo mais alto e maior complexidade de instalação e manutenção.

### (2.5) Eletromagnético

   O meio eletromagnético envolve a transmissão de dados por ondas de rádio, micro-ondas, ou infravermelho através do ar, sem a necessidade de cabos físicos. Esse tipo de transmissão é amplamente utilizado em redes sem fio (wireless).

* Ondas de rádio: usadas em redes Wi-Fi, comunicações de satélite e redes de longa distância (LTE/5G).
* Micro-ondas: usadas para transmissões de longa distância em linhas de visão direta, como em comunicações entre torres de transmissão.
* Infravermelho: Utilizado em comunicações de curta distância, como controles remotos ou em alguns dispositivos IoT.
* Vantagens: flexibilidade e mobilidade, já que não depende de cabos.
* Desvantagens: susceptibilidade a interferências, obstáculos físicos e limitações de alcance e largura de banda.

---

## (3) Boas Práticas para Crimpagem do cabo UTP e Teste

Crimpar um cabo UTP (Unshielded Twisted Pair) Cat 5 exige atenção a alguns detalhes para garantir uma conexão eficiente e estável, livre de problemas, engenharia social e consequentemente, ataques. Sua missão é crimpar um cabo UTP CAT 5 com um conector RJ45 em cada ponta e passar no teste de condutividade. Usar o padrão 568A nas duas pontas. Você também pode optar pelo 568B nas duas pontas. Aqui estão as boas práticas para esse processo:

**a)** Escolha do Cabo e Conectores Corretos
   - Verifique se o cabo é compatível com o padrão Cat 5.
   - Utilize conectores RJ-45 adequados para cabos Cat 5 (ou Cat 5e).
   
**b)** Corte Limpo do Cabo
   - Utilize uma ferramenta de corte para garantir que o cabo seja cortado de forma reta e precisa, evitando fios desalinhados que podem dificultar a conexão.

**c)** Desencape o Cabo Com Cuidado
   - Ao remover a capa externa do cabo, deixe expostos cerca de 2,5 cm (1 polegada) dos pares trançados internos.
   - Não desencape, ou corte ou danifique os fios internos no momento de desencapar a capa externa.

**d)** Desenrolar e Organizar as Vias Internas
   - Separe os pares de fios e os alinhe de acordo com o padrão escolhido (T568A ou T568B).
   - Certifique-se de que os fios estão alinhados e retos antes de inserir no conector.
   - Não desenrole demais os fios; mantenha a torção o mais próximo possível do conector, pois isso ajuda a minimizar interferências.

**e)** Escolha do Padrão Correto
   - Decida entre o padrão **T568A** ou **T568B** e certifique-se de seguir o mesmo padrão em ambas as extremidades do cabo, especialmente se estiver fazendo um cabo patch.
   - As combinações de cores para o padrão T568A são:
     - pino (1) Verde/Branco
     - pino (2) Verde
     - pino (3) Laranja/Branco
     - pino (4) Azul
     - pino (5) Azul/Branco
     - pino (6) Laranja
     - pino (7) Marrom/Branco
     - pino (8) Marrom
   - Para o padrão T568B (mais usado em redes residenciais):
     - pino (1) Laranja/Branco
     - pino (2) Laranja
     - pino (3) Verde/Branco
     - pino (4) Azul
     - pino (5) Azul/Branco
     - pino (6) Verde
     - pino (7) Marrom/Branco
     - pino (8) Marrom

#### Atenção: 

* Cabo Direto: sempre use cabo direto (568A - 568A ou 568B - 568B) quando estiver conectando dispositivos diferentes entre si.

* Cabo Cruzado: sempre use cabo cruzado (568A - 568B) quando estive conentando o mesmo tipo de equipamento.

* Sempre usamos as portas **Fast Ethernet** para conexão do RJ45 + cabo UTP de PC e **Giga Ethernet** para Switches e Roteadores.


**f)** Inserção Correta dos Fios no Conector
   - Certifique-se de que os fios estão perfeitamente alinhados e nivelados antes de inserir no conector RJ-45.
   - Pressione firmemente os fios dentro do conector até que cada um toque seu respectivo pino de metal.
   - O cabo externo (capa) deve estar preso dentro do conector para maior resistência e durabilidade.

**g)** Uso da Ferramenta de Crimpagem
   - Posicione o conector no alicate de crimpagem e aperte firmemente para fixar os contatos metálicos nos fios.
   - Certifique-se de que o conector está totalmente inserido no alicate antes de crimpar para evitar crimpar mal e danificar o conector.

**h)** Teste o Cabo
   - Após crimpar, utilize um **testador de cabos** para garantir que todos os fios estão corretamente conectados e o cabo está funcionando corretamente.
   - Verifique se todos os pares estão funcionando e se não há fios cruzados ou mal conectados.

---

## (4) Roteiro Prático

#### (4.1) Formem duplas de dois :)

#### (4.1) Pegue um lance de cabo UTP disponível com o professor. Cada aluno fará uma ponta do mesmo cabo;
Atenção: as ferramentas terão que ser compartilhadas.

#### (4.2) Usando o estilete ou decapador de cabo, remova o equivalente a 2 dedos de capa azul, sem ferir as vias internas;

#### (4.3) Desembaresse as 8 vias, deixando-as bem retas;

#### (4.4) Coloque as vias na ordem correta

   - pino (1) Verde/Branco
   - pino (2) Verde
   - pino (3) Laranja/Branco
   - pino (4) Azul
   - pino (5) Azul/Branco
   - pino (6) Laranja
   - pino (7) Marrom/Branco
   - pino (8) Marrom

#### (4.5) Sem soltar a organização das vias, apare as pontas das vias por igual de modo que sobre 1,5 dedo de comprimento;

#### (4.6) Sem soltar a organização das vias, insira-as no RJ45 e na ordem certa: pino 1 com Verde/Branco e certifique-se que todas as 8 vias estão no encostando no fundo do conector, onde há os garfinhos de cobre;

#### (4.7) Segurando o cabo dentro do conector, pegue o alicate, encaixe o conector no espaço e esmague o conector com a força do ódio

#### (4.8) Solte o conector do alicate e aguarde a outra ponta ficar pronta para seguir;

#### (4.9) Pegue o testador de cabo, conecte qualquer ponta nos encaixes e ligue-o. Os LEDS precisam piscar um ao lado do outro sincronizadamente. Se isso aconteceu, SUCESSO!

#### (4.10) Caso algum LED tenha falhado, faça: esmague novamente os 2 conectores e teste novamente;

#### (4.11) Caso ainda assim algum LED tenha falhado, senta e chora. Vai ter que refazer uma das pontas. Mas antes, faça uma inspeção visual e tente encontrar qual ponta tem maior probabilidade de estar errada, com cor de via invertida ou que não esteja em contato com o garfinho de cobre. Volte na etapa (4.2)
