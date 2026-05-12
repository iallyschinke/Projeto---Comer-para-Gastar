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

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  background: #eef0e8;
  font-family: Arial, Helvetica, sans-serif;
  padding: 120px 20px 8px;

  background:
    radial-gradient(circle at center, #ffffff 0%, transparent 38%),
    linear-gradient(90deg, #eef4d8 0%, #f8f8ef 50%, #dfe8ad 100%);
}

/* HEADER FIXO */

.header {
  position: fixed;
  top: 15px;
  left: 50px;
  right: 50px;
  z-index: 999;
  background: white;
  border-radius: 25px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px 65px;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
}

/* LOGO */

.logo {
  display: flex;
  align-items: center;
  height: 80px;
  overflow: hidden;
}

.logo img {
  width: 220px;
  height: auto;
}

/* MENU */

.menu {
  display: flex;
  align-items: center;
  gap: 55px;
  margin-right: -80px;
}

.menu a {
  text-decoration: none;
  color: #1d7a2f;
  font-size: 20px;
  font-weight: 500;
  position: relative;
  transition: 0.3s;
}

/* LINHA HOVER DO MENU */

.menu a::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -8px;
  width: 0%;
  height: 3px;
  background: #1d7a2f;
  border-radius: 10px;
  transition: 0.3s;
}

/* APARECE AO PASSAR O MOUSE */

.menu a:hover::after {
  width: 100%;
}

/* COR AO PASSAR */

.menu a:hover {
  color: #0f3517;
}

/* ÁREA DIREITA DO HEADER */

.acoes-header {
  display: flex;
  align-items: center;
  gap: 12px;
}

/* BOTÃO CADASTRO */

.cadastro {
  background: #146626;
  color: white;
  text-decoration: none;
  border: none;
  border-radius: 14px;
  padding: 16px 30px;
  font-size: 18px;
  font-weight: bold;
  cursor: pointer;
  transition: 0.3s;
  margin-right: -300px;
}

/* REMOVE QUALQUER LINHA */

.cadastro::after {
  display: none;
}

.cadastro:hover {
  background: #0d4e1a;
  color: white;
}

/* BOTÃO ENTRAR */

.entrar {
  background: #146626;
  color: white;
  border: none;
  border-radius: 14px;
  padding: 16px 30px;
  font-size: 18px;
  font-weight: bold;
  cursor: pointer;
  transition: 0.3s;
}

.entrar:hover {
  background: #0d4e1a;
}

main,
.secao {
  scroll-margin-top: 130px;
}

.secao {
  min-height: 500px;
  padding: 80px 20px;
  text-align: center;
  border-top: 2px solid rgba(20, 102, 38, 0.12);
  box-shadow:
    0 -8px 20px rgba(0, 0, 0, 0.03),
    0 8px 20px rgba(0, 0, 0, 0.03);
  margin-top: 80px;
}

.secao h1 {
  font-size: 72px;
  color: #146626;
  margin-bottom: 30px;
}

.folha-centro {
  display: flex;
  justify-content: center;
  margin-top: -30px;
}

.folha-centro img {
  width: 200px;
  height: auto;
}

.name5 {
  font-size: 50px;
  font-weight: bold;
  color: #146626;
  text-align: center;
}

.texto-centro {
  text-align: center;
  margin-top: -30px;
}

.texto-centro p {
  font-size: 20px;
  line-height: 1.6;
  color: #333;
}

.text1 {
  color: #0d4e1a;
  font-weight: bold;
}

.conteudo-imagens {
  position: relative;
  margin-top: 40px;
  min-height: 560px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.gastos-caloricos {
  background-color: #0d4e1a;

  width: fit-content;

  margin: 0 auto;

  display: flex;
  justify-content: center;
  align-items: center;

  padding: 0;

  border-radius: 30px;
  overflow: hidden;

  position: relative;
  z-index: 10;
}

.gastos-caloricos img {
  width: 800px;
  max-width: 100%;
  display: block;
  border-radius: 30px;
}

.img-lateral {
  width: 380px;
  position: absolute;
  right: 80px;
  top: 120px;
}

.img-lateral-2 {
  width: 380px;
  position: absolute;
  left: 80px;
  top: 160px;
}

.cta-final {
  background: white;

  width: fit-content;

  margin: 40px auto 80px;

  padding: 20px 28px;

  border-radius: 22px;

  display: flex;
  align-items: center;
  justify-content: space-between;

  gap: 30px;

  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.06);
}

.cta-esquerda {
  display: flex;
  align-items: center;
  gap: 20px;
}

.icone-folha {
  width: 70px;
  height: 70px;
  background: #dfe8c8;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.icone-folha img {
  width: 200px;
}

.texto-cta p {
  font-size: 18px;
  color: #3d3d3d;
}

.texto-cta h2 {
  font-size: 22px;
  color: #146626;
  font-weight: bold;
}

.botao-cta {
  position: relative;
  z-index: 20;
  background: #146626;
  color: white;
  border: none;
  border-radius: 14px;
  padding: 16px 30px;
  font-size: 18px;
  font-weight: bold;
  cursor: pointer;
  transition: background 0.3s ease;
}

