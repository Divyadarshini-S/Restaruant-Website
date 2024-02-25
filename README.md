spicy hut/CSS/style.css
@@ -0,0 +1,209 @@
:root{
     --red:crimson;
    --green:#53BF9D;
    --yellow:#FFC54D;
    --white:whitesmoke;
}

body,h2{
    margin:0;
    font-family: Arial, Helvetica, sans-serif;
}

.landing{
    background-image: url('../media/bg.jpg');
    background-size: cover;
    background-position: center;
    height:100vh;
    color:var(--white);
}

header a{
    text-decoration: none;
    color:var(--yellow);
    min-width: 120px; 
}

header{
    display:flex;
    flex-wrap:wrap;
    row-gap:1em;
    padding:1em;
}

#logo{
    flex:3;
    font-size:1.25em;
    min-width:260px;
}

nav{
    flex:2;
    display:flex;
    align-items: center;
}   

nav a{
    flex:1;
}

nav a:hover{
    color:var(--green);
}

header h2 i,nav a i{
    margin-right: .5em; 
}


.maintext{
    display:flex;
    flex-direction:column;
    height:50vh;
    justify-content: center;
    padding:2em;
}

.tagline1{
    color:var(--red);
    font-size:2.5em;
    font-weight: bolder;
}

.tagline2{
    color:var(--yellow);
}

.maintext div{
    margin-top:.75em;
}

.maintext button{
    width:20vw;
    margin-top:2em;
    border-radius:10px;
    padding:.7em;
    background-color: var(--green);
    color:var(--white);
    border: 1px solid var(--green);
}

.menu{
    display:grid;
    grid-template-columns: repeat(auto-fit,minmax(320px,1fr));
    background:linear-gradient(to right,rgb(100, 100, 100),rgb(53, 52, 52));
    color:var(--white);
}

#menuheading,#locheading{
    background:linear-gradient(to right,rgb(100, 100, 100),rgb(53, 52, 52));
    font-size:2.5em;
    color:var(--red);
    display: flex;
    justify-content: center;
}

.menu th{
    color:var(--green);
    font-size: 1.8em;
}

table{
    width:100%;
    padding:1em;
}

.menu tr{
    display:flex;
    justify-content: center;
    margin-top:.8em;
}

.menu td:nth-child(1){
    flex:1;
    justify-self: left;
}


.menu td:nth-child(2){
    justify-self: right;
}

.maincourse{
    grid-row:span 2;
}

.locations{
    background:linear-gradient(to right,rgb(100, 100, 100),rgb(53, 52, 52));
    color:var(--white);
    display:flex;
    flex-wrap:wrap;
}

.locations h2{
    color:var(--green);
    margin-bottom: .8em;
}

.locations div{
    flex:1;
    padding:1em;
    min-width:220px;
}

footer{
    background-color: rgb(55, 55, 55);
    color:var(--white);
    padding:.25em 1em;
}

#copyright{
    margin-left:20px;
}
.social-menu ul{
    display: flex;
    padding:0;
}

.social-menu ul li{
    list-style: none;
    display:inline-block;
    margin: 0 15px;
}

.social-menu ul li .fab{
    font-size: 25px;
    line-height: 40px;
    transition: .3s;
    color: #000;
}

.social-menu ul li .fab:hover{
    color: #fff;
}

.social-menu ul li a{
    position: relative;
    display: block;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: #fff;
    text-align: center;
    transition: .6s;
    box-shadow: 0 5px 4px rgba(0,0,0,.5);
}

.social-menu ul li a:hover{
    transform: translate(0, -10%);
}

.social-menu ul li:nth-child(1) a:hover{
    background-color: #4267B2;
}
.social-menu ul li:nth-child(2) a:hover{
    background-color: #E4405F;
}
.social-menu ul li:nth-child(3) a:hover{
    background-color: #00ACEE;
}
