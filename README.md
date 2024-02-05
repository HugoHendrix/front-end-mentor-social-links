# Frontend Mentor - Solução do perfil de links sociais

Esta é uma solução para o [Desafio do perfil de links sociais no Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Os desafios do Frontend Mentor ajudam você a aprimorar suas habilidades de codificação, construindo projetos realistas.

## Sumário

- [Visão Geral](#visão-geral)
  - [O desafio](#o-desafio)
  - [Captura de Tela](#captura-de-tela)
  - [Links](#links)
- [Meu Processo](#meu-processo)
  - [Desenvolvido com](#desenvolvido-com)
  - [O que Aprendi](#o-que-aprendi)
  - [Desenvolvimento Contínuo](#desenvolvimento-contínuo)
  - [Recursos Úteis](#recursos-úteis)
- [Autor](#autor)
- [Agradecimentos](#agradecimentos)



## Visão Geral

### O desafio

Os usuários devem ser capazes de:

- Ver estados de hover e foco para todos os elementos interativos na página.

### Captura de Tela

![App Screenshot](https://github.com/HugoHendrix/front-end-mentor-social-links/blob/main/design/solution-frontend-Mentor-social-links-profile.png?raw=true)


## Links

- URL da Solução: [FrontEnd Mentor](https://hugohendrix.github.io/front-end-mentor-social-links/)


## Meu Processo

### Desenvolvido com

- Marcação HTML5 semântica
- Propriedades personalizadas CSS
- Bootstrap
- Fluxo de trabalho "mobile-first"



### O que Aprendi

Aprendi a melhorar a experiência do usuário ao interagir com a minha página, principalmente focando em acessibilidade e usabilidade. Aqui estão alguns conceitos e práticas:

- **Foco e Hover:** Compreendi a importância de estilos para `:hover` e `:focus` para fornecer feedback visual aos usuários durante a interação.

- **Acessibilidade:** Entendi como adicionar estilos específicos para o foco (`:focus`) ajuda os usuários que navegam pelo teclado ou usam leitores de tela, proporcionando uma experiência mais inclusiva.

- **Estilização Responsiva:** Aprendi a ajustar estilos para diferentes dispositivos, como a melhoria específica para dispositivos móveis, garantindo uma experiência consistente em diversas plataformas.

- **Seleção de Elementos:**
   Conheci o seletor `:focus-within`, que permite aplicar estilos quando qualquer elemento filho de um contêiner é focado. Isso é útil para destacar um contêiner inteiro quando qualquer parte dele é interativa.

- **Remoção de Estilos Padrões:** Aprendi a remover estilos padrões do navegador, como a borda ao focar em links, proporcionando uma aparência mais personalizada e consistente.

Essas práticas são essenciais para criar interfaces web atraentes, funcionais e acessíveis. 


```css
/* Adiciona um estilo para o foco nos links */
ul li a:focus {
  outline: none; /* Remove a borda padrão do navegador */
  box-shadow: 0 0 0 3px var(--Blue-Hendrix); /* Adiciona uma borda ao redor do link ao focar */
}

/* Melhora a experiência de foco em dispositivos móveis */
ul li a:focus:not(:hover) {
  color: var(--Off-Black);
  background-color: var(--Blue-Hendrix);
}

/* Adiciona um estilo para o foco nos itens da lista */
ul li:focus-within {
  background-color: var(--Blue-Hendrix);
  color: var(--Gray);
}

/* Adiciona um estilo para o foco nos itens da lista e seus links */
ul li:focus-within a {
  color: var(--Gray);
}

/* Remove a borda padrão do botão do Bootstrap quando focado */
.btn:focus {
  outline: none;
  box-shadow: none;
}

```

## Desenvolvimento Contínuo

- Aprender mais sobre as classes do Bootstrap.
- Aprofundar o entendimento em:
  - Reaproveitamento e refatoração.
  - Responsividade.
  - BEM (Block Element Modifier).
  - Acessibilidade.

### Recursos Úteis

- [Bootstrap Cheat Sheet](https://bootstrap-cheatsheet.themeselection.com/) - Uma folha de referência rápida para as classes do Bootstrap. Útil para explorar e entender as possibilidades oferecidas pelo framework.
- [Maujor](https://www.maujor.com/) - Site do senhor Maurício Samy Silva, que fornece valiosos recursos e conhecimentos sobre desenvolvimento web.

## Autor

- Frontend Mentor - [@HugoHendrix](https://www.frontendmentor.io/profile/HugoHendrix)
- Linkedin - [Hugo Hendrix](https://www.linkedin.com/in/hugohendrix/)


