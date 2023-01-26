```html
#Form HTML 

  

É um dos principais pontos de interação do usuário com a web ou app. 

Após os dados serem preenchidos, eles são enviados para um servidor ou a própria página pode processá-los. 

Para esse post, vou usar uma forma mais resumida do form. Então, vamos usar as seguintes tags : 

<form><label><input><textarea><button>  

Todo formulário começa com <form> 

<form action="/pagina-processa-dados-do-form" method="post"></form> 

 
OBS: ele trabalha com muitos atributos, mas é uma boa prática caso não precise de todos, o mínimo para manter uma boa prática são dois, 
e sobre os quais irei detalhar agora: 

Action: define a URL para onde os dados são enviados 

Method: define o método HTML, GET ou POST. 

 

Vamos trabalhar um exemplo, observe como as **divs** agrupa os conjuntos de tags: 
 
 
  <form action="/pagina-processa-dados-do-form" method="post"> 
    <div> 
        <label for="nome">Nome:</label> 
        <input type="text" id="nome" /> 
    </div> 
    <div> 
        <label for="email">E-mail:</label> 
        <input type="email" id="email" /> 
    </div> 
    <div> 
        <label for="msg">Mensagem:</label> 
        <textarea id="msg" name="msg" 

          rows="5" cols="33">Mesagem digitada</textarea> 
    </div> 

<div class="button"> 
        <button type="submit">Enviar sua mensagem</button> 
    </div> 
</form> 

 
 

Com esse exemplo, vamos trabalhar algumas informações: 

<label</label>  

Responsável por mostrar uma informação na tela, usada apenas para definir de forma visual o que o usuário deve fazer no campo logo 
abaixo dela. Ela usa um atributo chamado for, assim, ele é responsável por vincular a label a uma entrada (input) de dados. 

 

<input/>

É responsável por receber a informação do usuário, e assim como a label, ele necessita de um atributo chamado de id, ele vincula a label ao input. 
Então esse vínculo, é usado para que, ao clicar na label, ela possa posicionar o curso no input, e assim deixar a interação mais fácil. 

 

OBS: essas duas tags iniciais, trabalham de maneira “conjuntas”, sendo a primeira que direciona o usuário e informa o que deve ser feito ao preencher os dados no input. 

<label for="nome">Nome:</label> 
<input type="text" id="nome" /> 
 

Contudo, o <input/> recebe um atributo que nele podemos passar valores que muda completamente as características da tag. Assim, faz-se necessária 
uma atenção especial ao atributo “type”. No nosso caso, usamos esses atributos em dois momentos e com dois tipos de parâmetros diferentes: 

<input type="text" id="nome" /> o “text” informa a tag, que ela receberá um texto simples, esse valor é basicamente o valor padrão. 

<input type="email" id="email" /> o “email”, ele dar ao input a possibilidade de analisar o que foi difitado, assim ele pode analisar, fazer testes para 
saber o se o que foi digitado é coerente para um endereço de e-mail. 

Na sequência, vou deixar uma lista com alguns valores que poderão ser usado no type, e caso queira saber mais sobre alguns deles, basta consultar no link 
logo abaixo.” https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Input 

Os valores para o type são: button, checkbox, color, date, datetime, datetime-local, email, file, hidden, image, month, number, password, radio, 
range(aqui temos algumas especificações), reset, search, submit, tel, text, time, url, week. 

 

<textarea></textarea>  

É destinada a receber texto do usuário, assim, ele recebe alguns parâmetros:  

Rows e Cols: usados para definir o tamanho da caixa de texto, assim é possível estilizar a caixa para o tamanho ideal, mas eles não delimitam o tamanho do texto, caso o conteúdo ultrapasse o valor definido no rows e cols, o HTML automaticamente cria uma barra de scroll.  
 

<button></button> 

É o botão, responsável por finalizar o processo de cadastro. 

 

https://developer.mozilla.org/pt-BR/docs/Learn/Forms/Your_first_form
```
