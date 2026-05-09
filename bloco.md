.header::after {
content: "";

position: absolute;

left: 0;
bottom: 0;

width: 0%;
height: 5px;

background: #146626;

transition: width 0.4s ease;
}

.header:has(.cadastro:hover)::after {
width: 100%;
} // caso queira colocar a linha verde abaixo do botão cadastre-se
