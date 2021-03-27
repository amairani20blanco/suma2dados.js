# suma2dados.js
<script>
  class lanzar{
    lanzar1(){return Math.ceil(Math.random ()*6);}
    lanzar2(){return Math.ceil(Math.random ()*6);}
  }
  
  let sumad=[0,0,0,0,0,0,0,0,0,0,0,0],
  suma=0,dado=new lanzar();
  for(let i=1;i<100;i++){
    suma=0;
    let a=dado.lanzar1();
    let b=dado.lanzar2();
    suma=a+b; 
    sumad[suma-2]++;
  }
  for(j=0;j<11;j++)
    document.write("suma de dados: "+(j+2)+"<br>" + sumad[j] + " veces <br>");

</script>
