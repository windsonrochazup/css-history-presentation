---
theme: default
background: >-
  https://images.unsplash.com/photo-1517134191118-9d595e4c8c2b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## CSS history presentation
drawings:
  persist: false
---

<div
  v-if="$slidev.nav.currentPage === 1"
  v-motion
  :initial="{ opacity: 0, x: -1000 }"
  :enter="{ opacity: 1, x: 0 }">
  <h1>A (re)volução do CSS ao longo do tempo</h1>
</div>

<!--
Boa tarde pessoal, hoje vamos falar como se deu a evolução/revolução do CSS ao longo do tempo.
-->

---
theme: default
---

<div
  v-if="$slidev.nav.currentPage === 2"
  v-motion
  :initial="{ opacity: 0, x: -1000 }"
  :enter="{ opacity: 1, x: 0 }">
  <h1>Kalléo Pinheiro</h1>
  <h3>Frontend Software Engineer</h3>
</div>

<br/>
<br/>

<div class="leading-8 opacity-80">
🏠 Brasiliense, Brasília/DF<br>
⚽  Flamenguista<br>
🐕 Casado e pai da Nina<br>
🎓 Bacharel em Sistemas de Informação, 2017<br>
😍 Linux<br>
💻 JS/TS<br>
👨‍💼 Na <a href="https://zup.com.br/" target="_blank">@ZUP</a> há 3 anos<br>
</div>

<div class="my-10 grid grid-cols-[40px,1fr] w-min gap-y-4">
  <ri-github-line class="opacity-50"/>
  <div><a href="https://github.com/kalleopinheiro" target="_blank">kalleopinheiro</a></div>
  <carbon-email  class="opacity-50"/>
  <div>windson.rocha@zup.com.br</div>
</div>

<img src="https://avatars.githubusercontent.com/u/51678631?v=4" class="rounded-full w-100 abs-tr mt-16 mr-12"/>

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
      v-if="$slidev.nav.currentPage === 3"
      v-motion
      :initial="{ opacity: 0, x: -1000 }"
      :enter="{ opacity: 1, x: 0 }">
      <h1>Um pouco de história</h1>
    </div>
    <v-clicks>
      <li>A web foi criada por volta de 1991;</li>
      <li>Existia a necessidade de melhorar;</li>
      <li>Surgiu o  Cascading Style Sheets(CSS);</li>
      <li >Ainda possuía muitas limitações;</li>
      <li>Surgirão padrões comportamentais e ferramentais;</li>
    </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-60 inline-block" src="/CSS.jpg">
  </div>
</div>

