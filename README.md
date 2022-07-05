Made in **22/01/2022**.

## In this assignment we learned how to implement tests and to make functions based on tests.
#### Our learning goal was to understand how tests and Test Driven Development works.
<img src='https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg' width='40'/> <img src='https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jest/jest-plain.svg' width='40'/>

#### Here is a code snippet:
 ````javascript
 describe('4 - Implemente os casos de teste para a função `circle`', () => {
  it('Verifica se ao receber um raio, a função `circle` retorna um objeto contedos os valores esperados', () => {
    // fail('Teste vazio!');
    // ESCREVA SEUS TESTES ABAIXO:
    expect(circle(NaN)).toBeUndefined();
    // Teste se circle retorna undefined, caso o parâmetro passado não seja um número.
    // não tô conseguindo pegar o objeto que a função retorna
    expect(typeof circle(7)).toEqual('object');
    // Teste se circle retorna um objeto.
    expect(Object.keys(circle(7)).length).toEqual(3);
    // Teste se o objeto retornado tem 3 propriedades.
    expect(circle()).toEqual(undefined);
    // Teste se a função, quando não recebe nenhum parâmetro, retorna undefined.
    expect(circle(2).circumference).toBe(12.56);
    // Teste que a função retorna, dentro de um objeto, a circunferência correta para um círculo de raio 2.
    expect(circle(3).area).toBe(28.259999999999998);
    // Teste que a função retorna, dentro de um objeto, a área correta para um círculo de raio 3.
    expect(circle(3)).toEqual({ radius: 3, area: 28.259999999999998, circumference: 18.84 });
    // Teste que a função retorna, num objeto, os dados corretos de um círculo de raio 3.
  });
});
````

#### Trybe has a private repository with files that can't be shared. So here is my commit history print:
<img src='images-readme/commit-history.png'>

#### Here is the Trybe Evaluator
<img src='images-readme/evaluator.png'>
