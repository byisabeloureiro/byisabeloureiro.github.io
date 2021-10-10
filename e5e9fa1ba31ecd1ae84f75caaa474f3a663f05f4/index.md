**Índice**
- [Páginas Criadas](#páginas-criadas)
- [Páginas Alteradas](#páginas-alteradas)
- [Tags](#tags)
  * [Administrativas](#administrativas)
  * [Outras](#outras)



### Páginas Criadas

#### Collections
Esta seccão ilustra todas as páginas custom de collections que foram criadas. 
Uma página de collection é uma página que mostra todos os produtos de uma determinada collection. 
Permite por isso definir, como se quer que essa página seja.

##### Collection Natal

Nome | Tipo | Descrição
------------ | ------------- | -------------
collection.natal.liquid | Template | Este template, está associado a todas as categorias e sub-categorias de Natal
collection-natal-template.liquid | Section | Esta seccção é em tudo igual à seccção collection-template.liquid. A única diferença é ter o side menu de natal do lado esquerdo.
snippet-sidebar-natal | Snippet | Contém o menu do lado esquerdo com as subcategorias de Natal. O menu está configurado em OnlineStore -> Nagigation (ver imagem em baixo). 


Neste imagem é possível ver como está o side-menu de natal configurado no Shopify, e o nome do handler que é usado no ficheiro snippet-sidebar-natal.liquid.
![image](https://user-images.githubusercontent.com/92253809/136710373-d4c07fdb-4c3c-4f3c-8d38-2cedcea22158.png)


#### Product
Esta seccão ilustra todas as páginas custom de product que foram criadas. 
Uma página de product é uma página os detalhes de um determinado produto com as suas opcções.
Permite por isso definir aspectos como opcções adicionais, como nomes para personalização dos produtos, entre outros.

É importante que todas as opções de um produto, que tenham influência no preço final, por exemplo ter ou não embrulho, seja configuradas, via shopify, adicionando essas opções como variantes do produto, e não via html/javascript directamente no tema.



### Páginas Alteradas
Esta secção enumera todas as páginas do tema que foram alteradas. 
Isto é importante, porque, um dia que o tema tenha algum update, seja fácil perceber que páginas foram impactadas.

Nome | Tipo | O que foi alterado
------------ | ------------- | -------------
search.liquid | Template | linha 19. De grid_results = false para grid_results = true

### Tags
#### Administrativas 
Todas as tags administrativas começam por configuration


#### Outras






```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```
