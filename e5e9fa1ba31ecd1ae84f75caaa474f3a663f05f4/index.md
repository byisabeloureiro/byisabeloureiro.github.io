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

##### Product só nome de quem recebe e nome de quem recebe
**Ficheiros**
Template: product.receives.offer.liquid
Section: product-receives-offer-template.liquid

**Baseado em..**
Template: product.liquid
Section: product-template.liquid

A diferença é a inclusão dos snippets com os nomes de quem recebe e o nome de quem oferece para serem personalizados

            {%- if product.tags contains "configurationDontShowReceivingName" -%}
                <!-- do nothing -->
            {%- else -%}
                {% include 'snippet-receiving-name' %}
            {%- endif -%}
          
            {%- if product.tags contains "configurationDontShowReceivingName" -%}
          		<!-- do nothing -->
          	{%- else -%}
          		{% include 'snippet-offering-name' %}
          	{%- endif -%}
           


**Detalhes**
Este template é útil quando, apenas existe uma opção variante seguido do nome de quem recebe e o nome de quem oferece.
Este template também serve, se os nomes a personalizar puderem aparecer no fim de todas as opções.
Outro aspecto importante deste template é a mudança de variante, faz com que a imagem mostrada, mude também.

A product-template.liquid

Exemplo de página
![image](https://user-images.githubusercontent.com/92253809/136712184-1482dff8-1363-48c2-b588-3530331e869a.png)





### Páginas Alteradas
Esta secção enumera todas as páginas do tema que foram alteradas. 
Isto é importante, porque, um dia que o tema tenha algum update, seja fácil perceber que páginas foram impactadas.

Nome | Tipo | O que foi alterado
------------ | ------------- | -------------
theme.js | Main theme javascript | Mudanças na função initProductVariant. Conforme a tag que o produto tenha, gera ou não os selectors automaticamente. Ver tags para mais pormenores.
search.liquid | Template | linha 19. De grid_results = false para grid_results = true
 

### Tags
#### Administrativas 
Todas as tags administrativas começam por configuration

Nome | Descrição
------------ | ------------- 
configurationNoDefaultInitProduct | Esta tag é usada para que os seletectors das opções das variantes não sejam automaticamente gerados pelo shopify. 


#### Outras



### Snippets

Nome | Descrição
------------ | ------------- 
snippet-receiving-name |
snippet-offering-name |
snippet-school-receiving-name.liquid  | Este snippet tem algumas instruções para quem preenche o nome da Educadora, Professora (...) a quem se destina o miminho. Neste momento é usado no template sentence.offer.receives 




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
