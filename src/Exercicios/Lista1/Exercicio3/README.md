# Exercício 3

## 3a)

Uma possível configuração seria guardar no VBO a posição e a cor de cada vértice do triângulo. O vértice P1 teria a cor vermelha, o P2 teria a cor verde e o P3 teria a cor azul. O VAO fica responsável por indicar qual parte desses dados representa a posição e qual parte representa a cor.

## 3b)

No vertex shader, a posição e a cor seriam identificadas separadamente. A posição poderia ser identificada como atributo 0 e a cor como atributo 1, igual a configuração feita no VAO. O shader saberia quais valores usar para posicionar cada vértice e quais valores usar como sua cor.
