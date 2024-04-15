# Projeto Final de Reinforcement Learning

## Integrantes do grupo:
- [Davi Reis Vieira](https://github.com/DaviReisVieira)
- [Henrique Matinelli Frezzatti](https://github.com/henriquemf)
- [Luiza Valezim](https://github.com/LuizaValezim)
- [Nicolas Maciel Queiroga](https://github.com/NicolasQueiroga)

## Objetivo do projeto
O objetivo desse projeto se baseia na utilização dos aprendizados obtidos durante o curso de Reinforcement Learning envolvendo o conhecimento de algoritmos que utilizam uma Q-Table para um ambiente denominado CyberBattleSim, explorando estratégias de aprendizado por reforço para aprimorar o desempenho dos agentes (atacante e defensor) no ambiente. Isso inclui a melhoria da capacidade de detecção de ataques, a eficácia na mitigação de ameaças e a otimização das ações dos agentes para atingir seus objetivos. 

Nesse ambiente, há dois agentes que poderão ser utilizados em uma rede extensa e complexa de computadores: atacante e defensor. Cada agente possui um determinado `action space` e um `observation space`.

## Sobre o ambiente
- Em primeiro lugar, o ambiente de simulação é definido por uma topologia de rede fixa e um conjunto de vulnerabilidades que os agentes podem usar para se mover lateralmente na rede. O objetivo do atacante é tomar controle de uma parte da rede explorando vulnerabilidades implantadas nos nós dos computadores. Enquanto o atacante tenta se espalhar pela rede, um agente defensor observa a atividade da rede e tenta detectar qualquer ataque em andamento e mitigar o impacto no sistema expulsando o atacante.
- Para implementar a mitigação, há uma reconfiguração dos nós infectados, um processo modelado abstratamente como uma operação que se estende por vários passos de simulação.
- Para comparar o desempenho dos agentes, observamos duas métricas: o número de `steps` de simulação necessários para atingir seu objetivo e as `rewards` cumulativas ao longo dos passos de simulação em diferentes fases de treinamento com seus respectivos números de episódios.

## Método
- **Definição do ambiente:** Estabelecer os parâmetros do ambiente de simulação, incluindo a topologia da rede, as vulnerabilidades dos nós e os recursos disponíveis para os agentes, tudo isso dentro do ambiente escolhido `CyberBattleSim`
- **Formulação do problema:** Especificar os objetivos dos agentes (atacante e defensor) e a função de recompensa que guiará o aprendizado.
- **Escolha do algoritmo de aprendizado por reforço:** Iremos testar e treinar utilizando algoritmos utilizados no projeto intermediário da disciplina, sendo estes o DQN e DDQN.
- **Treinamento dos agentes:** Treinar os agentes, permitindo que aprendam e ajustem suas estratégias com base nas interações com o ambiente.
- **Avaliação do desempenho:** Avaliar o desempenho dos agentes com base em métricas como o número de `steps` de simulação para atingir seus objetivos, a eficácia na detecção e mitigação de ataques, e a estabilidade do sistema em face de diferentes cenários de ameaça.

## Resultados esperados
É esperado nesse projeto uma análise mais aprofundada sobre o ambiente e um treinamento que resulte em agentes de ataque e defesa mais eficientes e adaptáveis, capazes de lidar com uma variedade de cenários de ameaça no ambiente CyberBattleSim. Isso pode incluir uma redução no tempo necessário para alcançar os objetivos, uma melhoria na detecção e resposta a ataques e uma maior resiliência do sistema em face de ameaças emergentes. 

Além disso, espera-se um avanço nos conhecimentos de cibersegurança pelos integrantes do projeto e que esse projeto sirva como base para diversas ramificações possíveis envolvendo esse tema. 

## Referências bibliográficas para o projeto:
1. Múltiplos autores. **Bridging Automated to Autonomous Cyber Defense: Foundational Analysis of Tabular Q-Learning**. Publicado em: 11 de novembro de 2022. Disponível em: https://dl.acm.org/doi/pdf/10.1145/3560830.3563732
2. Múltiplos autores. **CyberBattleSim**. Publicado em: 8 de abril de 2021. Disponível em: https://github.com/microsoft/CyberBattleSim
3. Múltiplos autores. **Employing Deep Reinforcement Learning to Cyber-Attack Simulation for Enhancing Cybersecurity**. Publicado em: 30 de janeiro de 2024. Disponível em: https://www.mdpi.com/2079-9292/13/3/555
4. Múltiplos autores. **A Multiagent CyberBattleSim for RL Cyber Operation Agents**. Publicado em: abril de 2023. Disponível em: https://www.researchgate.net/publication/370213244_A_Multiagent_CyberBattleSim_for_RL_Cyber_Operation_Agents
