# 25_2-Polivisual

**Título do TCC: POLIVISUAL: UM ESTUDO SOBRE A IMPLEMENTAÇÃO
DA REALIDADE AUMENTADA NAS SALAS DE AULA
BRASILEIRAS SOB UMA ÓTICA DOCENTE** 

**Alunos: Thales Maia Barreto**

**Semestre de Defesa: 2025-2**

[PDF do TCC](./TCC-2.pdf)

# TL;DR
Para testar o Polivisual, você precisa ter o Node.js instalado em sua máquina. Caso já tenha, instale as dependências do projeto com o comando `npm install` e depois rode localmente com `npm run dev -- --host`.

Utilize o endereço de rede (exibido no terminal após executar o comando para rodar o projeto localmente) no seu navegador no celular. Certifique-se de que ambos os aparelhos estejam conectados na mesma rede.

# Descrição Geral
O avanço contínuo da tecnologia tem causado profundas transformações na sociedade, in-
cluindo o surgimento da Realidade Aumentada. No contexto educacional, essa tecnologia
pode ser explorada de forma benéfica, especialmente nas escolas, por meio de dispositivos
móveis. As instituições de ensino desempenham papel fundamental na formação dos jo-
vens, e o uso adequado da tecnologia pode contribuir significativamente para a melhoria
da qualidade do ensino. Nesse sentido, este trabalho apresenta a percepção de professores
de diferentes regiões do Brasil sobre os desafios de implementação e os possíveis benefícios
pedagógicas da integração da Realidade Aumentada no ensino, e propõe uma aplicação
web utilizando tal tecnologia, denominada Polivisual, voltada ao ensino de poliedros para
alunos do ensino fundamental por meio de smartphones. Os resultados da Avaliação Expe-
rimental revelam um consenso entre os docentes quanto ao impacto positivo da ferramenta
para o aluno, destacando seu potencial para promover o engajamento e tornar o ambiente
de sala de aula mais colaborativo, consequentemente, melhorando a qualidade de ensino.

# Funcionalidades
* Escolha de poliedros: cubo, tetraedo e tronco.
* Escolha de realce: vértice, aresta e face.
* Visualização em 3D em Realidade Aumentada das suas escolhas.

# Arquitetura

```mermaid
graph TB
    User([Usuário])
    
    UC1[Escolher poliedro]
    UC2[Escolher realce]
    UC3[Começar RA]
    UC4[Mostrar na tela poliedro<br/>com realce]
    
    User --> UC1
    UC1 -.->|include| UC2
    UC2 -.->|include| UC3
    UC4 -.->|extend| UC3
    
    style User fill:#e1f5ff,stroke:#333,stroke-width:2px
    style UC1 fill:#fff4e6,stroke:#333,stroke-width:2px
    style UC2 fill:#fff4e6,stroke:#333,stroke-width:2px
    style UC3 fill:#fff4e6,stroke:#333,stroke-width:2px
    style UC4 fill:#fff4e6,stroke:#333,stroke-width:2px
```

# Dependências
* Node.js

# Execução
* Instale as dependências do projeto: `npm install`
* Rode localmente: `npm run dev -- --host`
