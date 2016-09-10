# responsive-design
A tutorial and materials for learning responsive design

Exercício Design Responsivo

1. Fazer um fork deste projeto
2. Clonar o seu fork no cloud9
3. Baixar os arquivos deste projeto no cloud9
4. Executar o projeto. Perceba que se trata de um site não responsivo. visualização somente em desktop.
5. Vamos fazer as seguintes alterações para torná-lo responsivo:
6. O segredo para se ter um site responsivo é criá-lo sobre uma base fluida. Isso faz com que o layout seja definido em razões e proporções, ao invés de valores absolutos. Então, temos que converter uma medida exata, em pixel, para uma relativa como "em".
    "EM" está relacionada às fontes (tipografia) onde 1em equivale a 16px que é justamente o tamanho padrão, em média, das fontes nos navegadores.
7. Observe que na linha 5 de seu CSS, as fontes da tag body estão configuradas em 18px. Vamos convertê-la para em:
    18px/16px=1.125em
    Altere o tamanho desta fonte para 1.125em
    font-size: 1.125em;
    Dica: deixe seus cálculos de conversão comentados no código, pois serão úteis mais adiante.
8. A conversão em "em" depende do contexto em que está inserido.
    CUIDADO para não confundir o contexto que deverá ser considerado para realizar uma conversão.
    Qual o valor "em" será atribuído à propriedade line-height na linha 7?
    A propriedade line-height (altura da linha) está ligada diretamente com a fonte do seletor body, por isso que ela é convertida com relação ao body e não, ao navegador. E como o font-size do body é 18px, o valor final será de 1.2222222222em.
    22px/18px=1.2222222222em
    Repare que foi divido por 18px (tamanho original da fonte) e não por 16px, que é o tamanho padrão quando o contexto for o navegador.
9. Para transformarmos uma layout fixo, determinado em pixel, por um flexível, utilizando porcentagem, a ideia é a mesma utilizada para a conversão da tipografia do site. O importante é saber identificar bem quem é o contexto, ou seja, quem é o elemento pai e seu descendente, o elemento filho.
    Siga fazendo as conversões de todas as medidas fixas para "em" ou "porcentagem".
    Siga as orientações do passo a passo: [COMO CRIAR UM SITE RESPONSIVO COM HTML5 E CSS3 – PARTE 3/3](http://www.carloshps.com.br/blog/criar-um-site-responsivo-com-html5-e-css3-parte-3-de-3/)
    Preste atenção nas medidas. Use como referência as que estão em seu CSS.
10. Repare que a propriedade "width" foi substituída por "max-width".
11. Não basta apenas converter os valores absolutos em relativos e achar que seu site já está responsivo. 
    Agora vamos converter o Layout Fluido em Layout Responsivo.
    Sites responsivos são criados sobre layouts fluidos com a ajuda de media queries, para não atingir resoluções de dispositivos específicos, mas  sim, adaptar o design e conteúdo, através de vários pontos de interrupção, chamados de breakpoints, afim de oferecer uma experiência integrada aos usuários.
12. Definir breakpoints.
    Podemos definir breakpoints para as seguintes dimensões:
        320 pixel – Smartphones no formato retrato com tela pequena
        480 pixel – Smartphones no formato paisagem com tela pequena
        768 pixel – Tablets no formato retrato, como o iPad
        960 pixel – Tablets no formato paisagem e alguns monitores mais antigos
        1200 pixel – Desktops, notebooks com monitores widescreen
13. Implementar as Media Queries
    As medias queries, em resumo, são recursos do CSS para reconhecer o dispositivo usado pelo usuário, mudar o layout para este dispositivo sem alterar o conteúdo.
    Use, no menu do CHROME "ferramentas do desenvolvedor" para simular os diferentes dispositivos e verificar as medias queries e seus pontos de interrupção. 
14. Quando seu site estiver responsivo, faça o commit das suas alterações no github.
15. Fazer o push das sua alterações para o github.
16. Abrir o pull request.