.botao-cta:hover {
  background: #0d4e1a;
}

/* TÍTULO DAS SESSÕES */

.historia {
  min-height: 100vh;
  padding: 90px 60px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 80px;
}

.historia-texto {
  width: 43%;
}

.historia-texto h1 {
  font-size: 82px;
  line-height: 0.95;
  color: #146626;
  margin-bottom: 25px;
}

.linha-historia {
  width: 120px;
  height: 4px;
  background: #146626;
  border-radius: 20px;
  margin-bottom: 35px;
}

.historia-texto p {
  font-size: 22px;
  line-height: 1.55;
  color: #214b2a;
  margin-bottom: 30px;
  text-align: left;
  align-items: flex-start;
}

.historia-texto strong,
.historia-card strong {
  color: #146626;
}

.historia-2 {
  color: #214b2a;
  text-align: left;
}

.botao-whats {
  background: #23862f;
  color: white;
  border: none;
  border-radius: 20px;
  padding: 18px 35px;
  font-size: 24px;
  cursor: pointer;
}

.historia-card {
  width: 44%;
  background: #f8f9f1;
  border: 2px solid #dfe8c8;
  border-radius: 28px;
  padding: 45px;
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
}

.ano {
  background: #0d8a3a;
  color: white;
  width: fit-content;
  padding: 15px 30px;
  border-radius: 18px;
  font-size: 35px;
  font-weight: bold;
  margin-bottom: 35px;
  display: flex;
  align-items: center;
  gap: 12px;
}

.ano img {
  width: 38px;
  height: 38px;

  object-fit: contain;
}

.historia-card > p {
  font-size: 25px;
  line-height: 1.6;
  color: #214b2a;
  margin-bottom: 50px;
}

.historia-itens {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.historia-itens div {
  text-align: center;
  color: #146626;
  border-right: 2px solid #dfe8c8;
  padding: 0 10px;
}

.historia-itens div:last-child {
  border-right: none;
}

.historia-itens span {
  font-size: 45px;
  display: block;
  margin-bottom: 10px;
}

.historia-itens p {
  font-size: 15px;
  line-height: 1.4;
  font-weight: bold;
}

.titulo-historia img {
  position: absolute;

  width: 100px;

  right: -65px;
  top: 48px;

  transform: rotate(8deg);
}

.titulo-historia span {
  color: #4b9e4d;
}

/* DICAS */

.dicas {
  min-height: 100vh;
  padding: 120px 60px 100px;
  text-align: center;
}

.titulo-dicas h1 {
  font-size: 72px;
  color: #146626;
  margin-bottom: 20px;
}

.titulo-dicas p {
  font-size: 28px;
  color: #4b4b4b;
  margin-bottom: 20px;
}

.linha-dicas {
  width: 110px;
  height: 6px;
  background: #146626;
  border-radius: 20px;
  margin: 0 auto 45px;
}

.cards-dicas {
  display: flex;
  justify-content: center;
  gap: 35px;
  flex-wrap: wrap;
}

.card-dica {
  width: 360px;
  min-height: 540px;
  background: #ffffff;
  border-radius: 24px;
  padding: 35px 28px;
  box-shadow: 0 8px 22px rgba(0, 0, 0, 0.08);
}

.imagem-dica {
  width: 250px;
  height: 250px;
  margin: 0 auto 25px;
  border-radius: 50%;
  background: #e8f3dc;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  position: relative;
}

.imagem-dica img {
  width: 210px;
  height: 480px;
  object-fit: contain;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.imagem-dica-2 {
  width: 250px;
  height: 250px;
  margin: 0 auto 25px;
  border-radius: 50%;
  background: #e8f3dc;
  align-items: center;
  display: flex;
  align-items: center;
  justify-content: center;
}

.imagem-dica-2 img {
  object-fit: contain;
  width: 280px;
  height: 280px;
}

.imagem-dica-3 {
  width: 250px;
  height: 250px;
  margin: 0 auto 25px;
  border-radius: 50%;
  background: #e8f3dc;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  position: relative;
}

.imagem-dica-3 img {
  width: 280px;
  height: 480px;
  object-fit: contain;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.card-dica h2 {
  font-size: 30px;
  line-height: 1.1;
  color: #23862f;
  margin-bottom: 15px;
}

.linha-card {
  width: 45px;
  height: 3px;
  background: #23862f;
  border-radius: 20px;
  margin: 0 auto 18px;
}

.card-dica p {
  font-size: 18px;
  line-height: 1.5;
  color: #146626;
  margin-bottom: 28px;
}

.card-dica button {
  width: 42px;
  height: 42px;
  border-radius: 50%;
  border: 3px solid #23862f;
  background: white;
  color: #23862f;
  font-size: 24px;
  font-weight: bold;
  cursor: pointer;
}

.titulo-historia {
  position: relative;

  text-align: left;
  align-items: flex-start;
  width: fit-content;

  font-size: 82px;
  line-height: 0.9;

  color: #146626;

  font-weight: bold;
}
