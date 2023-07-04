<h1 align="center">
  <strong>CSS Standards</strong> 
</h1>

## **CSS do Bem**

A organização do CSS é fundamental para manter seu código limpo, legível e fácil de dar manutenção. Um padrão popular de organização é o CSS do BEM (Block Element Modifier).
</br>

O CSS do BEM é uma metodologia de nomenclatura de classes que visa fornecer uma estrutura clara e consistente para o desenvolvimento de estilos. Ele divide o código CSS em três partes principais: Blocos (Blocks), Elementos (Elements) e Modificadores (Modifiers).
</br>

## **1- Blocos**
    
Blocos (Blocks): Os blocos são componentes independentes e reutilizáveis do seu site ou aplicativo. Eles devem ser autossuficientes e não depender de outros elementos. Para nomear as classes de blocos, use um prefixo único relacionado ao componente, como .button, .card, .header.

</br>

## **2- Elementos**

Elementos (Elements): Os elementos são partes dos blocos e têm significado somente no contexto do bloco em que estão. Eles são denotados adicionando um sublinhado duplo (__) ao nome do bloco, seguido pelo nome do elemento. Por exemplo, .button__icon, .card__title, .header__logo.

</br>

## **3- Modificadores** 

Modificadores (Modifiers): Os modificadores são usados para alterar o estilo ou comportamento de um bloco ou elemento. Eles permitem criar variações do componente sem precisar duplicar o código. Os modificadores são denotados adicionando um traço (--) ao nome do bloco ou elemento, seguido pelo nome do modificador. Por exemplo, .button--large, .card__title--highlighted, .header__logo--dark.
</br>

A estrutura de classes do BEM fica assim:

````
<div class="block">
  <div class="block__element"></div>
  <div class="block__element block__element--modifier"></div>
</div>
````

Ao seguir o CSS do BEM, você ganha os seguintes benefícios:
</br>

- Clareza e consistência na nomenclatura das classes.
- Componentes reutilizáveis e independentes.
- Baixo acoplamento entre elementos.
- Fácil localização e compreensão do código CSS.

</br>

## **Agrupamento lógico**

O agrupamento lógico no CSS refere-se à prática de agrupar seletores CSS relacionados ou que compartilham propriedades semelhantes. É uma técnica de organização que visa melhorar a legibilidade, manutenção e eficiência do código CSS
</br>

Ao agrupar seletores logicamente, você reúne regras de estilo relacionadas em um único bloco, tornando mais fácil entender e modificar o código. Isso é especialmente útil quando várias partes do seu site ou aplicativo têm estilos semelhantes ou compartilham propriedades comuns.

Um exemplo de agrupamento lógico:

```css
.seletor {
    [posicionamento]
    [tamanho]
    [bordas]
    [espaçamentos]
    [plano de fundo]
    [fonte e propriedades de texto]
}
```

Este é o método que considero mais produtivo e que utilizo nos meus projetos.

</br>

Aqui está um exemplo mias pratico e real do agrupamento:

```css
.foo {
  display:flex;
  flex-direction: column;
  justify-content: center;
  
  width: 200px;
  height: 100%;
  
  border-radius: 3px;
  border: 1px solid #000;
  
  margin: 20px 10px;
  padding: 8px;
  
  background-image: url('../assets/bg.png');
  background-position: center center;
  
  font-family: 'Roboto', sans-serif;
  font-size: 20px;
  font-weight: bold;
}
```
Com técnicas simples como essa, os seletores se tornam muito mais legíveis e fáceis de manter. Isso permite que o CSS seja mais funcional, semântico e compreensível, mantendo a flexibilidade do código como um aspecto importante.