<!--
  Então, vamos partir do início e falar um pouco do passado, um pouco de história…
  A internet como conhecemos hoje surgiu em 1991, o primeiro site da internet foi criado por Tim Berners-Lee durante sua participação em um projeto intitulado “The Project” quando ele atuava como físico no Centro de Europeu de Pesquisa Nuclear (CERN), o site descreve brevemente a World Wide Web(daí que vem os “www” dos sites hoje em dia) e o objetivo do Tim Berners-Lee era compartilhar códigos e procedimentos de como se fazer páginas semelhantes a essa. Acessar (http://info.cern.ch/hypertext/WWW/TheProject.html).

  A partir daí, muitos outros sites foram surgindo e isso levou a necessidade de melhorar a apresentação e formatação dessas páginas web.

  Em 1994 Håkon Wium Lie apresentou uma proposta de projeto para a World Wide Web Consortium(W3C), o Cascading Style Sheets(CSS) e somente em 1996 em parceria com a W3C foi publicado oficialmente.
  Mas ainda assim o CSS possui diversas limitações e seu uso não era muito intuitivo. Em 1998 foi lançada uma segunda versão, e sua terceira versão só veio surgir em 2012, nesse espaço tempo, foi onde a maioria dos desenvolvedores mais “antigos” sofreram bastante. Posicionar elementos em tela, adicionar bordas, opacidade, organização dos projetos, cada desenvolvedor tinha uma forma diferente de fazer as coisas.

  Por isso ainda nessa época veio a surgir algumas metodologias e ferramentas para auxiliarem na estilização do CSS.
-->

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
      v-if="$slidev.nav.currentPage === 4"
      v-motion
      :initial="{ opacity: 0, x: -1000 }"
      :enter="{ opacity: 1, x: 0 }">
      <h1>Metodologias e padrões</h1>
    </div>
    <v-clicks>
      <li>Minimizam os problemas de falta de padronização da escrita do CSS;</li>
      <li>Reduz o problema de colisão de estilos;</li>
      <li>SUITCSS, DRYCSS, SMACSS, OOCSS, RSCSS, ITCSS e BEM;</li>
      <li>Ainda assim era passível de falhas;</li>
    </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-40 inline-block" src="/bem-naming-structure.png">
  </div>
</div>

<!--
  Para resolver o problema de como padronizar a escrita do CSS, problemas de colisão de estilos entre diversas outras coisas, surgiram algumas metodologias e padrões de como escrever CSS. Algumas delas são:  SUITCSS, DRYCSS, SMACSS, OOCSS, RSCSS, ITCSS e o famoso BEM(Bloco, Elemento, Modificador) que foi o mais conhecido e utilizado. Mas essas metodologias não garantem totalmente um CSS bem escrito, dado que cabia ao desenvolvedor aplicar os conceitos relativos a cada metodologia…
-->

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
        v-if="$slidev.nav.currentPage === 5"
        v-motion
        :initial="{ opacity: 0, x: -1000 }"
        :enter="{ opacity: 1, x: 0 }">
        <h1>CSS Modules</h1>
      </div>
      <v-clicks>
        <li>Resolve o problema de colisão de estilos e escopo global do CSS;</li>
        <li>Metodologias como o BEM já não são mais necessárias;</li>
        <li>Já está presente nos pré/pós processadores do mercado e de Frameworks também;</li>
      </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-60 inline-block" src="/cssModules.png">
  </div>
</div>

<!--
  E para ajudar com esse problema surgiram ferramentas como o CSS MODULES que já é uma função agregada aos diversos pré/pós processadores do mercado. Ele resolve o problema de colisão de estilos e scopo CSS global. Basicamente ele gera “hashes” dinâmicos e aplicam nas classes CSS do projeto. Dado esse novo cenário, metodologias como o BEM, já não seriam mais necessárias na estilização de páginas Web.
-->

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
      v-if="$slidev.nav.currentPage === 6"
      v-motion
      :initial="{ opacity: 0, x: -1000 }"
      :enter="{ opacity: 1, x: 0 }">
      <h1>Pré-processadores</h1>
    </div>
    <v-clicks>
      <li>Interpretam o código e dão “super poderes” ao CSS;</li>
      <li>Permitem o uso de css em cascata, variáveis, funções e muito mais;</li>
      <li>Dão mais flexibilidade, produtividade e organização na escrita de CSS;</li>
      <li>Os mais conhecidos são: SASS, LESS e STYLUS;</li>
    </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-60 inline-block" src="/pre-processadores-css.png">
  </div>
</div>

<!--
  Seguindo na linha de evolução, temos os pré-processadores. Eles interpretam o código e dão maiores poderes ao CSS como automatizar a minificação de CSS, permitir o uso de variáveis no código(hoje também é possível com CSS nativo), condicionais, loops, herança, funções e muitas outras coisas que somente o CSS ainda não consegue fazer sozinho, resumindo, dão ao desenvolvedor uma maior produtividade, organização e rapidez em manutenção de código.

  Atualmente no mercado existem 3 ferramentas que tem se destacado, o SASS, Stylus e LESS, sendo o SASS o mais adotado entre eles pelos desenvolvedores mundo a fora.
-->

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
      v-if="$slidev.nav.currentPage === 7"
      v-motion
      :initial="{ opacity: 0, x: -1000 }"
      :enter="{ opacity: 1, x: 0 }">
      <h1>Pós-Processadores</h1>
    </div>
    <v-clicks>
      <li>Analisa o código gerado e aponta possíveis erros durante a compilação;</li>
      <li>Existem diversos plugins para personalizar seu comportamento;</li>
      <li>Modifica o código com base em melhorias a serem realizadas;</li>
      <li>O mais conhecido e utilizado é o PostCSS;</li>
    </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-40 inline-block" src="/postcss-logo.png">
  </div>
</div>

<!--
  Temos também os pós-processadores, eles tem o objetivo de ser mais rápido que os pré-processadores, e diferente dos pré-processadores, ele analisa o código CSS gerado, aponta possíveis erros durante a compilação, modificam o código com base em melhorias a serem realizadas, geralmente essas ações são personalizadas e definidas através de plugins. O pós-processador mais reconhecido no mercado atualmente é o PostCSS.
-->

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
      v-if="$slidev.nav.currentPage === 8"
      v-motion
      :initial="{ opacity: 0, x: -1000 }"
      :enter="{ opacity: 1, x: 0 }">
      <h1>Frameworks CSS</h1>
    </div>
    <v-clicks>
      <li>São componentes genéricos e reutilizáveis;</li>
      <li>Dão maior produtividade ao desenvolvedor;</li>
      <li>Poupa tempo e custo;</li>
      <li>Existem vários frameworks no mercado: Bootstrap, Materialize, Bulma, mais recentes o TailwindCSS, ChakraUI entre outros;</li>
    </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-60 inline-block" src="/frameworks.png">
  </div>
</div>

<!--
  Frameworks CSS são um conjunto de componentes genéricos que provêem uma estrutura básica de elementos reutilizáveis, sua utilização dá mais agilidade e produtividade durante o desenvolvimento, poupando tempo e custo de projeto.
-->

---
theme: default
layout: center
class: text-center
---

<div class="grid grid-cols-[2fr,2fr] gap-4">
  <div class="!all:leading-10 my-auto">
    <div
      v-if="$slidev.nav.currentPage === 9"
      v-motion
      :initial="{ opacity: 0, x: -1000 }"
      :enter="{ opacity: 1, x: 0 }">
      <h1>CSS in JS</h1>
    </div>
    <v-clicks>
      <li>É uma abordagem para gerenciar código CSS usando JavaScript;</li>
      <li>As bibliotecas CSS-in-JS nos fornecem uma nova abordagem para escrever CSS;</li>
      <li>Visam lidar com as limitações do CSS, como a falta de funcionalidade dinâmica, escopo e portabilidade;</li>
      <li>As bibliotecas mais populares são: Styled Components, Emotion, Aphrodite, Stitches, entre outros;</li>
    </v-clicks>
  </div>
  <div class="text-center pb-4 my-auto">
    <img class="h-40 inline-block" src="/styled-components.png">
  </div>
</div>

<!--
  É uma abordagem para gerenciar código CSS usando JavaScript. As bibliotecas CSS-in-JS nos fornecem uma nova abordagem para escrever CSS. Eles visam lidar com as limitações do CSS, como a falta de funcionalidade dinâmica, escopo e portabilidade.

  Atualmente as bibliotecas mais populares são: Styled Components, Emotion, Aphrodite entre outros.
-->

---
theme: default
layout: center
class: text-center
background: >-
  https://images.unsplash.com/photo-1488590528505-98d2b5aba04b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80
---

  <div
    v-if="$slidev.nav.currentPage === 10"
    v-motion
    :initial="{ opacity: 0, x: -1000 }"
    :enter="{ opacity: 1, x: 0 }">
    <h1>Talk is cheap</h1>
    <h1>show me the code</h1>
  </div>
  