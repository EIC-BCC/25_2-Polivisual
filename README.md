# 25_2-Polivisual

**Título do TCC: POLIVISUAL: UM ESTUDO SOBRE A IMPLEMENTAÇÃO
DA REALIDADE AUMENTADA NAS SALAS DE AULA
BRASILEIRAS SOB UMA ÓTICA DOCENTE** 

**Alunos: Thales Maia Barreto**

**Semestre de Defesa: 2025-2**

[PDF do TCC](./TCC_2.pdf)

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
<!-- Descreva nessa seção a arquitetura do seu código. Sugestão: use mermaid para inclusão de diagramas que ajudem a entender seu código (https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-… -->

```mermaid
usecaseDiagram
    actor "Usuário" as user

    usecase UC1 as "Escolher poliedro"
    usecase UC2 as "Escolher realce"
    usecase UC3 as "Começar RA"
    usecase UC4 as "Mostrar na tela poliedro\ncom realce"

    user --> UC1
    UC1 ..> UC2 : <<include>>
    UC2 ..> UC3 : <<include>>
    UC4 ..> UC3 : <<extend>>
```

# Dependências
* Node.js

# Execução
* Instale as dependências do projeto: `npm install`
* Rode localmente: `npm run dev -- --host`
