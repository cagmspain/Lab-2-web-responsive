@import url(./base.css);

body {
display: grid;
grid-template-rows: 10rem 2rem 1fr 2rem;
}

/\*\*

- ############
- ## Header
- ############
  \*/

header {
display: flex;
flex-direction: column;
align-items: center;
justify-content: space-evenly;
background-image: url("./background.jpeg");
color: white;
}
header div button.whiteuno {
background-color: white;
width: 110px;
height: 30px;
border-radius: 25px;
}
header div button.bluedos {
background-color: blue;
color: white;
width: 110px;
height: 30px;
border-radius: 25px;
}
header form input {
border-radius: 25px;
border: solid transparent;
background-color: rgba(255, 255, 255, 0.4);
}
header ul {
display: flex;
gap: 1rem;
list-style: none;
}
header ul li a {
text-decoration: none;
color: white;
}

header > nav > menu {
display: flex;
gap: 1rem;
}
nav > menu img {
border-radius: 50%;
}

header > nav > menu > li {
display: flex;
align-items: center;
}

/\*\*

- #########
- ## Nav
- #########
  \*/

body > nav > menu {
display: flex;
/_ justify-content: space-evenly; _/
}

/\*\*

- ##########
- ## Main
- ##########
  \*/

main {
display: flex;
flex-wrap: wrap;
justify-content: space-evenly;
gap: 1rem;
}

main > article {
display: flex;
flex-direction: column;
}

main > article > p.description {
flex-grow: 1;
}

/\*\*

- ############
- ## Footer
- ############
  \*/

body > footer {
display: flex;
justify-content: space-evenly;
align-items: center;
}

/\*\*

- #############################################
- ## Cuando el ancho máximo supere los 600px
- #############################################
  \*/

@media (min-width: 600px) {
body {
grid-template-rows: 5rem 1fr 2rem;
grid-template-columns: 10rem 1fr;
}

    body > header,
    body > footer {
    	grid-column: span 2;
    }

    body > header {
    	flex-direction: row;
    	justify-content: space-between;
    	align-items: center;
    }

    body > nav > menu {
    	flex-direction: column;
    }

    body > footer {
    	justify-content: center;
    	gap: 2rem;
    }

}

- {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }

body {
min-height: 100vh;
}

nav menu {
list-style: none;
}

/_ HEADER _/

header form {
width: fit-content;
box-shadow: var(--shadow);
}

header form label {
display: none;
}

header form input {
padding: 0.3rem;
outline: none;
border: none;
}

header menu a {
display: inline-block;
font-size: 0;
height: 1.5rem;
width: 1.5rem;
background-size: contain;
}

/_ NAV_/

body > nav menu li {
width: 100%;
}

body > nav menu a {
text-align: center;
color: black;
text-decoration: none;
display: block;
width: 100%;
height: 100%;
padding: 0.5rem 0;
}

body > nav menu a:hover {
background: var(--background);
}

/_ MAIN _/

main {
background: var(--background);
padding: 1rem;
}

article {
border: 2px solid rgba(255, 255, 255, 0.6);
width: 15rem;
height: 15rem;
border-radius: 10px;
overflow: hidden;
}

article img {
width: 100%;
height: 100%;
object-fit: cover;
}

article p.price {
text-align: right;
}

/_ FOOTER _/

footer a {
color: var(--primary);
width: max-content;
}

/_ MEDIA QUERY _/
@media (min-width: 600px) {
/_ HEADER _/

    header {
    	z-index: 1;
    	padding: 0 2rem;
    }

    /* NAV */

    body > nav {
    	padding-top: 1rem;
    }

    body > nav menu a {
    	text-align: left;
    	padding-left: 0.5rem;
    }

}
