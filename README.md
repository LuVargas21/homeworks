# homeworks

//ESTAS SON LAS VARIABLES QUE SE REPITEN EN TODO EL PROYECTO

$brand-color: #D1F2EB;
$brand-font: 'Cabin Sketch', cursive;
$container-font: 'Cutive Mono', monospace;
$content-font: 'Times New Roman', Times, serif;
$color-font: #000000;
$color-btn: #ffffff;
$card-boder: #00000020;
$size1: 10px;
$size2: 15px;
$size3: 20px;
$size3b: 25px;
$size4: 40px;
$size5: 50px;
$size6: 100px;
$size7: 250px;
$size8: 90px;
$size9: 80px;


@import "variables";
@import "header";
@import "footer";
@import "grids";
@import "texts";
@import "container";

// MAP DE FOOTER

$redesSociales: (
    YouTube: #ffffff,
    Facebook: #ffffff,
    Instagram: #ffffff,
);

@each $red in $redesSociales {
    .red-# ($red) {
        color: $color;
    }

}

// EXTEND EN CARDS

.card {
    padding: $size2;
    margin: $size2;
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-color: $color-btn;
    background-clip: border-box;
    border: 1px solid $card-boder;
    border-radius: $size1 -6;

}

.card2 {

@extend .card; 
    background-color: #3fbc79;
    border-radius: $size1;
}


//MIXIN 

@mixin containerSize {
    margin: 80px;
    padding: 15px;    
}

.container {
  @include containerSize; 
}


// MODIFICACIONES EN EL FOOTER, AGREGANDO ICONOS DE LIBRERIAS EXTERNAS //
AGREGUÉ UN FAVICON //
AGREGUÉ UNA DESCRIPCION DE LA PAGINA EN TODOS LOS HTML // 
AGREGUE KEYWORDS FIJAS Y VARIABLES EN TODOS LOS HTML // 
// MODIFIQUÉ ALGUNAS COSAS DEL DISEÑO. 
