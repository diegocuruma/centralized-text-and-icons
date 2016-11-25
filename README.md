## Exemplo

Texto e ícones centralizados

[veja o exemplo](http://codepen.io/curuma/pen/pNwYjJ)


## Bibliotecas 
- Bootstrap

## Código para o funcionamento.

## HTML 
- index.html
```html
<!doctype html>
<html lang="pt-br">
<head>
	<meta charset="utf-8" />

	<title>Vertical Middle</title>
	<meta name="author" content="Vertical Middle - diego curumim" />
	<meta name="viewport" content="width=device-width, initial-scale=1" />
	
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
	
	<!-- stylo -->
	<style type="text/css">
		@import url(http://fonts.googleapis.com/css?family=Open+Sans);		
	</style> 
	
	<link href="style.css" rel="stylesheet" type="text/css" /> 
	
	<!-- ícone-->
	<link rel="shortcut icon" href="favicon.png"/>
</head>
<body>

	<section class="container">
 	   <header class="tit">
       		<h2>Texto e ícones centralizados</h2>
       </header>

	   <ul class="row">
		   <li class="lista col-md-2 col-xs-6 col-sm-6">
			<a href="#" title="Administração" class="lista__link" style="background-color:#b5a044">
			  <figure class="box">
				<div class="box__item">												
					<img src="http://image.flaticon.com/icons/png/512/3/3729.png" class="box__img">					 
					<h3 class="box__tit">
					Administração																													                                      </h3>                                                                       
				</div>
			  </figure>
			 </a>
		   </li>
		   
		   <li class="lista col-md-2 col-xs-6 col-sm-6">
			<a href="#" title="Alimentação" class="lista__link" style="background-color:#58b6ff">
			  <figure class="box">
				<div class="box__item">												
					<img src="http://image.flaticon.com/icons/png/512/264/264129.png" class="box__img">					 
					<h3 class="box__tit">
					Alimentação
					</h3>                                                                       
				</div>
			  </figure>
			 </a>
		   </li>
		   		   		   
		   <li class="lista col-md-2 col-xs-6 col-sm-6">
			<a href="#" title="Finanças" class="lista__link" style="background-color:#6d4488">
			  <figure class="box">
				<div class="box__item">												
					<img src="http://image.flaticon.com/icons/svg/134/134654.svg" class="box__img">					 
					<h3 class="box__tit">
					Finanças
					</h3>                                                                       
				</div>
			  </figure>
			 </a>
		   </li>
		   
		   <li class="lista col-md-2 col-xs-6 col-sm-6">
			<a href="#" title="Visa" class="lista__link" style="background-color:#f99349">
			  <figure class="box">
				<div class="box__item">																	
					<img src="http://image.flaticon.com/icons/svg/39/39134.svg" class="box__img">
				</div>
			  </figure>
			 </a>
		   </li>
		   
		   <li class="lista col-md-2 col-xs-6 col-sm-6">
			<a href="#" title="Shows" class="lista__link" style="background-color:#5fc778">
			  <figure class="box">
				<div class="box__item">																	
					<h3 class="box__tit">
					Shows
					</h3>                                                                       
				</div>
			  </figure>
			 </a>
		   </li>
		   
		   <li class="lista col-md-2 col-xs-6 col-sm-6">
			<a href="#" title="Marketing e Tecnologia" class="lista__link" style="background-color:#e1556f">
			  <figure class="box">
				<div class="box__item">																	
					<h3 class="box__tit">
					Marketing e Tecnologia
					</h3>                                                                       
				</div>
			  </figure>
			 </a>
		   </li>
		 </ul>  
	</section> 
	   
</body>
</html>
```

## Código CSS
- styles.scss
```css
/*
|----------------------------------------------
| Reset
|----------------------------------------------
*/
*, html, body {margin:0; padding:0; font-size:100%;}
body {font:0.93em Arial, sans-serif; color:#000; text-align:left; line-height:1.3em;}
	a {text-decoration:none; color:#1a1a1a;}
	//a:hover {}
	img, a img, fieldset {border:0;}
	address, em {font-style:normal;}
	li {list-style-type:none;}	
	p{
        font-family: 'Open Sans';
        text-align: justify; 
        color:#2a2a2a; 
        line-height:25px;
    }	
	
//for para cores e margin nos titulos

 @for $i from 1 through 6 {
   h#{$i} {      
      font-family: 'Open Sans';
     }
 }





// títulos
.tit{
	margin:80px 0 40px; 
}

// vertical middle => 
.lista{
	&__link{
		display: block;
		&:hover{
			background-color: #b9c4d3 !important
		}
	}
}
.box{
	display:inline-table;
	height:150px;
	width:100%;
	text-align:center;
	&__item{
		display: table-cell;
		vertical-align: middle;	
		text-align:center;		
		font-family: 'Open Sans';
		font-size: .9em;
		color: #fff;
	}
	
	&__tit{
		font-size:1.2em
	}
	&__img{
		margin: 0 auto;
    width:32px;
    height:32px;    
	}
}


```


